# 🌸 Bloblist

A task tracker that doesn't suck for ADHD brains.

A small, slightly unhinged blob lives at the top of your list. It judges your tasks (lovingly), panics about deadlines, and evolves as you complete things. There's a map. There are quests. There are treasure chests. It's one HTML file.

> *"the prophecy is fulfilled"* — Goober, after you check off your first task

## What makes it different

Most todo apps are quiet, polite, and easy to forget. Bloblist is built around the way ADHD brains actually work — **task initiation is the problem, not task tracking**, and **dopamine doesn't fire from a static checkbox**.

So it has:

- **A blob who reacts to you.** Different moods based on your day. Sad when ignored, smug after a streak.
- **Variable rewards.** Sometimes you finish a task and get 5 coins. Sometimes you hit a jackpot for 25. Slot-machine logic, intentionally.
- **Body doubling mode.** A pretend coworking session where the blob "works alongside you" with rotating idle messages every 8 seconds.
- **Task roulette.** When you don't know where to start, hit the dice. It picks for you.
- **A 2-minute sprint button.** Because 25 minutes feels too big sometimes.
- **A breakdown helper.** Any task can be expanded into 2–15 minute micro-steps. Use the built-in editor or hit "Ask Claude" for a copy-pasteable prompt.

## Features at a glance

### 📋 Tasks
- Quick capture with one input field
- Tags for **urgency** (today / this week / someday), **context** (work / personal), **energy** (quick / deep focus / errand)
- Subtasks with progress bars
- Deadlines with auto-calculated "X days left" / "overdue" warnings
- **🔁 Recurring tasks** (daily / weekly / 2 weeks / monthly) — auto-spawn next instance on completion
- Notes per task
- Filter chips for everything

### ⚡ Now mode
Shows **one task at a time**, with the next concrete subtask highlighted. For when the list feels overwhelming.

### ⚔️ Quests
Group related tasks under a custom quest with an emoji and reward. Complete all tasks → claim coins.

### 🌍 Map
6 regions unlock as you complete tasks: Home Meadow → Whisper Forest → Tangerine Beach → Cloud Peak → Neon Hollow → The Void. Click an unlocked region to teleport your blob there. Treasure chests appear here.

### 🛍 Shop
- 7 unlockable blob characters (Goober → Zorp → Smush → Blarp → Glorm → Nebula → Uwu)
- Cosmetic accessories: hats, shades, bowtie, flower, rainbow aura
- **Blob fusion lab**: combine 2 unlocked blobs to discover hybrids. 5 secret combinations exist.

### 📊 Stats
Last 7 days as a bar chart. Your most productive day of the week. Tasks by energy type. Recent moods (from check-ins).

### Daily mechanics
- **🔥 Streak counter** — consecutive days with at least one completion
- **❤️ HP** — drops if you ignore the app for days, recovers per task done
- **🧊 Streak insurance** — 1 free skip per week so a bad day doesn't reset everything
- **Daily check-in** — quick mood log (😊 😐 😴 😤 🥳 🫠) for +2 coins
- **NPC visitors** — random characters drop by some days with mini-quests for bonus coins
- **🔔 Browser notifications** for tasks due today/tomorrow (opt-in)

## Install / use

It's one file. Three ways:

**1. Open locally**
Download `index.html`, double-click. Done. Your data lives in your browser's localStorage and stays on your machine.

**2. Host on GitHub Pages**
1. Fork this repo (or push your own)
2. Go to `Settings → Pages`
3. Under "Build and deployment", set Source to **Deploy from a branch**, branch `main`, folder `/ (root)`
4. Save. In ~30 seconds you'll have a URL like `yourname.github.io/bloblist`

**3. Drop on any static host**
Netlify, Vercel, Cloudflare Pages, S3 — any of them. Drag and drop the file. Works.

## Privacy

All data is in `localStorage`, scoped to your browser. Nothing leaves your device. Nothing syncs across devices (this is a single-file project, not a backend service). If you and a friend use the same hosted URL, you each have separate task lists.

If you want cross-device sync, you'd need to fork this and add a backend (Supabase + a small auth flow would do it).

## Backup

Use the **Export JSON** button at the bottom of the app to save a backup file. **Import JSON** restores it. Do this occasionally, especially before clearing browser data.

## Browser support

Works in any modern browser. Uses `backdrop-filter` (frosted glass) which needs:
- Safari 14+
- Chrome / Edge 76+
- Firefox 103+

Older browsers will work but won't get the glass effect.

## Tech

Vanilla HTML, CSS, and JavaScript. No framework, no build step, no dependencies. ~1100 lines, single file.

## Credits

Designed and built collaboratively with [Claude](https://claude.ai). Inspired by ADHD productivity research and a healthy disdain for boring task apps.

## License

MIT — do what you want.