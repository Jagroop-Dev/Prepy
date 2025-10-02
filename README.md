# 📚 PCAD Exam Prep Platform

> A comprehensive, AI-powered study platform helping Data Analyst pathway students ace their PCAD certification exam — completely free.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![React](https://img.shields.io/badge/React-18+-61DAFB?logo=react)](https://reactjs.org/)
[![Supabase](https://img.shields.io/badge/Supabase-Database-3ECF8E?logo=supabase)](https://supabase.com/)
[![Vercel](https://img.shields.io/badge/Deployed%20on-Vercel-000000?logo=vercel)](https://vercel.com/)

---

## 🎯 What is this?

PCAD Exam Prep is a free web-based platform designed for students in the Digital Futures Data Analyst 12-week pathway. It provides everything you need to prepare for your certification exam:

- 🎓 **500+ Practice Questions** with detailed explanations
- 🎥 **12-Week Video Library** with searchable transcripts
- 🤖 **AI Study Assistant** powered by RAG (Retrieval-Augmented Generation)
- 📊 **Progress Analytics** to track your learning journey
- 🗂️ **Smart Flashcards** with spaced repetition
- 📝 **Note-Taking System** linked to video timestamps
---
<!--
## ✨ Key Features

### 🧠 AI-Powered Learning
Ask questions and get answers sourced directly from your course materials. The AI assistant searches through video transcripts and provides responses with clickable timestamps.

### 📈 Personalized Study Plans
Get adaptive recommendations based on your performance. The platform identifies weak areas and suggests what to study next.

### 🎮 Gamified Experience
Stay motivated with achievements, study streaks, and progress milestones. Turn exam prep into an engaging journey.

### 📱 Responsive Design
Study anywhere - fully optimized for desktop, tablet, and mobile devices.

---

## 🚀 Tech Stack

### Frontend
- **React 18** - UI framework
- **Vite** - Lightning-fast build tool
- **Tailwind CSS** - Utility-first styling
- **shadcn/ui** - Accessible component library
- **React Router v6** - Client-side routing
- **Zustand** - State management

### Backend & Database
- **Supabase** - PostgreSQL database, authentication, and storage
- **pgvector** - Vector embeddings for semantic search

### AI & Machine Learning
- **Google Gemini API** - AI response generation
- **OpenAI Embeddings** - Text embeddings for RAG
- **SM-2 Algorithm** - Spaced repetition for flashcards

### Deployment
- **Vercel** - Hosting and CI/CD
- **GitHub Actions** - Automated testing
- **Cloudflare** - CDN for static assets

---

## 📦 Installation

### Prerequisites
- Node.js 18+ 
- npm or yarn
- Supabase account (free tier)
- Google Gemini API key (free tier)

### Quick Start

```bash
# Clone the repository
git clone https://github.com/yourusername/pcad-exam-prep.git
cd pcad-exam-prep

# Install dependencies
npm install

# Set up environment variables
cp .env.example .env
# Edit .env with your Supabase and API keys

# Run database migrations
npm run db:migrate

# Start development server
npm run dev
```

Visit `http://localhost:5173` to see the app running!

---

## 🗄️ Database Setup

### Create Supabase Project
1. Go to [supabase.com](https://supabase.com) and create a new project
2. Copy your project URL and anon key
3. Enable pgvector extension in SQL editor:
   ```sql
   create extension vector;
   ```

### Run Migrations
```bash
npm run db:migrate
```

This will create all necessary tables:
- `users` - User accounts and preferences
- `topics` - 12-week curriculum structure
- `questions` - Practice question bank
- `videos` - Video library with transcripts
- `video_embeddings` - Vector embeddings for AI search
- `user_progress` - Track completed videos/topics
- `user_attempts` - Question attempt history
- `flashcards` - Spaced repetition system
- `notes` - User-generated notes
- `achievements` - Gamification system

---

## 🎨 Project Structure

```
pcad-exam-prep/
├── src/
│   ├── components/          # Reusable UI components
│   │   ├── ui/             # shadcn/ui components
│   │   ├── QuestionCard.jsx
│   │   ├── VideoPlayer.jsx
│   │   └── AIChat.jsx
│   ├── pages/              # Route pages
│   │   ├── Dashboard.jsx
│   │   ├── QuestionBank.jsx
│   │   ├── VideoLibrary.jsx
│   │   ├── StudyRoadmap.jsx
│   │   └── Analytics.jsx
│   ├── lib/                # Utilities and configs
│   │   ├── supabase.js
│   │   ├── ai.js
│   │   └── spacedRepetition.js
│   ├── hooks/              # Custom React hooks
│   ├── contexts/           # React contexts
│   └── App.jsx
├── public/                 # Static assets
├── supabase/              # Database migrations
└── docs/                  # Documentation
```

---

## 🧪 Development Phases

### ✅ Phase 1: MVP (Weeks 1-4) - CURRENT
- [x] Authentication system
- [x] Question bank with filtering
- [x] Practice test interface
- [x] Video library with transcripts
- [x] Basic progress tracking
- [x] Study roadmap

### 🚧 Phase 2: AI Features (Weeks 5-8) - IN PROGRESS
- [ ] RAG system setup
- [ ] AI study assistant
- [ ] Note-taking system
- [ ] Flashcard system with spaced repetition
- [ ] Analytics dashboard

### 📋 Phase 3: Polish (Weeks 9-12)
- [ ] Mobile optimization
- [ ] Achievement system
- [ ] Community features
- [ ] Discussion forum
- [ ] Study groups

### 🔄 Phase 4: Maintenance (Ongoing)
- [ ] Bug fixes and updates
- [ ] New content additions
- [ ] Performance monitoring

---

## 📊 Success Metrics

Our goals for the platform:
- **80%+** user satisfaction rate
- **20%+** improvement in practice test scores
- **<3 seconds** page load time
- **10+ hours** average study time per student
- **90%+** bug-free experience

---

## 🤝 Contributing

We welcome contributions! Here's how you can help:

1. **Fork the repository**
2. **Create a feature branch** (`git checkout -b feature/amazing-feature`)
3. **Commit your changes** (`git commit -m 'Add amazing feature'`)
4. **Push to the branch** (`git push origin feature/amazing-feature`)
5. **Open a Pull Request**

### Development Guidelines
- Follow the existing code style
- Write meaningful commit messages
- Test your changes thoroughly
- Update documentation as needed

---

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgments

- **Digital Futures** - For the amazing Data Analyst pathway program
- **Course Instructors** - For creating comprehensive study materials
- **Beta Testers** - For invaluable feedback and bug reports
- **Open Source Community** - For the incredible tools that made this possible

---

## 📞 Support

Having issues or questions?

- 📧 Email: support@pcadprep.com
- 💬 [Discussion Forum](https://github.com/yourusername/pcad-exam-prep/discussions)
- 🐛 [Report a Bug](https://github.com/yourusername/pcad-exam-prep/issues)
- 📖 [Documentation](https://docs.pcadprep.com)

---

## 🗺️ Roadmap

### Coming Soon
- 📱 Native mobile app (React Native)
- 🔌 Browser extension for quick access
- 📧 Email study reminders
- 💬 Real-time study sessions
- 🌍 Multi-language support
- 🎯 Custom quiz builder

---

## 💰 Cost Structure

This platform is **100% free** for students, built entirely on free-tier services:

- **Supabase Free Tier**: 500MB database, 1GB storage
- **Gemini API Free Tier**: 1,500 requests/day
- **Vercel Free Tier**: Unlimited deployments
- **Estimated Support**: 200-500 active students

If scaling is needed, costs would be approximately $25-50/month for hundreds of active users.

---

## 📈 Stats

![GitHub stars](https://img.shields.io/github/stars/yourusername/pcad-exam-prep?style=social)
![GitHub forks](https://img.shields.io/github/forks/yourusername/pcad-exam-prep?style=social)
![GitHub watchers](https://img.shields.io/github/watchers/yourusername/pcad-exam-prep?style=social)

---

<div align="center">

**[Website](https://pcadprep.vercel.app)** • **[Documentation](https://docs.pcadprep.com)** • **[Report Bug](https://github.com/yourusername/pcad-exam-prep/issues)** • **[Request Feature](https://github.com/yourusername/pcad-exam-prep/issues)**

Made with ❤️ for Data Analyst students

⭐ **Star this repo if you find it helpful!** ⭐

</div>
