name: 📘 Weekly Progress Log
description: Log what I learned, built, and plan next.
title: "[Progress] Week ##: e.g. SwiftUI Basics"
labels: ["progress", "weekly"]

body:
  - type: input
    id: date
    attributes:
      label: Date Range
      placeholder: e.g., May 30 – June 6
  - type: textarea
    id: learned
    attributes:
      label: ✅ What I Learned
      description: Summarize concepts, topics, etc.
  - type: textarea
    id: built
    attributes:
      label: 🔧 What I Built
      description: Mention any apps, playgrounds, commits
  - type: textarea
    id: next
    attributes:
      label: 🎯 What's Next
      description: Set goals or topics for next week
