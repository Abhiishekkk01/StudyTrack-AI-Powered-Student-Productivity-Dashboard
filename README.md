StudyTrack 📚
An AI-powered student productivity dashboard that helps you manage deadlines, tasks, and study sessions — without the manual effort.
🚀 Features

AI Syllabus Extractor — Upload a syllabus PDF or paste text; Claude AI auto-creates all tasks and deadlines instantly
Live Deadline Countdown — Color-coded urgency timers (🔥 urgent / ⚠ soon / ✓ ok) updating every minute
Procrastination Detector — Detects idle behavior and sends personalized nudges to get you back on track
Focus Timer — Pomodoro-style sessions (Classic 25/5, Deep Work 50/10) with streak tracking
Task Manager — Add, filter, and prioritize tasks by urgency and subject
Alerts & Notifications — Smart alerts with dismissal, custom creation, and notification bell
Reminder Scheduler — Set daily/weekly reminders with toggles
Analytics Dashboard — 4 live Chart.js charts: study hours, productivity trend, task completion, time distribution
Settings — Notification preferences, study goal slider, weekly task targets

🛠 Tech Stack

Vanilla HTML / CSS / JavaScript (single file, no build step)
Chart.js — analytics charts
Anthropic Claude API — AI syllabus extraction
Google Fonts — Space Grotesk, DM Sans

⚡ Getting Started
No installation required. Just open the file in a browser.
bashgit clone [https://github.com/your-username/studytrack.git](https://abhiishekkk01.github.io/StudyTrack-AI-Powered-Student-Productivity-Dashboard/)
cd studytrack
open index.html

The AI Syllabus Extractor requires an active internet connection to call the Anthropic Claude API.

📁 Project Structure
studytrack/
├── student-dashboard-enhanced.html   # Entire app — self-contained
└── README.md
🔑 API Usage
The AI feature uses the Anthropic Claude API (claude-sonnet-4-20250514) directly from the browser. To use your own key, locate the fetch call in the script section and add:
javascriptfetch("https://api.anthropic.com/v1/messages", {
  method: "POST",
  headers: {
    "Content-Type": "application/json",
    "x-api-key": "YOUR_API_KEY_HERE",
    "anthropic-version": "2023-06-01"
  },
  ...
})
🧠 HCI Principles Applied
PrincipleImplementationAffordanceDashed drop-zone signals file upload; toggle switches signal on/off stateFeedbackSnackbar toasts, loading spinners, badge counts confirm every actionError PreventionAI extraction shows preview before committing tasks to dashboardEfficiencySyllabus upload replaces 20+ manual task entries in one clickVisibilityDeadline countdown always on home screen — no digging required
⚠️ Known Limitations

Data resets on page refresh (no localStorage persistence yet)
Not fully mobile responsive
AI extraction requires internet connection

🗺 Roadmap

 localStorage persistence across sessions
 Mobile responsive layout
 AI study plan generator from exam dates
 Canvas/LMS integration for real assignment sync
 Collaborative study session sharing

👤 Author
Abhishek P — HCI Final Project, May 2026
