<img width="1782" height="892" alt="Screenshot (17)" src="https://github.com/user-attachments/assets/ee1fbfc4-3271-462c-8c11-8918ef2a3fc5" />Here’s a professional and well-structured `README.md` file for your GitHub repository based on the project details you provided:

---

# AI-Powered Mock Interview Platform



An AI-powered platform that simulates realistic technical interviews, providing personalized questions, live coding challenges, voice-based Q&A, and detailed feedback.

---

## Table of Contents

1. [Features](#features)
2. [Technologies Used](#technologies-used)
3. [Installation](#installation)
4. [Usage](#usage)
5. [Project Structure](#project-structure)


---

## Features

- **Resume Upload and Analysis**: Personalized interview questions generated from your uploaded resume.
- **Voice-Based Interviews**: AI interviewer powered by Murf AI to simulate real-world interviews.
- **Live Coding Challenges**: Built-in Monaco code editor for solving coding problems in real-time.
- **Detailed Feedback**: AI evaluates your performance across 5 categories and provides actionable insights.
- **Interview History**: Track all past interviews with scores, feedback, and improvement metrics.
- **Multi-Role Support**: Practice for roles like Frontend, Backend, Full Stack, Data Analyst, DevOps, and more.

---

## Technologies Used

### Backend
- **Node.js** & **Express**: Server-side framework.
- **MongoDB**: Database for storing user data, resumes, and interview history.
- **Google Gemini API**: For generating personalized questions and feedback.
- **AssemblyAI**: Speech-to-text transcription for voice answers.
- **Murf AI**: Text-to-speech for the AI interviewer's voice.

### Frontend
- **React**: Frontend framework for building the user interface.
- **Axios**: For API communication between frontend and backend.
- **Monaco Editor**: Code editor for live coding challenges.
- **Web Speech API**: Optional real-time transcription during interviews.

### Other Tools
- **PDF.js**: For parsing uploaded PDF resumes.
- **Multer**: Middleware for handling file uploads.
- **Bcrypt** & **JWT**: For secure authentication.

---

## Installation

### Prerequisites
- Node.js (v16 or higher)
- MongoDB Atlas account
- API Keys: Google Gemini, Murf AI, AssemblyAI

### Backend Setup
1. Navigate to the `server/` directory:
   ```bash
   cd server
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Create a `.env` file based on `.env.example` and add your API keys:
   ```env
   MONGODB_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret_key
   GEMINI_API_KEY=your_gemini_api_key
   ASSEMBLYAI_API_KEY=your_assemblyai_api_key
   MURF_API_KEY=your_murf_api_key
   ```

### Frontend Setup
1. Navigate to the `client/` directory:
   ```bash
   cd client
   ```
2. Install dependencies:
   ```bash
   npm install
   ```

### Start the Application
1. Start the backend server:
   ```bash
   npm start
   ```
2. Start the frontend development server:
   ```bash
   npm start
   ```

---

## Usage

1. **Upload Your Resume**: Provide your resume in PDF format to generate personalized interview questions.
2. **Start an Interview**: Choose your role (e.g., Frontend Developer) and difficulty level.
3. **Answer Questions**: Respond to voice-based questions or solve coding challenges in the built-in editor.
4. **Get Feedback**: After the interview, view detailed feedback with scores across multiple categories.
5. **Track Progress**: Use the dashboard to review your interview history and track improvement over time.

---

## Project Structure

```
AI-Mock-Interview-Platform/
├── README.md
├── server/
│   ├── src/
│   │   ├── config/          # Configuration files (e.g., Gemini AI setup)
│   │   ├── constants/       # Prompt templates and constants
│   │   ├── controllers/     # API controllers
│   │   ├── models/          # MongoDB schemas
│   │   ├── routes/          # API routes
│   │   ├── services/        # Business logic (e.g., AI interactions)
│   │   └── utils/           # Utility functions
│   ├── package.json
│   ├── .env.example         # Example environment variables
│   └── .gitignore
├── client/
│   ├── src/
│   │   ├── components/      # Reusable UI components
│   │   ├── pages/           # React pages (e.g., HomePage, InterviewPage)
│   │   ├── services/        # Frontend API service layer
│   │   ├── App.jsx          # Main application component
│   │   └── index.js         # Entry point
│   ├── package.json
│   └── .gitignore
├── .gitignore
└── LICENSE
```

---

