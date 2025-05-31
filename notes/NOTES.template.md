# 📝 Notes — SwiftyBite

A place to collect all my Swift and iOS development notes, quick code snippets, explanations, and useful links.

---

## 📅 Weekly Notes

### Week \[#] — \[Topic/Focus]

**Date:** YYYY-MM-DD

**Summary:**
Short overview of what I learned this week.

---

### Concepts & Definitions

* **Swift Optionals:**
  Variables that may or may not hold a value. Use `?` for optional type, `!` to force unwrap carefully.
  Example:

  ```swift
  var name: String? = "ChatGPT"
  print(name ?? "No name")
  ```

* **MVVM Pattern:**
  Model-View-ViewModel architectural pattern to separate UI and business logic.

---

### Code Snippets

```swift
// Example: Function to reverse a string
func reverseString(_ str: String) -> String {
    return String(str.reversed())
}
```

---

### Useful Links

* [Swift Language Guide](https://docs.swift.org/swift-book/)
* [100 Days of SwiftUI](https://www.hackingwithswift.com/100/swiftui)
* [Apple Developer Documentation](https://developer.apple.com/documentation/)

---

### Questions / Challenges

* How does `@State` differ from `@Binding` in SwiftUI?
* Best practices for error handling in async/await?

---

### Ideas to Explore

* Experiment with Combine framework
* Try creating a small SwiftUI animation
