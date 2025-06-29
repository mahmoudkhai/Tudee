# 📱 Personal Task Management App – Android

[![Watch the video](https://img.youtube.com/vi/IJXkHi8KEJk/0.jpg)](https://youtube.com/shorts/IJXkHi8KEJk)


## 📌 Project Overview

A personal task management app for Android, developed collaboratively by the squad. The app stores data locally using **Room Database** and implements **Jetpack Navigation** for seamless user flow. The project emphasizes a clean, justified architecture. Any unnecessary or unjustified complexity may negatively affect the project evaluation.

---

## 🧱 Architecture

- Each screen has its own `ViewModel`.
- `ViewModel`s depend on an abstraction called `TasksService`.
- `TasksService` provides **domain-level entities** and is implemented using:
  - Room **DAOs** for data access.
  - Mapping logic to convert Room models into domain entities.
- A fully-fledged Clean Architecture is not required due to the app's simplicity, but clear **separation of concerns** must be maintained.

---

## 🎨 UI & Design System

- A reusable **design system** must be created and used across the app.
- Avoid hardcoded styles, colors, dimensions, and text appearances.
- The UI must closely match the **Figma design**.
- Responsive layouts must be supported to ensure consistency across different screen sizes and orientations.
- Light and dark modes must be supported, following the system theme.

---

## 🌐 Localization

- The app automatically follows the device’s language settings.
- Must support both **English** and **Arabic**, including proper LTR/RTL layout handling.
- No separate in-app language setting screen is required.

---

## ✅ Features

### 🆕 Onboarding
- Display an onboarding screen **only on the first launch** of the app.

### 🏠 Home Screen
- Display statistics about today’s tasks.

### ✍️ Task Management
- Create a new task with:
  - Title  
  - Description  
  - Priority  
  - Category  
- View full task details.
- View all tasks filtered by a selected date.
- Delete a task.
- Update a task’s status:
  - From "To Do" → "In Progress"
  - From "In Progress" → "Done"

### 🗂️ Category Management
- Display a list of predefined categories.
- Add a new category:
  - With title and image selection from device storage.
- Edit or delete any user-created category.

### 🌗 Theming & Language
- Support for system-controlled light and dark themes.
- Support for both English and Arabic without needing manual language switching.

---

## 🧪 Testing

- Unit tests must be written to achieve at least **70% code coverage**, especially for business logic components.
