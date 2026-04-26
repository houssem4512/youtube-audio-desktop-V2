# 🎵 TubeGrab — YouTube Audio Downloader with AI Analysis

TubeGrab is a modern full-stack application that allows users to download YouTube videos as high-quality MP3 files, analyze music using AI, and play tracks with a built-in audio player. It combines **React, FastAPI, and optional Tauri desktop support** to deliver a smooth and powerful user experience.

---

## 🚀 Features

- 🎧 YouTube to MP3 downloader (high quality audio)
- 🤖 AI music analysis (genre, mood, artist, album, confidence score)
- 📚 Download history with search & delete
- 🎵 Built-in music player with progress bar
- ⚡ Real-time loading & toast notifications
- 💻 Optional desktop app using Tauri
- 🎨 Modern UI with animations and glassmorphism design

---

## 🧠 Tech Stack

Frontend: React + TypeScript + CSS  
Backend: FastAPI (Python)  
AI Layer: Custom music analysis engine  
Downloader: yt-dlp + FFmpeg  
Desktop (optional): Tauri (Rust)

---

## 📁 Project Structure

youtube-audio-desktop/
├── src/ (React frontend)
│   ├── pages (Home, History)
│   ├── components (MusicPlayer, AI panel)
│   └── App.tsx
│
├── backend/
│   ├── main.py (FastAPI server)
│   ├── download.py (yt-dlp logic)
│   ├── ai_service.py (AI analysis)
│   ├── database.py (history system)
│   └── config.py
│
├── src-tauri/ (optional desktop app)
└── package.json

---

## ⚙️ Installation

### 1. Clone repository
git clone https://github.com/your-username/youtube-audio-desktop.git
cd youtube-audio-desktop

---

### 2. Install frontend
npm install

---

### 3. Install backend dependencies
cd backend
pip install fastapi uvicorn yt-dlp pydantic

Install FFmpeg:
Windows: https://ffmpeg.org/download.html  
Linux:
sudo apt install ffmpeg

---

## ▶️ Running the project

### Start backend
cd backend
uvicorn main:app --reload

Backend runs at:
http://127.0.0.1:8000

---

### Start frontend
npm run dev

Frontend runs at:
http://localhost:5173

---

### Optional desktop app
npx tauri dev

---

## 🎯 How to use

1. Paste a YouTube URL
2. AI analyzes the video (genre, mood, artist)
3. Click Download MP3
4. Track download progress
5. Play music instantly in the built-in player
6. View or manage history anytime

---

## 🧩 API Endpoints

POST /analyze → Analyze YouTube video  
POST /download → Download MP3 file  
GET /history → Get download history  
DELETE /history/{video_id} → Delete entry  

---

## 🛠 Troubleshooting

- If audio does not play → check backend is running
- If analysis stuck → restart FastAPI server
- If download fails → ensure FFmpeg is installed
- If frontend not updating → restart npm dev server

---

## 📌 Future improvements

- Spotify integration
- Playlist system
- Cloud sync
- AI playlist generator
- Mobile version (React Native)

---

## 👨‍💻 Author

Built with React + FastAPI + AI audio processing pipeline

---

## 📄 License

This project is for educational and personal use.
