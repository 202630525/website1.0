# 🌿 Aura Planner (아우라 플래너)

> A calm, motivating, and frosted-glassmorphic time management web application built for college students to overcome academic overwhelm, track deadlines, and master their time.

---

## 📸 Overview & Vision

**Aura Planner** is designed to shift students from a state of reactive stress ("a slave to passing time") into proactive, mindful control over their schedules. Built with a soothing **Glassmorphism UI** layered over dynamic high-definition nature wallpapers, it provides an inspiring, distraction-free environment to plan studies, build habits, and preserve downtime without guilt.

---

## ✨ Core Features

### 1. 🌅 Hero Landing Page
- **Dynamic Backgrounds & Quotes:** Randomly fetches high-res nature visuals and inspirational quotes on every entry.
- **Interactive CTA:** A smooth glass roll-up button labeled **"공부 시작하자!^^"** that seamless routes users straight into their central command center.

### 2. 🏛️ Central Lobby (Dashboard)
- **Today's Top 3 Focus:** Quick-input card for daily non-negotiable goals.
- **Habit Tracker:** Simple check-in system for positive non-academic habits (e.g., reading, mindful rest).
- **Deadline Radar:** D-Day countdown summary for upcoming exams, homework, and performance evaluations (수행평가).
- **Burnout Guard Alert:** Visual safety warning triggered when continuous study blocks exceed 5 hours without a planned break.

### 3. ⏱️ Integrated Web Tools (In Development)
- **Multi-Horizon 30-Min Time Blocker:** Granular schedule planning with "High Energy / Low Energy" tags and "Guilt-Free Recreation" color coding.
- **Execution Speed Timer:** Task stopwatch to measure real execution time against estimated duration.
- **Deadline Calendar:** Visual schedule view with customizable warning alerts.

---

## 🎨 Design Aesthetic

- **Style:** Frosted Glassmorphism (`backdrop-blur-md`, translucent white panels, soft borders, subtle glowing highlights).
- **Theme:** Relaxing nature visuals paired with modern pastel accents.
- **Typography & Layout:** Clean, minimalist, and responsive.

---

## 🛠️ Tech Stack

- **Frontend Framework:** [React](https://react.dev/) + [Vite](https://vitejs.dev/)
- **Styling:** [Tailwind CSS](https://tailwindcss.com/)
- **Iconography:** [Lucide React](https://lucide.dev/)
- **Date Handling:** [date-fns](https://date-fns.org/)

---

## 📂 Project Structure

```text
aura-planner/
├── public/
├── src/
│   ├── components/
│   │   ├── HeroLanding.jsx       # Landing view with nature wallpaper & quotes
│   │   ├── CentralLobby.jsx      # Command dashboard (Top 3, Habits, D-Days)
│   │   ├── DeadlineCalendar.jsx  # Calendar & deadline manager
│   │   ├── ExecutionTimer.jsx    # Speed stopwatch
│   │   └── TimeBlocker.jsx       # 30-min granular time grid
│   ├── App.jsx                   # Main routing & state controller
│   ├── index.css                 # Custom glassmorphism utility classes
│   └── main.jsx                  # React entry point
├── index.html
├── tailwind.config.js
├── postcss.config.js
├── package.json
└── README.md
```

---

## 🚀 Quick Start Guide

### Prerequisites
- [Node.js](https://nodejs.org/) (v18.0.0 or higher)
- `npm` or `yarn`

### Installation

1. **Clone or create project directory:**
   ```bash
   cd aura-planner
   ```

2. **Install project dependencies:**
   ```bash
   npm install
   ```

3. **Start the local development server:**
   ```bash
   npm run dev
   ```

4. **Open in browser:**
   Navigate to `http://localhost:5173/` to view the website live!

---

## 📝 Glassmorphism CSS Reference

The project uses custom utility classes defined in `src/index.css`:

```css
@layer utilities {
  .glass-panel {
    @apply bg-white/20 backdrop-blur-md border border-white/30 shadow-2xl rounded-2xl;
  }
  .glass-card {
    @apply bg-white/15 backdrop-blur-sm border border-white/25 shadow-sm rounded-xl hover:bg-white/25 transition-all duration-200;
  }
  .glass-input {
    @apply bg-white/10 backdrop-blur-md border border-white/30 text-white placeholder-white/60 focus:outline-none focus:ring-2 focus:ring-white/50 rounded-lg px-4 py-2;
  }
  .glass-button {
    @apply bg-white/25 backdrop-blur-md border border-white/40 text-white font-semibold hover:bg-white/40 active:scale-95 shadow-lg rounded-full transition-all duration-300;
  }
}
```

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).
