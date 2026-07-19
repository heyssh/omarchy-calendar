# omarchy-calendar

A month-view calendar with per-day notes for [Omarchy](https://github.com/basecamp/omarchy).

## Features

Click the calendar icon in the bar and a month view pops up — click it again to close it. Pick any day to see its notes, add a new one, or remove any note with its × — each day keeps its own list, so nothing gets mixed up between dates, and everything's saved locally to `~/.local/state/ssh.calendar/notes.json`. Days that have notes get a small dot under the day number, so you can spot them at a glance without opening each one. The grid always shows six full weeks, so the panel stays the same size whether you're looking at February or a five-week month. A small WEEK/NOTES readout up top gives you a bit of context — which week of the year you're on, how many notes the month has — without having to count anything yourself. `‹ Today ›` buttons step between months or jump straight back to the current one.

This plugin only adds its own bar icon — it doesn't modify Omarchy's built-in `Clock` widget or any other core file.

## Configuration

The week start day (Monday vs. Sunday) is auto-detected from your system locale, so it should already match what you're used to. To override it, add `"weekStart"` to this plugin's entry in `~/.config/omarchy/shell.json`:

```json
{ "id": "ssh.calendar", "weekStart": "sunday" }
```

## Install

```bash
omarchy plugin add https://github.com/heyssh/omarchy-calendar.git
omarchy plugin enable ssh.calendar
omarchy bar plugin add ssh.calendar
```

Or by hand: drop this repo into `~/.config/omarchy/plugins/ssh.calendar/`,
then `omarchy plugin rescan`, `omarchy plugin enable ssh.calendar`,
`omarchy bar plugin add ssh.calendar`.

## Update / remove

```bash
omarchy plugin update ssh.calendar
omarchy plugin remove ssh.calendar
```

## License

MIT — see [LICENSE](LICENSE).
