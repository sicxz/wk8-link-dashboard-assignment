# Week 8 Project // Build and Deploy a Personal Link Dashboard with AntiGravity

**Points:** 100  
**Due:** February 26 at 11:59 PM

## Overview
Build a personal link dashboard, the page you see every time you open a new browser tab. It should organize your most important links by category so everything you need is one click away.

Your app must let users:
- Add links
- Edit links
- Delete links
- Organize links into categories
- Save everything with `localStorage`

This is a static app (`HTML`, `CSS`, `JavaScript`) with no server and no external database. You will publish it with GitHub Pages.

## Live Demo
Add your demo link here.

## Before You Start
Make sure you have:
- A modern browser (Chrome, Firefox, or Edge)
- AntiGravity: <https://antigravity.google/>
- GitHub Desktop: <https://desktop.github.com/download/>

## Step 1: Set Up Your GitHub Account
GitHub is where developers store, share, and collaborate on code.

1. Go to <https://github.com> and create an account (if you do not already have one).
2. Choose a professional username.
3. Verify your email.

## Step 2: Build the Base App with AntiGravity
1. Create a folder named `dashboard` (Desktop is fine).
2. Open AntiGravity.
3. Paste this starter prompt:

```text
Build me a personal link dashboard that you'll use as your browser's new tab page.

The app organizes links into categories. Each category has a name and contains multiple links. Each link has a name and a URL.

Features I need:

Display links grouped by category
Add a new link (with name, URL, and which category it goes in)
Edit an existing link
Delete a link
Create and delete categories
Store everything using the browser's localStorage (NO background server, NO external database)
Must be a purely static site (HTML/CSS/JS) so I can easily host it on GitHub Pages for free.
Make it clean and minimal. This is a page I'll see hundreds of times, so it should load fast and look good.
```

4. Wait for file generation and confirm `index.html` exists.
5. Open `index.html` in your browser and test adding categories and links.
6. Make sure `index.html` is in the project root (not in `src/` or `app/`).

### Prompting Note
Do not try to do everything in one huge prompt. Build in steps. Test each step. If something breaks, tell the AI exactly what is wrong.

## Step 3: Iterate and Add Features
Pick at least **2** features below.

### 1) Make It Look Better
```text
The layout works, but I want to push my own personal aesthetic. (Describe what you want: e.g., "I want a brutalist web design", "I want it to look like a retro 90s computer", "I want soft pastel colors and rounded edges"). Use this time to converse with the AI to dial in the perfect look for you.
```

### 2) Add Panels for Different Contexts
```text
I want multiple panels, like tabs. For example a "Work" panel and a "Personal" panel, each with their own set of categories and links. Add a panel switcher at the top. Clicking a panel shows only that panel's categories and links.
```

### 3) Add Drag-and-Drop Reordering
```text
Let me reorder categories and links by dragging them. Add a drag handle on the left side of each item. When I drop something in a new position, save the new order. I should also be able to drag links between categories. Make the drag handles visible when I hover over an item so the dashboard stays clean.
```

### 4) Add a Description Field
```text
Add an optional description field to links. Show it as smaller, dimmer text below the link name. Include it in the add/edit form. Keep it optional.
```

### 5) Add Theme Switching
```text
Add a theme toggle: light mode, dark mode, and system (follows OS preference). Save the choice to localStorage. Apply the theme before the page paints so there's no flash of the wrong theme. Ensure the toggle is a select dropdown menu and works flawlessly without crashing.
```

### 6) Add Keyboard Shortcuts
```text
Let me press number keys 1 through 9 to switch between panels. Don't trigger shortcuts when I'm typing in a form field.
```

### 7) Connect School Assignments
```text
Let's connect this to my classes. Add a section that uses the Canvas LMS API (or my school's API) to automatically pull and display my upcoming assignments, their due dates, and links to submit them right on the dashboard.
```

### 8) Stretch Goal: Secure Edit Mode
```text
Since I'll be deploying this publicly to GitHub Pages, I don't want anyone else messing with my links. Add a static password lock screen overlay that requires a specific password (like 'password') before allowing access to Edit Mode or adding context links. Save the unlock state to localStorage so I only have to type it once, and add a Lock button so I can sign out!
```

### Design Note
Do not accept generic default AI styling. Pick a design reference and ask the AI to match the visual direction.

## Step 4: Push Your `dashboard` Folder to GitHub

### Option A (Recommended): GitHub Desktop
1. Open GitHub Desktop and sign in.
2. `File` -> `Add Local Repository...`
3. Choose `Desktop/dashboard`.
4. If needed, click `Create a repository`.
5. Publish it as **Public**.
6. For updates: commit, then `Push origin` (or `Sync`).

### Option B (Advanced): VS Code Terminal
```bash
git init
git add .
git commit -m "Add dashboard app"
```

Connect remote:
```bash
git remote add origin <PASTE-REPO-URL-HERE>
git branch -M main
git push -u origin main
```

Update later:
```bash
git add .
git commit -m "Update dashboard"
git push
```

## Step 5: Deploy with GitHub Pages
1. Open your repo on GitHub.
2. Go to `Settings` -> `Pages`.
3. Under Source, choose `Deploy from a branch`.
4. Choose branch `main` and folder `/ (root)`.
5. Save.
6. Wait 3-5 minutes and open the live URL.

## Submission (Canvas)
Submit:
1. **Live URL** (GitHub Pages)
2. **Repository URL**
3. **Brief Reflection (3-4 sentences)** answering:
   - Which follow-up features did you build?
   - What was it like using an AI assistant?
   - What mistakes did AntiGravity make, and how did you fix them?

## Grading Rubric
| Category | Points | Description |
|---|---:|---|
| Base App Working |  | Dashboard loads, CRUD works, categories work, `localStorage` persists |
| Feature Additions (2+) |  | At least two extra features are functional |
| Deployed and Live |  | Working GitHub Pages URL |
| Code on GitHub |  | Public repo with source code |
| Reflection |  | Thoughtful 3-4 sentence response |

## Troubleshooting
- **Pages shows README instead of app:** Move `index.html` to repo root, commit, and push.
- **Site did not update yet:** Wait 3-5 minutes, then hard refresh.
- **Generated code does not work:** Share exact error and behavior with AI.
- **Lost links:** `localStorage` is browser-specific. Clearing data or switching browsers can remove local data.
- **`fatal: not a git repository`:** Open terminal in the correct project folder first.

## Checklist
- [ ] ✅ Base app works
- [ ] ✅ At least 2 upgrades added
- [ ] ✅ Repo is public on GitHub
- [ ] ✅ Site is live on GitHub Pages
- [ ] ✅ Submission items are ready
