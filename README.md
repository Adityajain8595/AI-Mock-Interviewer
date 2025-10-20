<h1 align="center">AI MOCK INTERVIEWER</h1>
<p align="center"><em>Your AI-powered companion for mastering job interviews</em></p>

<p align="center">
  <a href="https://reactjs.org/"><img src="https://img.shields.io/badge/React-19.1-blue.svg" alt="React"></a>
  <a href="https://fastapi.tiangolo.com/"><img src="https://img.shields.io/badge/FastAPI-Latest-009688.svg" alt="FastAPI"></a>
  <a href="https://python.langchain.com/"><img src="https://img.shields.io/badge/LangChain-Latest-2496ED.svg" alt="LangChain"></a>
</p>

---

## 📍 Overview

**AI Mock Interviewer** is a cutting-edge platform that revolutionizes interview preparation through AI-powered simulations. The platform combines **resume analysis, personalized questions, voice interactions, and real-time feedback** to create a comprehensive interview preparation experience.

By leveraging advanced AI technologies, it helps candidates:
- Practice interviews in a realistic, pressure-free environment
- Receive instant, objective feedback on responses
- Improve communication and interview skills
- Build confidence through repeated practice

**[Live Demo](https://career-sarthi-nine.vercel.app/mock-interview)** @ CareerSarthi platform we built for GenAI Exchange Hackathon 2025

---

## 👾 Features

- **Resume Analysis**: Automatically analyzes uploaded resumes to personalize interview questions
- **Job Context Adaptation**: Tailors interview questions based on the target job role and description
- **Voice Interaction**: Natural voice-based interaction with text-to-speech capabilities
- **Real-time Feedback**: Provides immediate feedback on interview responses
- **Session Management**: Maintains interview context and history for progressive improvement
- **Modern UI**: Sleek, responsive interface built with React and Tailwind CSS

## 🏗 Architecture

The system is divided into modular **frontend and backend services**:

- **Frontend Stack**:
  - React 19.1 with Vite for fast development
  - Tailwind CSS with Typography plugin
  - Framer Motion for smooth animations
  - Axios for API communication
  - React Markdown for text formatting

- **Backend Stack**:
  - FastAPI for high-performance API
  - LangChain & LangChain Community for AI integration
  - Google Cloud AI Platform for AI services
  - Google Cloud Text-to-Speech for voice synthesis
  - PyMuPDF for PDF parsing
  - Python-dotenv for environment management

- **Key Components**:
  - `app.py` → FastAPI application server
  - `interview.py` → Core interview logic
  - `talk.py` → Text-to-speech integration
  - `resume_parser.py` → Resume analysis engine
  - `prompts.py` → Interview templates
  - `session_store.py` → State management

The architecture ensures **scalability** and **maintainability** through:
- Microservices architecture
- Cloud-ready deployment
- Stateless API design
- Modular component structure

---

## 🚀 Getting Started

### ☑️ Prerequisites

Ensure your system has:

- **Python** 3.8 or higher
- **Node.js** 16.x or higher
- **Google Cloud Platform** account
- **Git** for version control

### ⚙️ Installation

1. Clone the repository:
```sh
❯ git clone <repository-url>
❯ cd AI-Mock-Interviewer
```

2. Set up backend:
```sh
❯ cd backend
❯ python -m venv venv
❯ venv\Scripts\activate  # On Windows
❯ pip install -r requirements.txt
```

3. Configure environment:
```sh
❯ # Create .env file with:
GOOGLE_CLOUD_PROJECT=your_project_id
GOOGLE_APPLICATION_CREDENTIALS=path_to_credentials.json
LANGCHAIN_API_KEY=your_langchain_api_key
```

4. Set up frontend:
```sh
❯ cd ../frontend
❯ npm install

# Required dependencies:
# - React & React DOM v19.1
# - Framer Motion for animations
# - Tailwind CSS for styling
# - Axios for API requests
# - React Markdown for text formatting
```

### 🎯 Running the Application

1. Start backend server:
```sh
❯ cd backend
❯ uvicorn app:app --reload
```

2. Launch frontend:
```sh
❯ cd frontend
❯ npm run dev
```

Access the application at:
- Frontend: `http://localhost:5173`
- Backend API: `http://localhost:8000`

### 💻 Usage Guide

1. **Upload Resume**
   - Support for PDF format
   - Automatic skill and experience extraction

2. **Configure Interview**
   - Select job role
   - Provide job description
   - Choose interview duration

3. **Start Interview**
   - Real-time voice interaction
   - Natural conversation flow
   - Immediate feedback on responses

## 📁 Project Structure

```sh
└── AI-Mock-Interviewer/
    ├── backend/
    │   ├── app.py             # FastAPI application entry point
    │   ├── interview.py       # Core interview logic
    │   ├── prompts.py         # Interview question templates
    │   ├── resume_parser.py   # Resume analysis
    │   ├── session_store.py   # Session management
    │   ├── talk.py           # Text-to-speech integration
    │   └── requirements.txt   # Python dependencies
    └── frontend/
        ├── src/
        │   ├── App.jsx        # Main application component
        │   ├── ChatApp.jsx    # Chat interface component
        │   ├── Interview.jsx  # Interview interface component
        │   ├── assets/        # Static resources
        │   ├── index.css      # Global styles
        │   └── main.jsx       # Application entry point
        ├── public/            # Public static files
        ├── package.json       # Node.js dependencies
        ├── postcss.config.cjs # PostCSS configuration
        ├── tailwind.config.cjs # Tailwind CSS configuration
        └── vite.config.js     # Vite configuration
```

<details closed>
<summary>Contributing Guidelines</summary>

1. **Fork the Repository**: Start by forking the project
2. **Clone Locally**: 
   ```sh
   git clone <repository-url>
   ```
3. **Create a Branch**: 
   ```sh
   git checkout -b feature/amazing-feature
   ```
4. **Make Changes**: Implement your feature or fix
5. **Test**: Ensure your changes work as expected
6. **Submit PR**: Push changes and create a Pull Request

</details>

---

## 🙌 Acknowledgments

Special thanks to:

- **Google Cloud Platform** for AI and TTS services
- **LangChain** for AI integration support

---

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

