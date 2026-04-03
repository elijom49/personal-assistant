# Agents

## Skill routing

| If the request is about... | Use skill |
|---|---|
| Work email, inbox, outreach | executive-assistant |
| Personal email, non-work inbox | personal-assistant |
| Calendar, scheduling, availability | executive-assistant |
| Task list, today's priorities | daily-task-manager |
| Morning briefing | daily-task-prep |
| Shopping, errands, groceries | personal-assistant |
| Habits, fitness, streaks | personal-assistant |
| Custom reminders | personal-assistant |
| Pre-meeting context | meeting-prep |
| Drafting any email | email-drafter |
| Project status, blockers | project-tracker |
| Meeting notes, action items | meeting-notes |

## Handoff rules

- Skills can read any workspace file but only write to files in their domain
- If a task spans two skills, complete the first then trigger the second
- Never delete items from task list, shopping list, or reminder files — mark done instead
