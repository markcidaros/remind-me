# ⏰ Remind Me

A to-do list that actually makes you remember. One self-contained HTML file — no install, no accounts, no server, no tracking.

Open `remind-me.html` in any browser on a PC or phone, or send the file to someone and they get their own completely separate private list.

## What it does

Adding a task is a short guided flow instead of a form:

1. **What do you need to remember?** — e.g. *"Tell Mr. X about the shipment delay"*
2. **When is the deadline?** — quick picks (In 1 hour, Tonight 6pm, Tomorrow 9am, In 3 days, Next week), an exact date & time, or no deadline at all
3. **When should I nudge you?** — see below
4. **Anything else?** — description, category, priority, repeat, checklist (all optional)
5. **Review** — change anything before saving

Every step after the first can be skipped, so a task can be one line and nothing more.

### Reminder options

These stack — pick as many as you want on one task:

| Type | Choices |
| --- | --- |
| At the deadline | Ping me when it's due |
| Warn me before | 10 min · 30 min · 1 hour · 3 hours · 1 day · 2 days · 1 week |
| Keep nagging until done | Every hour · day · 2 days · 3 days · week, at a time of day you choose |
| One-off exact reminder | Any specific date and time |

When a reminder fires: **Done**, **Snooze 1h**, **Snooze 3h**, **Tomorrow 9am**, or **Open**.

### Phone calendar integration

Every task has a 📅 button (plus **Add all to calendar**). It generates a standard `.ics` file that your phone imports into its own calendar app, alarms included — so **your phone reminds you natively, even if you never open this app again**. Works on both Android and iOS.

Editing a task and re-adding it updates the same calendar event instead of creating a duplicate.

### Everything else

- Search across titles, notes and checklist steps
- Filters: Overdue · Today · Upcoming · Completed
- Six colour categories, three priority levels
- Repeating tasks that roll forward to the next date when you tick them off
- Checklists with progress bars
- Three themes: Light, Solar, Dark
- Chime on reminder (toggleable)
- JSON backup export / import
- Keyboard shortcuts: `/` to search, `N` for a new task

## Privacy

Nothing ever leaves your device. Tasks are stored in your browser's `localStorage` only — there is no server, no analytics, and no network request of any kind. Two people opening the same file have two entirely separate lists that cannot see each other.

Because it's browser storage, clearing your browsing data erases your tasks — use **Settings → Export backup** if that matters to you.

## A note on notifications

System notifications are reliable when the page is **hosted over `https://`**. Opened as a local `file://`, most mobile browsers refuse to grant notification permission — in that case you'll still see in-app alerts, and the `.ics` calendar route works everywhere and needs no permission at all.

## License

MIT
