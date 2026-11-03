# Taskflow – To-Do List

A clean, responsive, and lightweight task management application built using **HTML, CSS, and Vanilla JavaScript**. Taskflow helps users organize daily activities, track their progress, and manage completed and pending tasks through a simple interface.

## Features

- **Add Tasks:** Create new tasks using the Add Task button or Enter key.
- **Complete Tasks:** Mark tasks as completed or switch them back to active.
- **Delete Tasks:** Remove individual tasks from the list.
- **Task Filtering:** View All, Active, or Done tasks.
- **Clear Completed:** Remove all completed tasks with one action.
- **Task Counter:** Displays the number of remaining tasks.
- **Task Statistics:** Shows total, active, and completed task counts.
- **Local Storage:** Automatically saves tasks in the browser.
- **Data Validation:** Handles invalid or corrupted stored data safely.
- **Responsive Design:** Adapts to different screen sizes.
- **Keyboard Support:** Supports Enter key submission.

## Technologies Used

- **HTML5** – Application structure.
- **CSS3** – Styling, responsive layout, animations, and visual design.
- **JavaScript (Vanilla JS)** – Application logic, DOM manipulation, and event handling.
- **Browser LocalStorage** – Persistent task storage.
- **Google Fonts** – Manrope, DM Mono, and Playfair Display typography.

## Project Structure

```text
intercircle2/
│
├── index.html       # Main HTML entry point
├── styles.css       # External stylesheet
├── app.js           # Task management functionality
└── README.md        # Project documentation
```

## Getting Started

### Prerequisites

- A modern web browser (Chrome, Edge, Firefox, etc.).
- Visual Studio Code (recommended).
- Live Server extension (optional).

### Installation

1. Clone the repository:

   ```bash
   git clone <your-repository-url>
   ```

2. Navigate to the project directory:

   ```bash
   cd intercircle2
   ```

3. Open the project in Visual Studio Code.

4. Run `index.html` using Live Server or open it directly in your browser.

**Note:** No additional dependencies, frameworks, or build tools are required.

## How It Works

1. Enter a task in the input field.
2. Click the **Add Task** button or press Enter.
3. Mark tasks as completed using the circular checkbox.
4. Use the filters to organize tasks.
5. Delete individual tasks whenever needed.
6. Click **Clear Completed** to remove all finished tasks.

## Data Persistence

Taskflow uses browser `localStorage` to save tasks.

- Tasks are stored using the key `taskflow.tasks.v1`.
- `JSON.stringify()` converts the task array into JSON before saving.
- `JSON.parse()` retrieves stored tasks when the application starts.
- A `try/catch` block handles invalid JSON data.
- Data validation ensures that each task has a numeric ID, string text, and boolean completion status.

### Task Data Structure

```javascript
{
  id: 1730000000000,
  text: "Finish project notes",
  done: false
}
```

## Technical Implementation

- Uses JavaScript arrays to maintain task state.
- Uses DOM manipulation to dynamically render tasks.
- Implements event delegation for task completion and deletion.
- Uses `textContent` to display user-entered text safely.
- Uses `replaceChildren()` to refresh the task list.
- Uses `Intl.DateTimeFormat()` to display the current date.
- Implements responsive CSS media queries for mobile devices.

## Future Improvements

- Add task editing functionality.
- Introduce task deadlines and reminders.
- Add priority levels for tasks.
- Implement dark mode.
- Add categories and search functionality.
- Improve accessibility and keyboard navigation.

## Author

**Satyam Kushwaha**

Computer Science & Engineering Student

---

*Taskflow – Organize your tasks, focus on what matters, and make everyday progress.*