# 🧪 Interview Prep — SwiftyBite
> **`INTERVIEW.md`** is a template use to prepare for iOS/Swift developer interviews. It includes sections for technical Q\&A, behavioral prep, common challenges, and whiteboard/code exercises.


A curated list of technical and behavioral questions, answers, and resources to help me prepare for iOS developer interviews.

---

## 📘 Swift Basics

* **What is an optional in Swift?**
  An optional represents a variable that can hold a value or no value (`nil`). It is declared with a `?`.

  ```swift
  var name: String? = "Swifty"
  ```

* **What’s the difference between `struct` and `class`?**
  `struct` is a value type (copied on assignment), while `class` is a reference type (shared reference).

* **Explain `guard` vs `if let` for unwrapping.**
  `guard` is used for early exit and improves readability when conditions fail.

  ```swift
  guard let name = name else { return }
  ```

---

## 🧱 UIKit & SwiftUI

* **How does navigation work in UIKit vs SwiftUI?**

  * UIKit: `UINavigationController`, segues
  * SwiftUI: `NavigationStack`, `NavigationLink`

* **What is a `@State` and `@Binding` in SwiftUI?**

  * `@State` is for local view state
  * `@Binding` allows passing a reference to a state variable from a parent view

---

## 🔄 Architecture & Patterns

* **What is MVVM and how is it used in iOS apps?**
  MVVM stands for Model-View-ViewModel.

  * `Model`: data layer
  * `View`: UI
  * `ViewModel`: logic that binds model to the view

* **What are delegates and how do they work?**
  Delegation is a design pattern where one object acts on behalf of another. Used often in UIKit.

---

## 🌐 Networking

* **How do you make a network call in Swift?**
  Using `URLSession`, with or without `async/await`.

  ```swift
  let (data, _) = try await URLSession.shared.data(from: url)
  ```

* **How do you decode JSON in Swift?**
  Using `Codable` with `JSONDecoder`.

---

## 🧪 Coding Challenges (Whiteboard / Interview)

* Reverse a string
* Check for palindrome
* Merge two sorted arrays
* Fibonacci (recursive and iterative)
* LRU cache pattern
* Implement a custom `Button` in SwiftUI
* API request with retry logic

---

## 👥 Behavioral / Soft Skills

* Tell me about a time you faced a difficult bug.
* How do you handle version control with teams?
* Why iOS development? What do you enjoy about it?
* How do you learn new frameworks/libraries?

---

## 🧰 Tools & Tips

* **Prepare a portfolio of 3–5 apps on GitHub**
* Use `Playgrounds` or `LeetCode` for daily Swift practice
* Mock interviews via [pramp.com](https://www.pramp.com), [exponent](https://www.tryexponent.com/)
