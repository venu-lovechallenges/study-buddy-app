# 📚 Study Buddy App

An AI-powered study assistant designed for O/L students in Sri Lanka. Built with React, Node.js/Express, and featuring cute mascot characters to make learning fun!

## ✨ Features

- 🎓 **Grade Selection**: Support for Grade 10, Grade 11, and University levels
- 📚 **O/L Study Packs**: Complete syllabus coverage for all subjects
- 🗣️ **Spoken English**: Interactive units from greetings to conversational fluency
- ✅ **Unit Tests**: Practice tests to assess your progress
- 🤖 **AI Tutor**: Ask questions and get contextual answers based on the syllabus
- 🎨 **Beautiful UI**: Pink-themed interface with Tailwind CSS
- 📱 **Responsive Design**: Works on web, mobile, and desktop

## 🚀 Quick Start

### Prerequisites
- Node.js v14+ 
- npm or yarn

### Installation

**Backend:**
```bash
cd server
npm install
npm start
```
Server runs on `http://localhost:5000`

**Frontend:**
```bash
cd client
npm install
npm start
```
App runs on `http://localhost:3000`

## 📁 Project Structure

```
study-buddy-app/
├── client/                    # React frontend
│   ├── public/
│   │   └── index.html        # HTML entry point
│   ├── src/
│   │   ├── App.jsx           # Main app component
│   │   ├── index.jsx         # Entry point
│   │   ├── index.css         # Tailwind styles
│   │   └── components/
│   │       ├── Sidebar.jsx    # Navigation & grade selection
│   │       ├── AIAssistant.jsx# Chat with AI tutor
│   │       └── CategoryView.jsx# Main content display
│   ├── tailwind.config.js     # Tailwind configuration
│   ├── postcss.config.js      # PostCSS configuration
│   └── package.json
│
├── server/                    # Express API backend
│   ├── server.js             # Main server file
│   ├── data/
│   │   └── syllabus.json     # Syllabus content
│   ├── package.json
│   └── .gitignore
│
├── README.md
└── .gitignore
```

## 🔌 API Endpoints

### POST /api/ask
Ask the AI tutor a question
```json
{
  "grade": "Grade 10",
  "question": "What is photosynthesis?"
}
```

### GET /api/syllabus/:grade
Get syllabus data for a grade
- `/api/syllabus/Grade%2010`
- `/api/syllabus/Grade%2011`
- `/api/syllabus/University`

### GET /health
Health check endpoint

## 🎨 Styling

- **Tailwind CSS 3.3+** for utility-first styling
- **Custom Pink Theme** for StudyBuddy branding
- **Responsive Design** with flexbox and grid
- **Smooth Transitions** and hover effects

## 📝 Data Structure

Syllabus data in `server/data/syllabus.json`:

```json
{
  "Grade 10": {
    "O/L Study Packs": [
      {
        "subject": "Mathematics",
        "lang": ["English", "Sinhala"],
        "topics": ["Algebra", "Geometry", "Trigonometry", ...]
      }
    ]
  }
}
```

## 🏗️ Component Architecture

```
App
├── Sidebar (Grade & Category Selection)
├── CategoryView (Main Content)
└── AIAssistant (Chat Interface)
```

## 🚧 Next Steps

- [ ] Connect to real AI API (OpenAI/Gemini)
- [ ] Add user authentication
- [ ] Implement progress tracking
- [ ] Add Sinhala language support
- [ ] Create interactive unit tests
- [ ] Add multimedia content (videos, images)
- [ ] Implement dark mode
- [ ] Add offline support

## 🤝 Contributing

1. Create a feature branch: `git checkout -b feature/amazing-feature`
2. Commit changes: `git commit -m 'Add amazing feature'`
3. Push to branch: `git push origin feature/amazing-feature`
4. Open a Pull Request

## 📄 License

MIT License - feel free to use this project for educational purposes

## 💬 Support

For questions or issues, please create an issue on GitHub.

---

**Built with ❤️ for students** 📚✨
