# Kanha Tracker — Personal OS for 2026

A comprehensive personal productivity operating system built as a single-page HTML/CSS/JS application. Track goals, habits, learning, notes, routines, and more — all in one place.

---

## 🚀 Overview

**Kanha Tracker** is a self-contained personal dashboard designed for the "2026 Learning Year." It combines multiple productivity tools into a cohesive interface with localStorage persistence, dark theme, and zero external dependencies.

---

## ✨ Features

### 📊 Dashboard

- Daily focus area with persistent notes
    
- Progress rings and habit completion stats
    
- Active goals tracking with visual progress bars
    
- Learning progress (course lecture counter)
    
- Mission statement display
    
- Random motivational quote rotator
    
- Weekly habit summary heatmap
    
- Revision log status indicator
    

### 🎯 Goals

- **Year Goals** — Track progress (0-100%), add notes, update status (Active/Paused/Completed)
    
- **Monthly Goals** — Per-month goal checklists with completion tracking
    
- **Weekly Planner** — Day-by-day task lists with checkboxes
    

### ✅ Habits

- Daily habit checkoffs with streak tracking
    
- 30-day history view with visual calendar per habit
    
- Add/delete habits with custom icons
    

### ⏰ Routine Manager

- Create multiple daily routines (e.g., Weekday/Weekend)
    
- Time-slot based schedule with categories (Study/Break/Personal/Health)
    
- Set active routine for the day
    

### 📚 Learning Tracker

- Course management with lecture counters
    
- Increment/decrement completed lectures
    
- Daily learning logs (what you learned, notes, rating 1-5⭐, study hours)
    

### 📓 Sticky Notes

- Visual notes with color-coded backgrounds
    
- Pin to top / archive notes
    
- Search functionality
    
- Masonry-style grid layout
    

### 💡 Motivation Vault

- Editable mission statement
    
- Quote library (add, favorite, delete)
    
- Personal rules/commandments
    

### 📊 Analytics

- Best/current habit streak tracking
    
- Total study hours logged
    
- Goal completion stats
    
- **Charts:** Habit completion bar chart (14 days), Goal progress radar, Study hours per week, Today's habit donut
    
- Revision log heatmap (90 days)
    

### 📝 Revision Log

- Daily structured reflection entries
    
- Fields: What I learned, Web Dev notes, English notes, AI notes, Mistakes, Tomorrow's goals
    
- Day rating (1-5⭐) and study hours
    

### 🔭 Vision Board

- Multi-section vision board
    
- Text descriptions + image upload (stored as Data URLs)
    
- Sections: 2026 Vision, 2027 Vision, Long-term Vision (auto-seeded)
    

### 🖼️ Media Vault

- Image upload and storage (max ~5MB total)
    
- Categorization (Goal Charts, Routine Screenshots, Motivation, etc.)
    
- Lightbox gallery view
    
- Storage usage meter
    

### ⚙️ Settings

- Profile name management
    
- JSON export/import (full backup)
    
- Module-level data reset
    
- Complete data reset with confirmation
    
- Sidebar default state (expanded/collapsed)
    

---

## 🛠️ Technical Stack

|Layer|Technology|
|---|---|
|Frontend|HTML5, CSS3 (CSS Grid/Flexbox, Custom Properties)|
|JavaScript|Vanilla ES6+ (no frameworks)|
|Storage|localStorage (namespaced: `kanha_tracker_v1_*`)|
|Icons|Emoji + SVG|
|Fonts|Google Fonts: Space Grotesk, JetBrains Mono|
|Charts|Canvas-based custom drawing (no Chart.js)|

---

## 📁 File Structure

text

kanha-tracker-os.html   # Single-file application (HTML/CSS/JS)

The entire application is contained in **one HTML file** — open it in any modern browser and it runs instantly.

---

## 🚦 Getting Started

1. **Download** the `kanha-tracker-os.html` file
    
2. **Double-click** to open in your browser (Chrome, Edge, Firefox, Safari recommended)
    
3. Complete the **4-step onboarding**:
    
    - Enter your name
        
    - Set your mission statement
        
    - Select your 2026 goals
        
    - Define your success vision
        
4. Start tracking! All data saves automatically to your browser's localStorage
    

---

## 💾 Data Storage

- **Location:** Browser localStorage
    
- **Namespace:** `kanha_tracker_v1_` (all keys prefixed)
    
- **Modules stored:** goals, habits, routine, notes, learning, motivation, revision, vision, media, settings, onboarding
    
- **Estimated limit:** ~5MB (handles quota warnings gracefully)
    
- **Backup:** Use Settings → Export JSON to save your data
    

---

## 📱 Responsive Design

- Desktop-first with responsive breakpoints at 768px
    
- Collapsible sidebar with toggle button
    
- Mobile menu (hamburger button) with backdrop overlay
    
- Grid layouts adapt from 2-4 columns → 1 column on mobile
    

---

## 🎨 Color Palette (Dark Theme)

|Role|Color|
|---|---|
|Background Base|`#0F172A` (Slate 900)|
|Card Background|`#1E293B` (Slate 800)|
|Primary Accent|`#4F46E5` (Indigo 600)|
|Secondary Accent|`#38BDF8` (Sky 400)|
|Success|`#22C55E` (Green 500)|
|Warning|`#F59E0B` (Amber 500)|
|Danger|`#EF4444` (Red 500)|
|Text Primary|`#F8FAFC` (Slate 50)|
|Text Secondary|`#94A3B8` (Slate 400)|

---

## ⌨️ Keyboard Shortcuts

|Action|Key|
|---|---|
|Skip to main content|`Tab` then `Enter` (skip link)|
|Navigate sidebar|`Tab` + `Enter`|
|Check/uncheck habits|Click or `Space`/`Enter` on checkbox|

---

## 🔄 Data Persistence Example

javascript

// Storage module example
Storage.get('habits')     // Returns habits data
Storage.set('goals', data) // Saves goals
Storage.exportAll()       // JSON backup
Storage.resetAll()        // Clear everything

---

## 🧪 Browser Compatibility

|Browser|Version|
|---|---|
|Chrome|90+ ✅|
|Edge|90+ ✅|
|Firefox|88+ ✅|
|Safari|15+ ✅|
|Opera|76+ ✅|

Requires `localStorage`, `crypto.randomUUID()`, and modern ES6 features.

---

## 🚧 Future Enhancements (Planned)

- ☁️ Cloud sync (Firebase)
    
- 🔐 Google authentication
    
- 🤖 AI study assistant (Claude integration)
    
- 📅 AI daily planner
    
- 📱 Push notifications
    
- PDF/CSV export for analytics
    

---

## 📄 License

Private — Built for personal use (Kanha's 2026 Learning Year). Not for redistribution.

---

## 🙏 Credits

- **Design:** Kanha Tracker OS
    
- **Fonts:** [Space Grotesk](https://fonts.google.com/specimen/Space+Grotesk) by Florian Karsten, [JetBrains Mono](https://www.jetbrains.com/lp/mono/) by JetBrains
    
- **Icons:** System emoji
    

---

## 📞 Support

This is a self-contained local tool. No internet connection required after first load (except Google Fonts).

**To reset everything:** Settings → Reset ALL Data → Type "RESET" → Confirm

---

**Version:** 1.0.0  
**Year:** 2026 Learning Year  
**Author:** Kanha
