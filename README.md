#PulseTask
A fast, modern, zero-dependency browser-based task management application engineered for fluid workflow execution and seamless state persistence.

Overview

PulseTask is a lightweight, responsive productivity web application designed to keep your focus intact. Built entirely with vanilla JavaScript, modern CSS variables, and HTML5 semantic elements, PulseTask delivers a fluid experience with interactive drag-and-drop ordering, real-time search filtering, dynamic categorization, and native localStorage state management.

Key Features

* Complete CRUD Operations: Create, edit, complete, and delete tasks instantly.
* Category Tagging: Organize tasks into Work, Personal, Study, and Health buckets with distinct color badges.
* Live Search & Filtering: Filter tasks instantly by title via real-time search or switch view modes (All, Active, Completed).
* Native Drag-and-Drop: Intuitive list item reordering using standard browser HTML5 drag-and-drop APIs.
* Persistent Storage: Automatically syncs state changes to localStorage to survive page reloads and browser resets gracefully.
* Micro-Interactions & Animations: Strikethrough transitions, subtle scaling effects on check completion, and entry/exit list animations.
* Zero External Dependencies: Built with pure vanilla technologies for instant load times and lightweight footprint.
🛠️ Architecture & Tech Stack
* Markup: Semantic HTML5 (<header>, <main>, <section>, <form>) with accessibility considerations.
* Styling: CSS3 utilizing CSS Custom Properties (Variables), Flexbox, CSS Grid, and custom keyframe animations.
* Logic: Vanilla JavaScript (ES6+) structured around state-driven UI rendering, XSS sanitization, and event delegation.

Data Model Schema

Each task object stored within the application state follows this schema:
{
"id": "task_1700000000000_abc12",
"title": "Complete project proposal pitch",
"category": "Work",
"dueDate": "2026-11-20",
"completed": false,
"createdAt": 1700000000000,
"order": 0
}

🚀 Getting Started

Since PulseTask requires no node modules, build steps, or external compilers, running it locally is seamless.
Prerequisites
Any modern web browser (Chrome, Firefox, Safari, Edge).
Installation
1. Clone the repository:
git clone https://github.com/maicodon/pulsetask.git

2. Navigate into the directory:
cd pulsetask

3. Open the project:
   
   * Double-click index.html to open it in your default browser, or
   * Use VS Code's Live Server extension for hot-reloading development.
📂 Project Structure
pulsetask/
├── index.html        # Semantic HTML layout and container structure
├── styles.css        # Responsive CSS layout, variables, and animations
├── app.js            # Core state management, CRUD logic, and event handling
└── README.md         # Project documentation and specifications

💡 Usage Guide

   1. Adding a Task: Type the task title into the input field, select a category and optional due date, then press Enter or click Add Task.
   2. Filtering Tasks: Click the Active or Completed tabs to change view modes, or type in the Search input to dynamically filter items by title.
   3. Reordering: Click and drag any task item up or down to reorder the list. The new sequence persists automatically in localStorage.
   4. Completing/Deleting: Click the checkbox to toggle completion status. Use the trash icon button to trigger the removal animation and delete the item.
      
Contributing

Contributions are welcome! If you'd like to improve PulseTask:
   1. Fork the Project.
   2. Create your Feature Branch (git checkout -b feature/AmazingFeature).
   3. Commit your Changes (git commit -m 'Add some AmazingFeature').
   4. Push to the Branch (git checkout -b feature/AmazingFeature).
   5. Open a Pull Request.
