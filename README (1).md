# 🧘 ZenFlow — Student Wellness AI

> **Your personal student wellness companion.** ZenFlow is a single-file web app that helps students track stress, manage their schedule, and protect their mental health — all powered by AI.

---

## ✨ Features

### 📊 Dashboard
A personalized home screen with a daily greeting, this week's stress trend chart, today's schedule at a glance, sleep vs. productivity tracking, and habit streaks.

### ✍️ Daily Check-in
A guided form covering four wellness dimensions:
- **Sleep & Rest** — log sleep quality and duration
- **Mood & Energy** — rate how you're feeling
- **Academic Load** — track assignment pressure
- **Personal Concerns** — surface anything weighing on you

A **Live Stress Preview** updates in real time as you fill in the form.

### 🧠 Stress Analysis
- **28-Day Stress History** chart so you can spot patterns over time
- **AI Insight** — a natural-language summary of your recent trends and what's driving them

### 📅 Smart Schedule
AI-generated daily schedule optimized around your stress levels, with configurable settings and personalized study tips for the day.

### 💡 AI Recommendations
Actionable cards across four areas:
- Priority Actions
- Mindfulness & Recovery
- Academic Strategy
- Weekly Challenge

Includes a built-in **4-7-8 Breathing Exercise** guided by the app.

### 📸 Live Stress Scan
Uses your camera and **MediaPipe Face Mesh** to detect facial action units and produce a real-time stress score — no data leaves your device.

### 💬 Mental Health Hub
- Wellness tips library
- Guided breathing exercises
- **AI Wellness Companion** — a chat interface for in-the-moment support

### 😂 AI Humor Therapist
Pick how you're feeling and get AI-generated humor relief, quick mood boosters, and therapy session stats. Because sometimes laughter really is the best medicine.

### 🏆 Rewards & Achievements
Earn points and badges for consistency. Unlock vouchers you can actually redeem.

### 👨‍👩‍👧 Parent Portal
An optional view for parents with a weekly wellness overview, key metrics, and student-controlled privacy settings.

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Frontend | Vanilla HTML, CSS, JavaScript (single file) |
| Fonts | Syne (headings) · DM Sans (body) via Google Fonts |
| Auth & Database | Firebase (Auth + Firestore) |
| Face Analysis | MediaPipe Face Mesh |
| Email | EmailJS |
| Charts | Custom CSS bar charts |
| AI | Claude / LLM API (recommendations, insights, humor) |

ZenFlow is intentionally **zero-dependency** on the build side — no npm, no bundler, no framework. Just open the HTML file and go.

---

## 🚀 Getting Started

### Prerequisites
- A Firebase project (Auth + Firestore enabled)
- An EmailJS account (for parent alert emails)
- An Anthropic or compatible AI API key (for AI features)

### Setup

1. **Clone the repo**
   ```bash
   git clone https://github.com/your-username/zenflow.git
   cd zenflow
   ```

2. **Open `zenflow.html`** in any modern browser — no build step needed.

3. **Configure your credentials** inside the app's Settings panel:
   - Firebase config (API key, project ID, etc.)
   - EmailJS public key, service ID, and template ID
   - AI API key

4. **Sign in** with your student email and start your first check-in.

---

## 🔒 Privacy

- Facial data from the Stress Scan is processed **locally in your browser** and never sent to any server.
- All wellness data is stored in your own Firebase project — ZenFlow has no central database.
- The Parent Portal is gated behind student-controlled privacy settings.

---

## 🎨 Design

ZenFlow supports **Day and Night modes** with smooth transitions. The UI uses a consistent design token system (`--accent`, `--surface`, `--text`, etc.) making it easy to retheme.

---

## 📄 License

MIT — do whatever you want, just don't sell it as your own wellness product without contributing back. 🌿
