# TaskMaster - Multi-Language Task Manager

TaskMaster is a web application designed to manage tasks, demonstrating the integration of multiple programming languages in a modern web development environment. It leverages Python for the backend API, Java for business logic, TypeScript for data models, and JavaScript for UI interactions.

## Features

-   **Task Creation:** Users can add new tasks with titles, descriptions, and priority levels (low, medium, high).
-   **Task Listing:** Displays a list of tasks with titles, descriptions, priority tags, and creation dates.
-   **Task Filtering:** Allows users to filter tasks by priority (all, high, medium, low).
-   **Task Deletion:** Users can delete tasks.
-   **Multi-Language Architecture:**
    -   **Python:** Handles the backend API using Pyodide, running Python code in the browser.
    -   **Java:** Processes business logic using a simulated Java `TaskService`.
    -   **TypeScript:** Defines type-safe data models (simulated in JavaScript with comments indicating TypeScript types).
    -   **JavaScript:** Controls the user interface and orchestrates interactions between different language components.
-   **Asynchronous Operations:** Uses `async/await` for handling asynchronous operations, such as fetching and manipulating tasks.
-   **Modular Design:** Demonstrates a modular architecture with clear separation of concerns between the UI controller, business logic service, and backend API.
-   **Debug Console:** Provides an on-screen debug console to log messages from different language components, aiding in development and troubleshooting.
-   **Toast Notifications:** Displays user-friendly toast notifications for successful actions and errors.
-   **Loading Indicator:** Shows a loading indicator while the application initializes, specifically during the Pyodide loading process.

## Technologies Used

-   HTML
-   CSS
-   JavaScript
-   Pyodide (for running Python in the browser)
-   lodash.js (for utility functions)

## Getting Started

Since this is a purely front-end application with simulated backend components, there are no complex installation steps.

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/husal90/taskmaster.git](https://github.com/husal90/taskmaster.git)
    cd taskmaster
    ```
2.  **Open `index.html` in your browser:** You can simply double-click the `index.html` file or serve it via a local web server.

## How to Use

1.  **Add a Task:**
    -   Enter the task title in the "Task Title" input field.
    -   Enter the task description in the "Description" textarea.
    -   Select the task priority from the "Priority" dropdown (Low, Medium, or High).
    -   Click the "Add Task" button.
2.  **View Tasks:**
    -   Tasks are displayed in the "Your Tasks" section.
    -   Each task shows the title, description, priority (with a colored tag), and creation date.
3.  **Filter Tasks:**
    -   Click on the priority filter buttons ("All", "High Priority", "Medium Priority", "Low Priority") to filter the tasks displayed.
4.  **Delete a Task:**
    -   Click the "✕" button next to the task you want to delete.

## Architecture

The application is structured into the following components:

-   **TaskService (simulated Java):** Handles task creation and validation.
-   **Python Backend (using Pyodide):** Manages task data (add, get, delete, filter) via a simulated API.
-   **TaskController (simulated TypeScript):** Manages the UI, interacts with the `TaskService` and Python backend, and handles user events.
-   **UI (HTML, CSS, JavaScript):** Provides the user interface for interacting with tasks.

## Notes

-   This application uses **simulated** Java and TypeScript functionalities within JavaScript for demonstration purposes.  It showcases the *concept* of multi-language integration in a simplified environment.
-   The Python backend runs in the browser using Pyodide, which may have performance considerations for more complex applications.
-   The application does not persist data across browser sessions.

## Author

[husal90](https://github.com/husal90/)

## License

This project is licensed under the [MIT License](LICENSE).
