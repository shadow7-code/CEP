# StudySaathi 3.0

A premium, modern, multi-page productivity web app designed to help students manage their study time, tasks, and goals effectively.

![StudySaathi 3.0](https://img.shields.io/badge/Version-3.0-blue)
![License](https://img.shields.io/badge/License-MIT-green)

## 📋 Project Overview

StudySaathi 3.0 is a fully responsive, feature-rich productivity platform built with modern web technologies. It provides students with all the tools they need to stay organized, focused, and motivated throughout their academic journey.

### Key Highlights
- ✨ **Premium UI/UX** - Apple-style soft design with Notion-inspired minimal layout
- 📱 **Fully Responsive** - Perfect experience on mobile, tablet, and desktop
- 🌓 **Light/Dark Mode** - Beautiful theme switching with system preference support
- 🎨 **Customizable** - Multiple accent colors to personalize your experience
- 💾 **LocalStorage Based** - No backend required, all data stored locally
- ⚡ **Lightweight** - Fast loading with optimized performance

## ✨ Features

### 1. **Home Dashboard** (`index.html`)
- Overview of XP, streak, completed tasks, and study time
- Quick action buttons to jump to key features
- Recent activity timeline
- XP progress visualization

### 2. **Task Manager** (`tasks.html`)
- Create, edit, and delete tasks
- Priority levels (High, Medium, Low)
- Due date tracking
- Filter by status (All, Active, Completed)
- Task completion rewards XP

### 3. **Study Timer** (`timer.html`)
- Pomodoro technique (25-minute focus sessions)
- Short breaks (5 minutes)
- Long breaks (15 minutes)
- Session history tracking
- Auto-start break after Pomodoro
- Browser notifications for completion

### 4. **Breathing Exercises** (`breathing.html`)
- Multiple breathing techniques:
  - **Box Breathing** - 4-4-4-4 seconds
  - **4-7-8 Method** - Stress relief and sleep aid
  - **Deep Breathing** - 5-5 seconds simple technique
  - **Alternate Nostril** - 6-6-6 pattern
- Visual breathing animation with smooth CSS transitions
- Guided instructions

### 5. **Notes App** (`notes.html`)
- Create and manage notes
- Pin important notes
- Search functionality
- Rich text editing
- Character count display

### 6. **Exam Countdown** (`exams.html`)
- Track upcoming exams with countdown timers
- Subject and location tracking
- Color-coded urgency (red for <7 days, yellow for <30 days)
- Exam date and time management

### 7. **Analytics** (`analytics.html`)
- Study time chart (last 7 days)
- Task completion visualization
- XP progress tracking
- Activity timeline
- Comprehensive statistics overview

### 8. **Chatbot** (`chatbot.html`)
- Rule-based study assistant
- Answers questions about:
  - Study tips and focus techniques
  - Current streak and stats
  - Task completion
  - XP and level
  - Study time
- Quick question suggestions
- Motivational messages

### 9. **Settings** (`settings.html`)
- Theme toggle (Light/Dark)
- Accent color selection (6 options)
- Data export (JSON)
- Data import (JSON)
- Clear all data option

## 🛠 Tech Stack

- **HTML5** - Semantic markup
- **TailwindCSS** - Utility-first CSS framework (via CDN)
- **Vanilla JavaScript** - No frameworks required for core functionality
- **Chart.js** - Beautiful charts and graphs
- **localStorage API** - Client-side data persistence

### Notes on Technology Choices
- ✅ Pure JavaScript (`.js` files only)
- ✅ No TypeScript (`.ts` or `.tsx` files)
- ✅ Lightweight and fast loading
- ✅ No backend dependencies
- ✅ Works offline after initial load

## 📁 Folder Structure

```
studysaathi-3.0/
├── index.html              # Home Dashboard
├── tasks.html              # Task Manager
├── timer.html              # Pomodoro Timer
├── breathing.html          # Breathing Exercises
├── notes.html              # Notes App
├── exams.html              # Exam Countdown
├── analytics.html          # Analytics & Charts
├── chatbot.html            # Chatbot Assistant
├── settings.html           # User Settings
├── css/
│   └── styles.css          # Custom styles and animations
├── js/
│   ├── storage.js          # localStorage management
│   ├── ui.js               # UI utilities and helpers
│   ├── tasks.js            # Task manager logic
│   ├── timer.js            # Timer functionality
│   ├── breathing.js        # Breathing exercises
│   ├── notes.js            # Notes management
│   ├── exams.js            # Exam countdown
│   ├── analytics.js        # Analytics and charts
│   ├── chatbot.js          # Chatbot responses
│   └── settings.js         # Settings management
├── components/
│   └── shared-nav.html     # Shared navbar and sidebar
├── assets/                 # Optional assets folder
│   ├── icons/
│   ├── images/
│   └── lottie/
└── README.md               # This file
```

## 📱 Responsive Design

StudySaathi 3.0 is built with a **mobile-first approach** using TailwindCSS breakpoints:

- **Mobile** (< 768px): 
  - Collapsible sidebar
  - Single-column layouts
  - Touch-friendly buttons
  - Optimized spacing

- **Tablet** (768px - 1024px):
  - Two-column grids
  - Visible sidebar
  - Balanced layouts

- **Desktop** (> 1024px):
  - Full sidebar navigation
  - Multi-column grids
  - Maximum content width
  - Hover effects

### TailwindCSS Breakpoints Used
- `sm:` - 640px and up
- `md:` - 768px and up
- `lg:` - 1024px and up
- `xl:` - 1280px and up

## 🎨 Animation Details

All animations are **CSS-only** (no 3D libraries):

### CSS Animations Included

1. **Breathing Animation** (`@keyframes breathe`)
   - Scale and opacity transitions
   - Smooth easing for inhale/exhale

2. **Fade In** (`@keyframes fadeIn`)
   - Elements fade in with slight upward movement
   - Used for new content appearance

3. **Pulse** (`@keyframes pulse`)
   - Gentle opacity pulsing
   - Used for attention-drawing elements

4. **Shimmer Effect**
   - Gradient shimmer animation
   - Subtle background movement

5. **Smooth Transitions**
   - All interactions use `transition-all duration-300`
   - Hover effects with `transform translateY`
   - Tilt effects on hover

### Interactive Effects

- **Tilt Hover**: Cards lift slightly on hover (`translateY(-4px)`)
- **Scale Animations**: Breathing circle scales smoothly
- **Color Transitions**: Theme switching with smooth color changes
- **Progress Bars**: Animated width transitions

### No 3D Animations
- ❌ No Three.js
- ❌ No 3D models or shapes
- ❌ No WebGL
- ✅ Pure CSS transforms and transitions

## 💾 LocalStorage

All data is stored in the browser's `localStorage`. No backend or database required!

### Data Stored

1. **Tasks** (`studysaathi_tasks`)
   - Task objects with title, description, priority, dueDate, completed status

2. **Notes** (`studysaathi_notes`)
   - Note objects with title, content, pinned status, timestamps

3. **Timer History** (`studysaathi_timer_history`)
   - Completed Pomodoro sessions with duration and mode

4. **Exam Dates** (`studysaathi_exam_dates`)
   - Exam information with name, subject, date, location

5. **User Preferences** (`studysaathi_user_prefs`)
   - Theme (light/dark)
   - Accent color
   - Notification settings

6. **Daily Streak** (`studysaathi_daily_streak`)
   - Current streak count
   - Longest streak
   - Last update date

7. **XP System** (`studysaathi_xp`)
   - Total experience points
   - Used to calculate level

8. **Statistics** (`studysaathi_stats`)
   - Tasks completed
   - Total study time
   - Notes created
   - Sessions completed

### Storage Utility

The `storage.js` file provides a clean API:
- `Storage.getTasks()` / `Storage.saveTasks()`
- `Storage.getNotes()` / `Storage.saveNotes()`
- `Storage.getXP()` / `Storage.addXP()`
- `Storage.exportData()` / `Storage.importData()`
- And more...

## 🚀 Usage Instructions

### Getting Started

1. **Clone or Download** the project
   ```bash
   git clone [repository-url]
   cd studysaathi-3.0
   ```

2. **Open in Browser**
   - Simply open `index.html` in any modern web browser
   - No build process or installation required!
   - Works with any local server (VS Code Live Server, Python http.server, etc.)

3. **Start Using**
   - Navigate through pages using the sidebar
   - Create tasks, start timers, write notes
   - Track your progress in Analytics

### Recommended Setup

For best experience, use a local development server:

**Python:**
```bash
python -m http.server 8000
# Open http://localhost:8000
```

**Node.js (http-server):**
```bash
npx http-server
```

**VS Code:**
- Install "Live Server" extension
- Right-click `index.html` → "Open with Live Server"

### Browser Compatibility

- ✅ Chrome/Edge (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Opera (latest)
- ⚠️ IE11 (not supported)

## 📤 Import/Export

### Export Data

1. Go to **Settings** page
2. Click **"Export"** button in Data Management section
3. A JSON file will be downloaded with all your data
4. File name: `studysaathi-export-YYYY-MM-DD.json`

### Import Data

1. Go to **Settings** page
2. Click **"Import"** button
3. Select a previously exported JSON file
4. Confirm the import (will overwrite current data)
5. Page will reload with imported data

### Backup Recommendations

- Export your data regularly
- Store backups in cloud storage
- Export before clearing browser data

### Export Format Example

```json
{
  "tasks": [...],
  "notes": [...],
  "timerHistory": [...],
  "examDates": [...],
  "userPrefs": {...},
  "streak": {...},
  "xp": 250,
  "stats": {...},
  "exportDate": "2024-01-15T10:30:00.000Z"
}
```

## 🎨 Customization

### Changing Accent Colors

1. Go to **Settings**
2. Click any of the 6 accent color options:
   - Blue (default)
   - Purple
   - Green
   - Red
   - Orange
   - Pink

The accent color affects:
- Buttons and links
- Progress bars
- Gradient backgrounds
- Highlight colors

### Theme Customization

Edit `css/styles.css` to customize:
- Color schemes
- Animation durations
- Border radius values
- Shadow styles

### Adding Features

The modular structure makes it easy to add features:
1. Create new HTML page
2. Add corresponding JS file in `js/` folder
3. Update `components/shared-nav.html` with new link
4. Use `Storage` class for data persistence

## 🏆 XP & Streak System

### Earning XP

- ✅ Complete a task: **+10 XP**
- ⏱️ Finish Pomodoro session: **+25 XP**
- 📝 Create a note: **+5 XP**

### Levels

- Level = `floor(XP / 100) + 1`
- Each level requires 100 XP
- Level 1: 0-99 XP
- Level 2: 100-199 XP
- And so on...

### Daily Streak

- Streak increments when you complete any activity
- Streak resets if you miss a day
- Track your longest streak
- Motivation to stay consistent!

## 🎯 Best Practices

### For Students

1. **Start with Tasks**: Create your study tasks for the week
2. **Use Pomodoro**: Work in 25-minute focused sessions
3. **Take Breaks**: Use breathing exercises between sessions
4. **Track Exams**: Add upcoming exams for countdown
5. **Review Analytics**: Check your progress weekly
6. **Stay Motivated**: Chat with the assistant for tips

### Productivity Tips

- Set specific task due dates
- Use priority levels effectively
- Pin important notes
- Maintain your daily streak
- Review analytics regularly

## 🐛 Troubleshooting

### Data Not Saving

- Check if localStorage is enabled in your browser
- Ensure you're not in private/incognito mode
- Clear browser cache and reload

### Charts Not Displaying

- Ensure internet connection (Chart.js loads from CDN)
- Check browser console for errors
- Try refreshing the Analytics page

### Theme Not Changing

- Hard refresh the page (Ctrl+Shift+R / Cmd+Shift+R)
- Check browser console for errors
- Clear cache and reload

## 📄 License

This project is open source and available under the MIT License.

## 🙏 Acknowledgments

- **TailwindCSS** - Utility-first CSS framework
- **Chart.js** - Beautiful charts
- **Inter Font** - Beautiful typography
- **Heroicons** - SVG icons (via TailwindCSS)

## 📞 Support

For issues, questions, or contributions:
- Open an issue on GitHub
- Check existing documentation
- Review code comments

## 🔮 Future Enhancements

Potential features for future versions:
- [ ] Reminders and notifications
- [ ] Calendar integration
- [ ] Study groups/collaboration
- [ ] Advanced analytics
- [ ] Mobile app (PWA)
- [ ] Cloud sync option

---

**Built with ❤️ for students worldwide**

*StudySaathi 3.0 - Your Companion for Academic Success*

