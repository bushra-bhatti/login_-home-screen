# Week 1 Assignment: Basic Flutter Development and UI Building

This repository contains the submission for the Week 1 Flutter assignment. The project demonstrates the setup of a Flutter development environment, building a responsive Login UI, implementing form validation using Regular Expressions, and navigating between screens.

---

## 🎯 Learning Objectives Completed
- Understand Flutter's basic structure and feature-first folder management.
- Build simple, structured, and responsive user interfaces.
- Learn and implement explicit navigation between screens.

---

## 🛠️ Tasks Accomplished

### 1. Environment Setup
- Successfully installed and configured the Flutter SDK.
- Configured the integrated development environment (IDE) using VS Code / Android Studio.
- Created a clean, functional base Flutter project template.

### 2. Basic UI Construction
Built a complete, responsive login interface using core structural widgets:
- **Container & SafeArea:** Used to provide structural boundaries and padding.
- **Column & Row:** Used to align input fields vertically and layout components (like the "Forgot Password" link) horizontally.
- **TextFormFields:** Implemented two distinct input fields specifically dedicated to capturing Email and Password data.
- **Buttons:** Implemented an `ElevatedButton` for the primary login trigger and a `TextButton` for the "Forgot Password?" utility.

### 3. Form Validation Implementation
- **Email Validation:** Configured a runtime Regular Expression (RegEx) check to ensure the user enters a properly formatted email address (e.g., user@example.com).
- **Password Validation:** Added a mandatory null-safety check to ensure the password input field cannot be left blank or empty.

### 4. Navigation Between Screens
- Developed a secondary target screen (**Home Screen**) that acts as the post-authentication dashboard.
- Implemented explicit screen transitions using `Navigator.push()` to route the user safely from the Login Screen to the Home Screen upon successful validation.

---

## 📂 Project Directory Structure

The project code is organized into separate files under the `lib/` directory to follow clean coding standards:

```text
lib/
│
├── main.dart                      # App entry point and Material configuration
│
├── core/
│   └── constants/
│       └── app_strings.dart       # Centralized app text and validation strings
│
└── features/
    ├── auth/
    │   └── screens/
    │       └── login_screen.dart  # Login UI with Form fields & validation logic
    │
    └── home/
        └── screens/
            └── home_screen.dart   # Welcome dashboard screen after navigation
