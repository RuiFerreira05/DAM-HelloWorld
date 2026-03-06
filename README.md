# Assignment TP1 — Hello World
Course: Desenvolvimento de Aplicações Móveis (DAM)
Student(s): Rui Ferreira (a51597)
Date: March 6th, 2026
Repository URL: https://github.com/RuiFerreira05/DAM-HelloWorld.git
---
## 1. Introduction
The objective of this assignment is to develop an introductory Android application named "Hello World," which serves as the first step towards mobile application development in Kotlin. This project fulfills the requirements of Tutorial 1, emphasizing basic UI construction, resource management, and application lifecycle monitoring.

## 2. System Overview
The HelloWorld app is a straightforward application consisting of a single screen (Activity). It demonstrates the use of standard Android UI elements such as `TextView`, `ImageView`, and `CalendarView`. It supports multiple configurations including portrait and landscape modes, as well as light and dark themes. 

## 3. Architecture and Design
The project follows the standard Android application architecture:
- **`MainActivity.kt`**: The single activity that manages the lifecycle and user interface.
- **`res/layout/activity_main.xml`**: The user interface definition constructed using `ConstraintLayout`. A landscape variant (`layout-land`) is also included.
- **`res/values/strings.xml`**: All string texts are extracted here to support internationalization and dynamic string formatting.

## 4. Implementation
The main implementation centers around UI design and logging:
- **UI Elements**: Configured a `ConstraintLayout` housing a title (`TextView`), a subtitle, an `ImageView` with a smile asset, and a `CalendarView`. 
- **Dynamic Strings and Logging**: The `MainActivity`'s `onCreate` method contains a logging statement `println(getString(R.string.activity_oncreate_msg, this@MainActivity.localClassName))` that formats a string dynamically to monitor the application state via Logcat.

## 5. Testing and Validation
The application was deployed and validated on an Android Virtual Device (AVD - Pixel 9 Pro and Pixel Tablet) to ensure that:
- The `ConstraintLayout` adapts correctly to different screen sizes.
- The UI properly adjusts when rotated to landscape mode.
- Dark mode rendering behaves correctly.
- The `onCreate` method accurately logs the dynamic string directly into Logcat.

## 6. Usage Instructions
1. Clone the repository: `git clone https://github.com/RuiFerreira05/DAM-HelloWorld.git`
2. Open the project in Android Studio (Panda 1 or newer recommended).
3. Wait for Gradle sync to complete.
4. Select an Android Virtual Device (AVD) or a physical device connected via ADB.
5. Click **Run** (`Shift + F10`) to launch the application.
6. Open the **Logcat** tab in Android Studio to observe the lifecycle log messages.

---
# Development Process
## 12. Version Control and Commit History
Version control using Git was employed from the very beginning. The commit history shows incremental feature additions:
- Initial project structure and "Hello World V1" setup.
- UI enhancements for "Hello World V2 Portrait".
- Creation of layout variants like landscape mode.
- Adjustments to dark mode rendering.
- Implementation of dynamic strings and logging.

## 13. Difficulties and Lessons Learned
- **ConstraintLayout Setup**: Learning how to properly anchor views to prevent overlaps.
- **Resource Extraction**: Understanding the importance of `strings.xml` for localization and dynamic formatting.

## 14. Future Improvements
- Add interactive buttons to change the image dynamically.
- Implement language localization for Portuguese and other languages.
---
## 15. AI Usage Disclosure (Mandatory)
No AI tools were explicitly used to generate code for this specific module as it corresponds to the "[AC NO, AI NO]" restrictions imposed by the assignment guidelines.
