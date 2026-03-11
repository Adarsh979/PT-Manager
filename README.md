# Today — Task Manager PWA

A minimal personal task manager with push notifications, built as a Progressive Web App.

## Features
- 📋 Task management with today's view
- 📅 Monthly calendar overview
- 🔔 Push notifications (morning summary, task reminders, evening nudge)
- 📱 Installable on Android & iOS
- 💾 Offline support via Service Worker
- 🆓 100% free to host on GitHub Pages

---

## 🚀 How to Deploy (GitHub Pages)

### Step 1 — Create a GitHub account
Go to [github.com](https://github.com) and sign up for free.

### Step 2 — Create a new repository
1. Click the **+** icon → **New repository**
2. Name it: `today-tasks` (or anything you like)
3. Set it to **Public**
4. Click **Create repository**

### Step 3 — Upload your files
**Option A — GitHub website (easiest):**
1. Open your new repo
2. Click **Add file** → **Upload files**
3. Drag and drop ALL files from this folder:
   - `index.html`
   - `sw.js`
   - `manifest.json`
   - `icons/` folder (both PNGs inside)
   - `.github/` folder (the whole thing)
4. Click **Commit changes**

**Option B — Git command line:**
```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/today-tasks.git
git push -u origin main
```

### Step 4 — Enable GitHub Pages
1. Go to your repo → **Settings** → **Pages**
2. Under **Source**, select **GitHub Actions**
3. The workflow will auto-deploy on every push

### Step 5 — Your app is live! 🎉
Your URL will be: `https://YOUR_USERNAME.github.io/today-tasks/`

---

## 📱 How to Install on Phone

### Android (Chrome):
1. Open your GitHub Pages URL in Chrome
2. Tap the **Install** banner that appears, OR
3. Tap the 3-dot menu → **Add to Home screen**

### iOS (Safari):
1. Open your GitHub Pages URL in Safari
2. Tap the **Share** button (box with arrow)
3. Tap **Add to Home Screen**
4. Tap **Add**

> ⚠️ On iOS, notifications only work when the app is installed to the home screen and you're on iOS 16.4+

---

## 🔔 Notifications Setup

1. Open the app and tap the 🔔 bell icon
2. Tap **Enable Notifications** and allow when prompted
3. Toggle on the notifications you want:
   - **Morning Summary** — daily task count at your chosen time
   - **Task Reminders** — fires at the time set per task
   - **Evening Nudge** — reminder if tasks are incomplete

---

## 🛠 How to Modify

All code is in a **single `index.html` file** — just open it in any text editor (VS Code, Notepad, etc.), make your changes, save, and push to GitHub. Your live site updates in ~30 seconds.

Common customizations:
- Change colors → edit the `:root` CSS variables at the top of `index.html`
- Change fonts → swap the Google Fonts link
- Add new fields to tasks → update the `submitTask()` function and task HTML template
