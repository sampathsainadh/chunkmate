Chunkmate is a full-stack web application built to intelligently split Markdown documents into smaller, context-preserving pieces. It's optimized for AI-related workflows or enhanced document readability. It includes a modern React-based UI and a fast Node.js/Express backend API.

INDEX
Features

Folder Layout

Technology Stack

Getting Started

How to Use

Debugging

Tweaks & Extensions

Licensing

Frontend Guide

Backend Guide

✨ Features
Upload .md (Markdown) files with ease.

Automated segmentation of content by headings and formatting rules.

Interactive viewing of document chunks with structured heading context.

Document navigator to switch between uploaded files.

Clean, responsive interface with intuitive controls.

Graceful error handling and helpful UI feedback.

📁 Folder Layout
css
Copy
Edit
docchunker/
├── server/
│   ├── routes/
│   │   └── files.js
│   ├── logic/
│   │   └── chunkProcessor.js
│   └── ...additional server files
├── client/
│   ├── src/
│   │   ├── components/
│   │   │   ├── ChunkDisplay.jsx
│   │   │   ├── FileSelector.jsx
│   │   │   └── FileUploader.jsx
│   │   ├── App.jsx
│   │   └── styles/
│   └── ...other client files
└── README.md
⚙️ Technology Stack
Frontend:

React

Tailwind CSS (alternative to styled-components)

react-markdown

Vite

Backend:

Node.js

Express.js

🚀 Getting Started
📌 Requirements
Node.js v16+

npm or yarn

🔧 Setup Instructions
Clone the repository

bash
Copy
Edit
git clone https://github.com/yourusername/docchunker.git
cd docchunker
Backend Setup

bash
Copy
Edit
cd server
npm install
Frontend Setup

bash
Copy
Edit
cd ../client
npm install
▶️ Running the Application
1. Start the API server
bash
Copy
Edit
cd server
npm start
Server runs on: http://localhost:3001

2. Launch the frontend
bash
Copy
Edit
cd ../client
npm run dev
Frontend runs on: http://localhost:5173

🧪 How to Use
Drag and drop a .md file or use the file picker to upload.

Choose a file from the sidebar to inspect its chunks.

Each segment includes repeated headings for better clarity.

Switch between files and view chunks in a readable format.

🛠 Debugging
Common Issues:
Blank screen or JavaScript error:

Confirm both servers are running.

Check DevTools for any stack traces.

API errors or fetch failures:

Make sure the backend is accessible at http://localhost:3001.

Chunking doesn’t work as expected:

Headings (#, ##, etc.) are required in your markdown files.

Review chunkProcessor.js to customize how segmentation is done.

🎨 Tweaks & Extensions
Styling
Update Tailwind or custom CSS classes inside components (e.g., ChunkDisplay.jsx) to reflect your desired look and feel.

Content Parsing Logic
Modify the logic in chunkProcessor.js to change how the documents are analyzed and split.

Backend Endpoints
View and edit routes in files.js to add features like delete, search, or pagination.

📘 Frontend Guide
See client/README.md for component details, styling tips, and markdown rendering strategies.

🖥 Backend Guide
See server/README.md for API structure, parsing logic, and database integration options.

🪪 License
This project is open source and available under the MIT License.
