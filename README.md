🌐 Frontend UI for Server Management

This document describes the Frontend User Interface (UI) for the Server Management Application.
The interface is designed to be modern, responsive, and user-friendly, allowing users to easily manage server data with style and simplicity. 💻✨

🚀 Key Features

🧭 Single-Page Application (SPA):
Built entirely with React, the UI runs smoothly on a single page without reloads.

⚙️ Full CRUD Operations:
Users can view, add, and delete servers through a clean interactive dashboard.

🌗 Light & Dark Mode:
A built-in theme toggle lets users switch between light and dark themes.
The choice is remembered using the browser’s localStorage.

🎨 Modern Aesthetic:
Sleek design, minimal layout, and the Roboto font ensure a professional, readable interface.

🧩 Technologies Used
Technology	Purpose
🧱 HTML5	Defines the structure of the UI
🎨 CSS3	Handles styling, animations, and theme variables
⚛️ React (via CDN)	Core library for UI components and state management
🧪 Babel (via CDN)	Transpiles JSX directly in the browser
🔤 Google Fonts (Roboto)	Enhances typography and readability
🛠️ How the UI Was Built

The frontend is designed as a self-contained React app within a single index.html file (found in the frontend/ directory).

Here’s a breakdown of how it’s structured and works:

🚀 React via CDN
Instead of a full build system, React and Babel are loaded directly from CDNs using <script> tags.
This makes setup lightweight and ideal for demonstration projects.

⚛️ React Component (App)
The application’s logic resides in a single component named App.
It manages:

Server data state

User input for adding servers

Re-rendering the interface when data updates occur

🎨 Styling and Theming

Font: Uses the Roboto font for a modern look.

Light/Dark Mode: Implemented with CSS variables.

Persistence: The user’s theme choice is saved in localStorage, so it’s remembered even after a page reload.

🔗 Communication with Backend

The frontend interacts with the backend REST API using the browser’s built-in fetch() method.

Action	HTTP Method	Endpoint	Description
📥 Fetch Servers	GET	/servers/getServer	Retrieves the list of all servers
➕ Add Server	PUT	/servers/createServer	Adds a new server record
❌ Delete Server	DELETE	/servers/deleteServer	Deletes a server by its ID

All requests and responses are in JSON format.

🧑‍💻 How to Use the Frontend

Follow these quick steps to get the UI running:

🏁 Ensure Backend is Running
Start your Spring Boot backend (Task 1) on port 8080.

🌍 Open the Frontend
Navigate to your project’s frontend/ directory and open index.html in any modern web browser (Chrome, Edge, Firefox, etc).

🎮 Start Managing Servers

View all available servers

Add new servers with the form

Delete any server instantly

Toggle between light and dark mode 🌗