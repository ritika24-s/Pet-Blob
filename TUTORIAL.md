# Bloblist — User Guide

A walkthrough of every feature, written for someone opening it for the first time.

---

## The basics

When you open Bloblist, you'll see your blob (Goober, by default) at the top with a few stats next to its name:

| Pill | Meaning |
|---|---|
| 🔥 0 | Streak — consecutive days with at least one task completed |
| 🪙 0 | Coins — earned by completing tasks, used in the shop |
| ❤️ 100 | HP — your blob's wellbeing. Drops if ignored, recovers per task |

Below that is a level bar (1 level per 5 tasks done) and a mood line — random sass, depending on your task list.

---

## The tabs

### ⚡ Now
Shows ONE task: the most urgent unfinished one, with the next subtask spotlit. When the whole list feels too much, come here.

### 📋 Tasks
Your full list. Type a task and hit Enter to capture quickly — defaults to "this week", "work", "quick win". Click any task to edit details.

### ⚔️ Quests
Group related tasks under a custom name with an emoji and reward. Use this for projects with multiple subtasks (e.g. "Launch the website", "Plan birthday party").

### 🌍 Map
Your blob's world. Six regions unlock as you complete tasks. Click any unlocked region to teleport your blob. Treasure chests show up here as 💰 markers.

### 🛍 Shop
Three sections: blobs you've unlocked, blob fusion lab (combine two for hybrids), accessories you can buy with coins.

### 📊 Stats
The last 7 days as a chart, your most productive weekday, total stats, and your mood log if you've been doing daily check-ins.

### ✅ Done
Everything you've completed. Helpful when you want to feel productive.

---

## How to actually use it

### Adding a task
Type in the top box. Hit Enter. That's it.
For more detail (deadline, energy level, recurring), click the task title to open the edit modal.

### Breaking down a big scary task
Click **✨ smaller** on any task. Two options:
1. Type your own steps, one per line
2. Hit "Ask Claude" — copies a structured prompt to your clipboard. Paste into a Claude chat (or any LLM), get back a numbered list, paste back.

Each step should take 2–15 minutes. Embarrassingly small steps are correct.

### Focus modes
- **⏱ Focus 25** — Pomodoro timer for that task. Earns 5 coins on completion.
- **⚡ 2-min sprint** — Same but for 2 minutes. Use it to break inertia. Earns 2 coins.
- **👥 Body double** — 25-min session where the blob "works alongside you" with rotating idle messages. Helps with task initiation. Earns 3 coins.

### When you don't know where to start
Hit **🎲 Pick one for me**. It picks a task (weighted toward urgent ones) and jumps you to the Now view.

### Recurring tasks
Open a task's edit modal. Set "🔁 Repeat" to Daily / Weekly / 2 weeks / Monthly. When you complete it, a fresh copy auto-spawns with the next deadline. Subtasks reset.

### Daily check-in
Once a day, a mood card appears at the top: 😊 😐 😴 😤 🥳 🫠. Tap one. Earn 2 coins. Your moods build a little log over time, visible in the Stats tab.

---

## The game layer

### Earning coins
- Quick task: 5 coins (sometimes 10 or 25 if lucky)
- Deep focus task: 8 coins
- Errand: 4 coins
- Daily check-in: 2 coins
- Pomodoro completion: 2-5 coins
- NPC quest reward: 10-30 coins
- Quest completion: whatever you set

### Variable rewards (loot)
Each task completion rolls dice:
- 5% chance → JACKPOT (5x normal)
- 10% chance → Lucky (2x)
- 10% chance → small bonus (+3)
- 75% chance → normal

This is intentional. Predictable rewards stop firing dopamine after a week. Variable ones don't.

### Treasure chests
Every 10th task you complete spawns a chest in a random unlocked region. You'll see 💰 markers on the map and chest icons in the Shop. Tap to open. Loot is random:
- 35% chance: small coin pile (30)
- 25% chance: medium pile (75)
- 25% chance: hefty haul (150)
- 15% chance: free shop item

### NPC visitors
About 40% of days, a random NPC blob appears as a card on your Tasks tab with a small mini-quest:
- **The wanderer** wants you to finish 3 tasks today
- **The merchant** wants 5 tasks
- **The sage** wants one deep focus task
- **The partygoer** wants a quick win
- **The mystery figure** just wants any task

Complete their condition that day → bonus coins. They leave at end of day either way.

### Blob fusion
In the Shop. Tap the two slot circles to cycle through your unlocked blobs. Hit "✨ fuse them". 50 coins per attempt. There are 5 secret hybrid combinations to discover.

Wrong combinations don't cost anything — they just say "those don't combine".

### HP system
Starts at 100, floor of 20.
- Drops 10 per day if you don't complete anything (after a 1-day grace period)
- Recovers 5 per task completed
- Below 40, blob looks sad and acts tired

Not punishment — just feedback. The blob is your gentle accountability buddy, not a drill sergeant.

### Streak insurance
Hit **🧊 Freeze streak** at the bottom once per week. Marks yesterday as "completed" so your streak survives a real bad day. Resets every Sunday.

---

## Settings & data

### Backup your data
**Export JSON** → saves a `bloblist-YYYY-MM-DD.json` file with everything (tasks, quests, meta).
**Import JSON** → restores from backup. Replaces current data.
**Copy as text** → markdown-style task list to your clipboard, useful for sharing or pasting into a Claude chat.

### Notifications
**🔔 Enable reminders** at the bottom. Browser asks for permission. After granting, you'll get one notification per day if any tasks are due today/tomorrow.

### Resetting
There's no "reset" button on purpose. If you really want to start fresh: open browser dev tools, go to the Application/Storage tab, find `bloblist_v3` and `bloblist_meta_v3` in localStorage, delete them, refresh.

---

## Tips that actually help

1. **Use the Now tab when the list is overwhelming.** It hides everything else.

2. **Set tasks as "Today" sparingly.** If everything is today, nothing is.

3. **Energy tags matter more than urgency.** When you have 10 minutes between meetings, filter to "Quick" or "Errand". You'll find something to actually do.

4. **Recurring tasks for habits, not chores.** "Read 10 pages" recurring daily works better than "Read 100 pages today".

5. **Daily check-ins build awareness.** Even if you skip everything else, those 14 mood emojis in Stats start to show patterns.

6. **The blob is on your side.** Even when it's sassing you. Especially then.
