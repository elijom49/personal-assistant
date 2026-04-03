# personal-assistant

A personal + professional AI assistant for people who want one agent to run both their work and personal life.

> Built on the conventions established by [clawchief](https://github.com/snarktank/clawchief) by Ryan Carson. This template extends the original with personal life management, meeting prep, email drafting, project tracking, and meeting notes.

## Requirements

- OpenClaw installed and working
- `gog` working for Gmail, Google Calendar, and Google Sheets

## Install steps

1. Clone this repo
2. Copy skills into OpenClaw: `cp -r skills/* ~/.openclaw/skills/`
3. Copy workspace files: `cp -r workspace/* ~/.openclaw/workspace/`
4. Fill in `workspace/USER.md`
5. Replace all `[PLACEHOLDER]` values in workspace files
6. Create Google Sheets for outreach, habits, and projects
7. Copy cron template: `cp cron/jobs.template.json ~/.openclaw/cron/jobs.json`
8. Verify: try "Check my inbox", "What's on my calendar today?", "Add milk to my shopping list"

## Placeholder reference

| Placeholder | Replace with |
|---|---|
| `[USER_NAME]` | Your name |
| `[WORK_EMAIL]` | Your work email |
| `[PERSONAL_EMAIL]` | Your personal email |
| `[USER_TIMEZONE]` | e.g. America/New_York |
| `[USER_CITY]` | Your city |
| `[CALENDAR_IDS]` | Comma-separated Google Calendar IDs |
| `[OUTREACH_SHEET_ID]` | Google Sheet ID for outreach |
| `[HABITS_SHEET_ID]` | Google Sheet ID for habits |
| `[PROJECTS_SHEET_ID]` | Google Sheet ID for projects |
| `[HABIT_1]`, `[HABIT_2]`, `[HABIT_3]` | Your habit names |

## Skills

| Skill | Purpose |
|---|---|
| executive-assistant | Work inbox triage, calendar, scheduling |
| daily-task-manager | Task list management |
| daily-task-prep | Morning briefing cron |
| personal-assistant | Personal inbox, shopping, habits, reminders |
| meeting-prep | Pre-meeting briefs |
| email-drafter | Draft emails in your voice |
| project-tracker | Project status and weekly review |
| meeting-notes | Capture notes, decisions, action items |

## Private files — do not commit

- `workspace/USER.md`
- `workspace/MEMORY.md`
- `workspace/memory/`
- `workspace/meeting-notes/`

## Troubleshooting

- **Morning briefing not running** — test manually: "Run daily task prep"
- **Calendar not accessible** — verify Calendar IDs and gog permissions
- **Work/personal email mixing** — check WORK_EMAIL and PERSONAL_EMAIL in IDENTITY.md
- **Habits not logging** — confirm HABITS_SHEET_ID and column headers match habit names
