# 🪖 STONERS — Tactical Habit Tracker

> "Discipline is the bridge between goals and accomplishment."

A military-tactical themed habit tracker built with Python Flask. Track your daily missions, build streaks, and dominate your goals — operator style.

## 🖥️ Live Demo
**https://stoners.onrender.com**

---

## ⚡ Features

* 🎯 **Daily Missions** — Add and track habits with military-style UI
* 🔥 **Streak Tracking** — Auto-calculated daily streaks
* 📡 **Smart Alerts** — Time-based alerts (Morning Brief, Evening Debrief, etc.)
* 📋 **Intel Reports** — Stats with bar charts and weekly trend graphs
* 📅 **Calendar Heatmap** — See your monthly completion history per habit
* 🪖 **Soldier Profile** — Rank system based on completion rate
* 🔐 **User Auth** — Register, login, secure sessions
* 🐘 **PostgreSQL** — Persistent data storage via Supabase

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| Backend | Python + Flask |
| Database | PostgreSQL (Supabase) |
| Frontend | HTML + CSS + JavaScript |
| Charts | Chart.js |
| Hosting | Render.com |

---

## 🚀 Run Locally

**1. Clone the repo**
```bash
git clone https://github.com/SelvaKailashS/Daily-Task-Manager.git
cd Daily-Task-Manager
```

**2. Install dependencies**
```bash
pip install -r requirements.txt
```

**3. Run the app**
```bash
python app.py
```

**4. Open in browser**
http://127.0.0.1:5000

---

## 🌐 Deploy on Render.com

1. Push your code to GitHub
2. Go to **render.com** → Sign up / Log in
3. Click **New +** → **Web Service**
4. Connect your GitHub account → Select the repo
5. Fill in the settings:

| Field | Value |
|-------|-------|
| Name | stoners |
| Environment | Python |
| Build Command | `pip install -r requirements.txt` |
| Start Command | `gunicorn app:app` |

6. Add environment variable:

| Key | Value |
|-----|-------|
| `DATABASE_URL` | Your Supabase PostgreSQL connection string |

7. Click **Create Web Service** → your app is live! 🎉

---

## 📁 Project Structure
Daily-Task-Manager/
├── app.py                ← Flask backend + all routes
├── requirements.txt      ← Python dependencies
├── .python-version       ← Python 3.12.3
└── templates/
├── base.html         ← Navigation + shared layout
├── index.html        ← Daily ops (home page)
├── stats.html        ← Intel report with charts
├── profile.html      ← Soldier dossier
├── habit_detail.html ← Mission calendar
├── login.html
└── register.html

---

## 📊 Pages

| Page | URL | Description |
|------|-----|-------------|
| Daily Ops | `/` | Today's missions + progress ring |
| Intel | `/stats` | Charts + stats + mission list |
| Soldier | `/profile` | Profile, rank, completion rate |
| Mission Brief | `/habit/ID` | Calendar heatmap per habit |
| Authenticate | `/login` | Login page |
| Enlist | `/register` | Registration page |

---

## 👤 Author

**Selva Kailash S** — [@SelvaKailashS](https://github.com/SelvaKailashS)
