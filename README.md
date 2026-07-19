# omarchy-calendar

Month-view calendar with per-day notes for [Omarchy](https://github.com/basecamp/omarchy).

## Features

Click the calendar icon in the bar and a month view pops up — click it again, or hit Esc, to close it. Pick any day to see its notes, add a new one, or clear the last one; each day keeps its own list, so nothing gets mixed up between dates, and everything's just saved locally to `~/.local/state/ssh.calendar/notes.json`. The grid always shows six full weeks, so the panel stays the same size whether you're looking at February or a five-week month. A small WEEK/NOTES readout up top gives you a bit of context — which week of the year you're on, how many notes the month has — without having to count anything yourself.

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
