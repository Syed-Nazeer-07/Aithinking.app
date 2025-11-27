AI Thinking

AI Thinking is a robust, client-side chat application that bridges the gap between raw AI capabilities and structured human workflow. Powered by Google Gemini 2.5 Flash and Firebase, it offers a seamless interface for chatting with text, images, and documents.

Live Demo / Preview: Simply open index.html in your browser.

✨ Key Features

Multimodal Capabilities:

Text: Natural language conversations with context awareness.

Images: Upload images for analysis (vision capabilities).

Documents: Analyze PDFs and text files directly in the chat.

Code: Syntax highlighting for code blocks using highlight.js.

Flexible Authentication:

Guest Mode: Start chatting immediately without login (chats saved to LocalStorage).

Google Login: Sync chats across devices using Firebase Authentication.

Modern UI/UX:

Responsive Design: Fully optimized for mobile and desktop (Tailwind CSS).

Dark/Light Mode: System-aware theme toggle with persistence.

Markdown Support: Rich text rendering using marked.js.

File Previews: Visual previews for uploaded images and file icons for documents.

Smart History:

Persistence: Chats are automatically saved to Firestore (for logged-in users) or LocalStorage (for guests).

Data Optimization: Large file attachments are handled efficiently to respect storage limits.

🛠️ Tech Stack

Frontend Engine: HTML5, Vanilla JavaScript (ES Modules).

Styling: Tailwind CSS (via CDN).

AI Model: Google Gemini API (gemini-2.5-flash-preview-09-2025).

Backend / BaaS:

Firebase Auth (Google Sign-In).

Firebase Firestore (Database).

Firebase Analytics.

Utilities:

marked.js (Markdown parsing).

highlight.js (Code syntax highlighting).

🚀 Getting Started

Since this is a client-side application using ES Modules and CDNs, no build step (like Webpack or Vite) is strictly required to run it locally.

Prerequisites

A modern web browser (Chrome, Firefox, Edge, Safari).

A local web server (recommended due to CORS policies with ES modules).

Installation & Setup

Clone the repository

git clone [https://github.com/yourusername/ai-thinking.git](https://github.com/yourusername/ai-thinking.git)
cd ai-thinking


Configuration
Open index.html and locate the configuration sections to add your own keys.

Step A: Gemini API
Find the API_KEY constant and replace it with your key from Google AI Studio.

const API_KEY = "YOUR_GEMINI_API_KEY_HERE";


Step B: Firebase Config
Find the firebaseConfig object and replace it with your project details from the Firebase Console.

const firebaseConfig = {
    apiKey: "YOUR_FIREBASE_API_KEY",
    authDomain: "your-project.firebaseapp.com",
    projectId: "your-project-id",
    // ... other config values
};


Run Locally
You cannot simply double-click index.html because of ES Module security restrictions (CORS). You must serve it.

Using Python:

python3 -m http.server 8000


Using Node (http-server):

npx http-server .


Using VS Code:
Install the "Live Server" extension and click "Go Live".

Access the App
Open your browser to http://localhost:8000 (or the port provided by your server).

📖 Usage Guide

Start a Chat: Type your query in the input box.

Attach Files: Click the + icon to upload images, PDFs, or code files.

Switch Modes: Use the Moon/Sun icon in the header to toggle Dark Mode.

Manage History: Click the Sidebar icon (top left) to view or delete past conversations.

Login: Click the "Login" button (if configured) to save your chats to the cloud.

📄 License

Distributed under the MIT License. See LICENSE for more information.

📞 Contact

Project Link:https://github.com/Syed-Nazeer-07/Aithinking.app
