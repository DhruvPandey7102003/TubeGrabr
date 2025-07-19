# TubeGrabr

A simple, modern web application to download YouTube videos by URL. This project consists of a React frontend and a Node.js/Express backend, leveraging yt-dlp for video processing.

⚠️ IMPORTANT LEGAL DISCLAIMER ⚠️
This tool is provided for educational and personal use only. Downloading copyrighted material from YouTube without explicit permission from the copyright holder may violate YouTube's Terms of Service and copyright laws. Users are solely responsible for ensuring their use complies with all applicable laws and terms. The creator of this software is not responsible for any misuse.

✨ Features
User-Friendly Interface: Clean and intuitive design for pasting YouTube video URLs.

Real-time Feedback: Provides status updates (processing, success, error) during the download process.

Robust Backend: Utilizes the actively maintained yt-dlp command-line tool for reliable video extraction.

Direct Download: Initiates a direct file download in the browser upon successful processing.

Responsive Design: Adapts seamlessly to various screen sizes (mobile, tablet, desktop).

Animated Background: Engaging visual effects for a modern look.

🚀 Technologies Used
Frontend
React: JavaScript library for building dynamic user interfaces.

Tailwind CSS: A utility-first CSS framework for rapid and responsive styling.

HTML/CSS/JavaScript: Standard web technologies.

Backend
Node.js: JavaScript runtime environment.

Express.js: Fast, minimalist web framework for Node.js.

youtube-dl-exec (npm package): A convenient Node.js wrapper for the yt-dlp command-line tool.

yt-dlp (Command-Line Tool): The core program responsible for downloading videos from YouTube and other sites.

cors: Node.js middleware to enable Cross-Origin Resource Sharing.

child_process (Node.js built-in): Used to spawn and manage the yt-dlp process.

📋 Prerequisites
Before you can run this project, ensure you have the following installed on your system:

Node.js and npm (or Yarn): Download and install the latest LTS version from nodejs.org.

yt-dlp (Command-Line Tool): This is critical for the backend to function. Download the yt-dlp.exe file from its official GitHub releases page (https://github.com/yt-dlp/yt-dlp/releases) and ensure it's placed in your system's PATH environment variable.

📦 Project Structure
Your project should be organized into two main, separate directories:

Tube Grabr/
├── youtube-downloader-frontend/
│   ├── public/
│   │   └── index.html
│   ├── src/
│   │   ├── App.js
│   │   ├── index.css
│   │   └── index.js
│   ├── package.json
│   ├── package-lock.json
│   ├── tailwind.config.js
│   └── postcss.config.js
└── youtube-downloader-backend/
    ├── node_modules/
    ├── package.json
    ├── package-lock.json
    └── server.js

⚙️ Setup and Running the Project
To set up and run this project, you will need to configure both the backend and frontend components separately. This involves creating the necessary directories, installing dependencies, and populating files with the provided code. Detailed steps for each component (Backend and Frontend) are available in the project's setup guide or documentation.

7. Running the Application
To run the full application, you need to start both the backend and the frontend servers in separate Command Prompt windows. Once both are running, open your web browser and navigate to the frontend URL (typically http://localhost:3000).

8. Usage
Paste a YouTube video URL into the input field on the website.

Click the "Download" button.

A new browser tab will open, and the video download should automatically begin. Check your browser's download bar or your default downloads folder.

9. Troubleshooting Common Issues
Common issues include problems with module recognition (missing scripts, unresolved modules) in the frontend, or internal server errors in the backend. These are typically resolved by ensuring correct file placement, proper dependency installation, and up-to-date yt-dlp and Node.js packages. Refer to detailed troubleshooting steps in the project's full documentation.

10. Future Improvements
Download Options: Implement frontend options for video quality (e.g., 720p, 1080p) or format (MP4, MP3).

Progress Bar: Display download progress on the frontend.

Error Handling: More user-friendly error messages on the frontend for specific backend failures.

Backend File Storage: Implement temporary file storage on the backend before serving, for more complex download scenarios or if direct streaming becomes problematic.

Deployment: Explore deploying the application to a cloud platform (e.g., Netlify/Vercel for frontend, Render/Google Cloud Run for backend).
