# Todo Application

A clean, responsive Todo application built with semantic HTML5, Tailwind CSS, and vanilla JavaScript.

The application allows users to create tasks, mark tasks as completed, delete tasks, and retain their task list across browser refreshes using `localStorage`.

## Features

- Add new todo tasks.
- Mark tasks as completed or active.
- Visually strike through completed tasks.
- Delete tasks from the list.
- Persist tasks using browser `localStorage`.
- Display the number of remaining tasks.
- Responsive layout for mobile, tablet, and desktop screens.
- Modern dark mode aesthetic using slate, zinc, and indigo colors.
- Semantic HTML5 structure with accessible labels and live regions.
- No build tools, frameworks, or dependencies required.

## Project Structure

```text
.
├── index.html
└── README.md
```

## Running the Application

### Option 1: Open Directly in a Browser

1. Download or clone the project.
2. Open the project directory.
3. Double-click `index.html`.

The application will run directly in your browser.

### Option 2: Use a Local Development Server

If you have Python installed, run the following command from the project directory:

```bash
python -m http.server 8000
```

Then open the following address in your browser:

```text
http://localhost:8000
```

## How It Works

Tasks are stored as JavaScript objects containing:

- A unique task ID.
- The task text.
- A completion status.

Whenever a task is added, completed, or deleted, the updated task list is serialized with `JSON.stringify()` and saved to `localStorage`.

When the page loads, the application reads the stored data with `localStorage.getItem()` and renders the saved tasks.

## Technologies Used

- HTML5
- Tailwind CSS via CDN
- Vanilla JavaScript
- Browser `localStorage` API

## GitHub Copilot Usage

GitHub Copilot was used as an AI-assisted development tool during the creation of this project.

Copilot helped with:

- Structuring the semantic HTML5 layout.
- Creating the responsive Tailwind CSS styling.
- Implementing task creation, completion toggling, and deletion logic.
- Adding `localStorage` persistence.
- Improving accessibility with labels, buttons, focus styles, and live regions.
- Reviewing the code for readability and maintainability.
- Drafting and organizing this project documentation.

The final implementation was reviewed and adjusted to ensure that the code meets the application's functional, responsive, and accessibility requirements.

## Browser Compatibility

The application uses modern browser APIs, including:

- `localStorage`
- `crypto.randomUUID()`, with a fallback for browsers that do not support it
- Standard DOM APIs

It should work in current versions of Chrome, Firefox, Safari, and Microsoft Edge.

## License

This project is available for personal and educational use.
