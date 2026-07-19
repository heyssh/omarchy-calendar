# omarchy-calendar

Month-view calendar with per-day notes for [Omarchy](https://github.com/basecamp/omarchy).

## Features

- Month grid (fixed 6×7 so the popup never resizes between short and
  long months)
- Click any day to select it; notes are scoped per day
- Add / remove notes for the selected day, saved to
  `~/.local/state/ssh.calendar/notes.json`
- WEEK / NOTES stats for quick context on the selected week and month
- Its own bar icon — click to open, click again to close

## Keyboard shortcuts

Inside the panel:

- `h` / `j` / `k` / `l` or arrows: move selection by day / week
- `enter` / `space`: focus the note input
- `x`: remove the last note for the selected day
- `t`: jump to today
- `[` / `]`: previous / next month
- `tab`: switch to the next panel
- `esc`: close

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
