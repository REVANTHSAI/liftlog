# 🏋️ Lift Log

A lightweight, mobile-friendly workout tracker built with **HTML, CSS, and vanilla JavaScript**.

Lift Log helps you create structured workout plans, track exercises and weights, monitor progress, and optionally sync your data across devices.

## ✨ Features

- **Workout Tracking**
  - Log exercises, sets, reps, and weights.
  - Support for bodyweight exercises.
  - Track completed workout days.

- **Custom Workout Plans**
  - Create multi-week training blocks.
  - Configure the number of workout days per week.
  - Customize exercises, sets, reps, rest periods, and cardio.
  - Rename exercises and workout sessions.

- **Progress Tracking**
  - Maintain exercise weight history.
  - Reuse exercise names across training blocks so weight history carries over.
  - Track completed sets and workouts.

- **Rest Timer**
  - Configure rest periods between sets.
  - Use a built-in rest timer during workouts.

- **Local Storage**
  - Workout plans and workout logs are stored locally in the browser.
  - The app works without an account or backend.

- **Cloud Sync**
  - Optional synchronization using **JSONBin**.
  - Sync workout plans and workout history across devices.
  - Falls back to local storage when cloud synchronization is unavailable.

- **Import & Export**
  - Export workout plans and workout history as JSON.
  - Import workout plans from JSON files.
  - Paste a JSON workout plan directly into the app.

- **AI-Friendly Workout Plans**
  - Includes a JSON schema that can be provided to an AI assistant to generate compatible workout plans.
  - Generated plans can be imported directly into Lift Log.

## 🛠️ Tech Stack

- HTML5
- CSS3
- Vanilla JavaScript
- Browser Local Storage
- JSON
- JSONBin API

No frameworks, build tools, or package managers are required.

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/<your-username>/lift-log.git
cd lift-log
```

### 2. Open the application

Open `workout-final.html` in a modern web browser.

No installation or build step is required.

## ☁️ Optional Cloud Sync

Lift Log can optionally synchronize workout data using JSONBin.

To enable synchronization, provide:

- JSONBin Master Key
- JSONBin Bin ID

If cloud synchronization is not configured, Lift Log continues to work using local browser storage.

## 📦 Data Backup

You can export your workout plan and workout history as a JSON backup.

The exported data uses the following structure:

```json
{
  "v": 2,
  "plan": {},
  "log": {}
}
```

This makes it possible to back up and restore your workout data independently of the application.

## 🤖 Generate Workout Plans with AI

Lift Log includes a JSON schema for generating compatible workout plans with an AI assistant.

A generated plan can contain:

- Plan name
- Days per week
- Weeks per training block
- Training blocks
- Workout days
- Exercises
- Sets and reps
- Rest periods
- Cardio

The generated JSON can then be imported or pasted into Lift Log.

## 💾 Data Storage

Lift Log follows a local-first approach.

Workout plans and workout history are stored in the browser using `localStorage`. When JSONBin synchronization is enabled, the application can retrieve existing data and save changes to the configured cloud bin.

## 🔐 Privacy

Lift Log does not require a user account.

Without cloud synchronization enabled, workout data remains in your browser's local storage.

If JSONBin synchronization is enabled, workout data is transmitted to the configured JSONBin service.

## 📁 Project Structure

```text
lift-log/
│
├── workout-final.html
├── README.md
└── LICENSE
```

The application is contained in a single HTML file, making it easy to run and host as a static website.

## 🌐 Hosting

Because Lift Log is a static HTML/CSS/JavaScript application, it can be hosted using:

- GitHub Pages
- Netlify
- Vercel
- Any static web server

## 🎯 Project Goal

Lift Log is designed to provide a simple, fast, and distraction-free way to follow structured workout programs while maintaining a history of strength progression.

> [!WARNING]
> ## AI-Generated & Personal-Use Project
>
> This entire project was **completely AI-generated** and was created specifically to cater to my **personal workout-tracking use case**.
>
> The code has not been developed as a production-ready application or extensively reviewed for security, scalability, or reliability. If you choose to use, modify, or deploy this project, please review and test the code carefully for your own requirements.

## 📄 License

This project is licensed under the **MIT License**.

See the [LICENSE](LICENSE) file for the full license text.
