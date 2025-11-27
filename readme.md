# 🧠 AI Thinking

**AI Thinking** is a robust, client-side chat application that bridges the gap between raw AI capabilities and structured human workflow. Powered by **Google Gemini 2.5 Flash** and **Firebase**, it offers a seamless interface for interacting with text, images, and documents.

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Status](https://img.shields.io/badge/status-Active-green.svg)

[**Live Demo**](#) | [**Report Bug**](https://github.com/yourusername/ai-thinking/issues) | [**Request Feature**](https://github.com/yourusername/ai-thinking/issues)

---

## ✨ Key Features

### 🤖 Multimodal Capabilities
* **Text:** Natural language conversations with deep context awareness.
* **Images:** Vision capabilities allow you to upload images for instant analysis.
* **Documents:** Analyze PDFs and text files directly within the chat interface.
* **Code:** Built-in syntax highlighting for code blocks using `highlight.js`.

### 🔐 Flexible Authentication
* **Guest Mode:** Start chatting immediately without login (chats saved to `LocalStorage`).
* **Google Login:** Sync conversations across devices using Firebase Authentication.

### 🎨 Modern UI/UX
* **Responsive Design:** Fully optimized for mobile and desktop using **Tailwind CSS**.
* **Dark/Light Mode:** System-aware theme toggle with preference persistence.
* **Markdown Support:** Rich text rendering powered by `marked.js`.
* **Smart Previews:** Visual previews for uploaded images and distinct icons for file attachments.

### 💾 Smart History
* **Persistence:** Chats are automatically saved to **Firestore** (for logged-in users) or **LocalStorage** (for guests).
* **Data Optimization:** Large file attachments are handled efficiently to respect storage limits.

---

## 🛠️ Tech Stack

* **Frontend Engine:** HTML5, Vanilla JavaScript (ES Modules)
* **Styling:** Tailwind CSS (via CDN)
* **AI Model:** Google Gemini API (`gemini-2.5-flash-preview-09-2025`)
* **Backend / BaaS:**
    * Firebase Auth (Google Sign-In)
    * Firebase Firestore (Database)
    * Firebase Analytics
* **Utilities:**
    * `marked.js` (Markdown parsing)
    * `highlight.js` (Code syntax highlighting)

---

## 🚀 Getting Started

Since this is a client-side application using ES Modules and CDNs, **no build step** (like Webpack or Vite) is strictly required to run it locally.

### Prerequisites
* A modern web browser (Chrome, Firefox, Edge, Safari).
* A local web server (required due to CORS policies with ES modules).

### Installation

1.  **Clone the repository**
    ```bash
    git clone [https://github.com/yourusername/ai-thinking.git](https://github.com/yourusername/ai-thinking.git)
    cd ai-thinking
    ```

2.  **Configuration**
    Open `index.html` in your code editor. You need to configure your API keys.

    * **Step A: Gemini API**
        Find the `API_KEY` constant and replace it with your key from [Google AI Studio](https://aistudio.google.com/).
        ```javascript
        const API_KEY = "YOUR_GEMINI_API_KEY_HERE";
        ```

    * **Step B: Firebase Config**
        Find the `firebaseConfig` object and replace it with your project details from the [Firebase Console](https://console.firebase.google.com/).
        ```javascript
        const firebaseConfig = {
            apiKey: "YOUR_FIREBASE_API_KEY",
            authDomain: "your-project.firebaseapp.com",
            projectId: "your-project-id",
            // ... other config values
        };
        ```

3.  **Run Locally**
    > **Note:** You cannot simply double-click `index.html` because of ES Module security restrictions (CORS). You must serve it.

    **Using Python:**
    ```bash
    python3 -m http.server 8000
    ```

    **Using Node (http-server):**
    ```bash
    npx http-server .
    ```

    **Using VS Code:**
    Install the "Live Server" extension and click "Go Live" in the status bar.

4.  **Access the App**
    Open your browser to `http://localhost:8000` (or the port provided by your server).

---

## 📖 Usage Guide

1.  **Start a Chat:** Type your query in the input box at the bottom.
2.  **Attach Files:** Click the **+** icon to upload images, PDFs, or code files for analysis.
3.  **Switch Modes:** Use the Moon/Sun icon in the header to toggle between Dark and Light modes.
4.  **Manage History:** Click the Sidebar icon (top left) to view past conversations or delete them.
5.  **Login:** Click the "Login" button to switch from Guest storage to Cloud storage.

---

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.

---

## 📞 Contact

Project Link: [https://github.com/yourusername/ai-thinking](https://github.com/yourusername/ai-thinking)
