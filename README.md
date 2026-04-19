# 🪖 STONERS — Tactical Habit Tracker

> *"Discipline is the bridge between goals and accomplishment."*

A military-tactical themed habit tracker built with Python Flask. Track your daily missions, build streaks, and dominate your goals — operator style.

---

## 🖥️ Live Demo

> Deploy on Render and paste your URL here.

---

## ⚡ Features

- 🎯 **Daily Missions** — Add and track habits with military-style UI
- 🔥 **Streak Tracking** — Auto-calculated daily streaks
- 📡 **Smart Alerts** — Time-based alerts (Morning Brief, Evening Debrief, etc.)
- 📋 **Intel Reports** — Stats with bar charts and weekly trend graphs
- 📅 **Calendar Heatmap** — See your monthly completion history per habit
- 🪖 **Soldier Profile** — Rank system based on completion rate
- 🔐 **User Auth** — Register, login, secure sessions
- 💾 **Local Storage** — All data stored in SQLite on your machine

---

## 🛠️ Tech Stack

| Layer    | Technology              |
|----------|-------------------------|
| Backend  | Python + Flask          |
| Database | SQLite (local)          |
| Frontend | HTML + CSS + JavaScript |
| Charts   | Chart.js                |
| Hosting  | Render.com              |

---

## 🚀 Run Locally

**1. Clone the repo**
```bash
git clone https://github.com/YOUR_USERNAME/Stoners.git
cd Stoners
```

**2. Install dependencies**
```bash
pip install flask flask-sqlalchemy werkzeug gunicorn
```

**3. Run the app**
```bash
python app.py
```

**4. Open in browser**
```
http://127.0.0.1:5000
```

The database `stoners.db` will be created automatically on first run.

---

## 🌐 Deploy on Render.com

**1.** Push your code to GitHub (see above)

**2.** Go to [render.com](https://render.com) → Sign up / Log in

**3.** Click **New +** → **Web Service**

**4.** Connect your GitHub account → Select the `Stoners` repo

**5.** Fill in the settings:

| Field           | Value                        |
|-----------------|------------------------------|
| Name            | stoners-app                  |
| Environment     | Python                       |
| Build Command   | `pip install -r requirements.txt` |
| Start Command   | `gunicorn app:app`           |

**6.** Click **Create Web Service**

**7.** Wait ~2 minutes → your app is live! 🎉

> ⚠️ **Note:** Render free tier uses ephemeral storage — the SQLite database resets on every redeploy. For persistent data on Render, upgrade to a paid plan or switch to PostgreSQL.

---

## 📁 Project Structure

```
Stoners/
├── app.py              ← Flask backend + all routes
├── requirements.txt    ← Python dependencies
├── render.yaml         ← Render deployment config
├── stoners.db          ← SQLite database (auto-created)
└── templates/
    ├── base.html       ← Navigation + shared layout
    ├── index.html      ← Daily ops (home page)
    ├── stats.html      ← Intel report with charts
    ├── profile.html    ← Soldier dossier
    ├── habit_detail.html ← Mission calendar
    ├── login.html
    └── register.html
```

---

## 📊 Pages

| Page         | URL        | Description                        |
|--------------|------------|------------------------------------|
| Daily Ops    | `/`        | Today's missions + progress ring   |
| Intel        | `/stats`   | Charts + stats + mission list      |
| Soldier      | `/profile` | Profile, rank, completion rate     |
| Mission Brief| `/habit/ID`| Calendar heatmap per habit         |
| Authenticate | `/login`   | Login page                         |
| Enlist       | `/register`| Registration page                  |

---

## 👤 Author

**Selva Kailash S** — [@SelvaKailashS-visual](https://github.com/SelvaKailashS-visual)

---
