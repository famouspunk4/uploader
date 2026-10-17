# YouTube Studio Uploader

A lightweight, self-hosted, browser-based tool to batch-convert MP3 audio files and a static cover image into video blobs, streaming them directly to your YouTube account via the Resumable Upload protocol.

---

## Features
- **Client-Side Encoding:** Renders MP3s and cover art directly in the browser using the Web Audio API and `MediaRecorder`.
- **Direct YouTube Integration:** Sign in with Google Identity Services (OAuth 2.0) and upload videos straight to YouTube using resumable data streams.
- **Queue Manager & Reordering:** Drag-and-drop file support, track reordering, and customizable metadata fields.

---

## Getting Started

Follow these steps to run the uploader locally on your machine:

1. **Download the Application File**
   * Download the [`index.html`](index.html) file and save it on your computer.

2. **Organize Your Files**
   * Create a dedicated folder in your file explorer (e.g., named `youtube-uploader`) and place `index.html` inside it.

3. **Start the Local Web Server**
   * Open your terminal or Command Prompt, navigate into your project folder, and run:
     ```bash
     python -m http.server 8000
     ```

4. **Launch the App**
   * Open your browser and navigate to:
     [http://localhost:8000](http://localhost:8000/)

---

## Configuration

1. Click the **API Setup** (gear icon) in the app header.
2. Enter your Google OAuth Client ID (saved securely in your browser's local storage).
3. Ensure `http://localhost:8000` is added under **Authorized JavaScript origins** in your Google Cloud Console credentials.
