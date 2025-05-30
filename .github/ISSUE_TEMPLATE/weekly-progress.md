name: 📘 Weekly Progress Log
description: Track this week’s learning & coding
title: "[Progress] Week X: "
labels: ["progress", "weekly"]
body:
  - type: input
    id: week
    attributes:
      label: Week #
      placeholder: e.g., Week 10
  - type: input
    id: date
    attributes:
      label: Date Range
      placeholder: e.g., June 1 – June 7
  - type: textarea
    id: learned
    attributes:
      label: ✅ What I Learned
      placeholder: Topics, concepts, etc.
  - type: textarea
    id: built
    attributes:
      label: 🔧 What I Built
      placeholder: Projects, code, links
  - type: textarea
    id: next
    attributes:
      label: 🎯 What’s Next
      placeholder: Topics or tasks for next week
