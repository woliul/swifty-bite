# 🧾 Git & GitHub Best Practices

Welcome! This guide defines the Git and GitHub best practices followed in this project. These standards simulate an in-house team environment, ensuring code quality, collaboration readiness, and traceable progress — even for a solo learner.

---

## 🔖 Table of Contents

1. [Branching Strategy](#-branching-strategy)
2. [Commit Conventions](#-commit-conventions)
3. [Pull Request Etiquette](#-pull-request-etiquette)
4. [Merge Guidelines](#-merge-guidelines)
5. [Git Workflow Summary](#-git-workflow-summary)
6. [Folder & File Naming](#-folder--file-naming)
7. [README & Documentation](#-readme--documentation)
8. [Common Commands Reference](#-common-commands-reference)

---

## 🌿 Branching Strategy

A clean branching model helps isolate features, bug fixes, and experiments.

### Branch Naming Convention

Examples:

- `feature/uikit-notes-section`
- `fix/button-alignment-bug`
- `chore/update-contributing-doc`

### Common Branch Types

| Type     | Use case                              |
|----------|----------------------------------------|
| `feature/` | New features, projects, or modules    |
| `fix/`     | Bug fixes or regressions             |
| `chore/`   | Config updates, tooling, docs        |
| `refactor/`| Internal refactors (no behavior change) |

> 💡 Always create a new branch for any non-trivial work.

---

## ✅ Commit Conventions

Use **conventional commits** for clarity and structured history.

### Commit Types

| Type       | Purpose                               |
|------------|----------------------------------------|
| `feat`     | New feature or functionality           |
| `fix`      | Bug fix or patch                       |
| `docs`     | Documentation-only changes             |
| `style`    | Formatting, missing semicolons, etc.   |
| `refactor` | Code change that doesn't fix a bug     |
| `test`     | Adding or modifying tests              |
| `chore`    | Misc tasks (configs, tooling updates)  |

**Examples:**

- `feat(swiftui): add quote list view`
- `fix(api): handle empty response from endpoint`
- `docs(notes): restructure README with learning path`

---

## 🚀 Pull Request Etiquette

When using GitHub PRs (now or in future teams):

- **Name clearly**: Use a descriptive title (e.g., "Add Crypto API integration")
- **Link issues** (if any): `Closes #12`
- **Checklist** before requesting review:
  - [ ] Code compiles
  - [ ] No debug logs or commented code
  - [ ] Project builds and runs

> Solo dev? Use PRs as changelogs, or to review before merging.

---

## 🔀 Merge Guidelines

- Only merge into `main` when tested or reviewed.
- Rebase or squash commits for clean history.
- Avoid merge commits unless handling divergent branches.

### Suggested Strategy:

```bash
# Rebase before merge
git checkout main
git pull origin main
git checkout feature/my-feature
git rebase main
# Test locally
git checkout main
git merge --squash feature/my-feature
````

---

## 📌 Git Workflow Summary

```bash
# Start new work
git checkout -b feature/new-uikit-app

# Make changes
git add .
git commit -m "feat(uikit): add new onboarding screen"

# Sync with main
git pull origin main --rebase

# Push branch
git push origin feature/new-uikit-app
```

Use `git stash` if switching branches mid-work.
Commit often, push daily.

---

## 📁 Folder & File Naming

* Use `kebab-case` for files and folders
* Avoid vague names like `test.swift` or `notes.md`
* Use date prefixes if helpful: `2025-06-10-uikit-overview.md`

---

## 📘 README & Documentation

Each major folder (e.g., `notes/`, `projects/`, `interview-prep/`) should have a `README.md`:

### Minimum Content

* Purpose of folder
* File organization (topics, months, etc.)
* How to contribute (if applicable)

Example:

```markdown
# Notes/
This folder contains concept-wise Swift and iOS notes, organized by topics and projects.  
✅ Use this as a quick reference for future review or interviews.
```

---

## 🧠 Common Commands Reference

```bash
# Create branch
git checkout -b feature/app-logic

# Commit changes
git add .
git commit -m "feat: complete task manager core"

# Rebase with main
git pull origin main --rebase

# Push
git push origin feature/app-logic

# Merge (squash recommended)
git checkout main
git merge --squash feature/app-logic
```

---

## 🧭 Future-Proofing

Even for solo learners, using professional practices:

* Keeps your GitHub portfolio clean and impressive
* Builds habits useful in actual dev teams
* Makes it easier to share, expand, or collaborate in future

---

Thanks for following best practices! 👨‍💻🍏
