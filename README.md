# ADHD Flow

An ADHD-friendly PWA for daily focus. Morning checklist, Pomodoro timer, rotating mantras, and a full system guide — all in one file, installable on your phone.

**[Live demo →](https://silasgubi.github.io/adhd-flow/)**

---

## What it does

| Feature | Description |
|---------|-------------|
| Morning checklist | Auto-resets at midnight |
| Rotating mantra | Random phrase on each open (20 curated) |
| Pomodoro 45/10 | Focus timer with audio alert |
| Life hierarchy | Health → Family → Work → Admin → Hobbies |
| System guide | Keep → Tasks → Claude → Calendar flow |
| Stuck protocol | 3-step unblocking modal |
| Offline | Works after first load via Service Worker |
| PT/EN | Language toggle, persisted in localStorage |

## Install on iPhone

1. Open the demo URL in **Safari**
2. Tap **Share → Add to Home Screen**
3. Opens fullscreen, no browser chrome

## How it fits into the system

```
Google Keep      → quick idea capture (mobile)
Google Tasks     → single source of truth for tasks
Claude Desktop   → reads Tasks, plans day, creates calendar blocks
Google Calendar  → confirmed focus blocks
ADHD Flow        → morning read + focus tools
```

Claude Desktop with the "Claude in Chrome" connector reads your actual Tasks, reasons through priorities (Eisenhower + energy level), and creates Calendar blocks — one conversation, no copy-paste.

## Customize

Everything lives in `index.html`:

- `CONTENT.pt.mantras` / `CONTENT.en.mantras` — your phrases
- `CONTENT.pt.checklist` / `CONTENT.en.checklist` — your morning routine
- "Guide" tab — your ADHD strategies
- "System" tab — your tool flow

## Stack

Vanilla HTML/CSS/JS. No build, no framework, no dependencies.

- Service Worker (offline)
- localStorage (daily checklist state)
- Web Audio API (Pomodoro alert)
- Clipboard API (copy prompts)

~1 file, ~33KB.

## License

MIT. If it helps someone, mission accomplished.
