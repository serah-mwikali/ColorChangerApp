# ColorChangerApp
## Overview

Color Changer App is a simple Android application built using **Kotlin** and **Jetpack Compose**. The app allows users to change the background color of the screen by clicking different color buttons.

This project is designed for beginners learning Android development and demonstrates the fundamentals of Jetpack Compose, including state management, layouts, modifiers, and UI recomposition.

---

## Features

* Change background color to Red
* Change background color to Blue
* Change background color to Green
* Responsive UI built with Jetpack Compose
* Real-time UI updates using Compose State

---

## Learning Objectives

This project helps developers understand:

* Jetpack Compose fundamentals
* Composable functions
* State management using `remember` and `mutableStateOf`
* Layouts using `Column`
* Modifiers
* Button click events
* UI recomposition
* Basic Android application structure

---

## Technologies Used

* Kotlin
* Android Studio
* Jetpack Compose
* Material 3

---

## Project Structure

```text
ColorChangerApp
│
├── MainActivity.kt
│
└── ColorChangerScreen()
```

---

## How It Works

1. The application starts from `MainActivity`.
2. `setContent()` loads the Compose UI.
3. A state variable stores the current background color.
4. When a button is clicked, the state changes.
5. Jetpack Compose automatically recomposes the UI and updates the background color.

---

## Key Concepts Demonstrated

### State Management

```kotlin
var backgroundColor by remember {
    mutableStateOf(Color.White)
}
```

Stores and updates the current background color.

### Button Click Events

```kotlin
Button(
    onClick = {
        backgroundColor = Color.Red
    }
)
```

Changes the state when the button is clicked.

### Recomposition

Whenever the state changes, Compose automatically redraws the affected UI components.

---

## Installation

1. Clone the repository:

```bash
git clone https://github.com/yourusername/ColorChangerApp.git
```

2. Open the project in Android Studio.

3. Sync Gradle files.

4. Run the application on an emulator or Android device.

---

## Future Improvements

* Add more colors
* Add random color generation
* Implement dark mode
* Add color picker functionality
* Add animations during color transitions
* Save selected color using DataStore

---

## Expected Output

Users can press different buttons to instantly change the background color of the application screen.

---

## Author

Developed as part of a Jetpack Compose learning journey to understand Android UI development and state management.
