# Discord Message Editor

A browser-based WYSIWYG editor for composing Discord messages with live preview, formatting tools, timestamp generation, and spell checking.

**Live site:** [gatekeeperdev.github.io/discord-wysiwyg](https://gatekeeperdev.github.io/discord-wysiwyg)

## Features

- **Formatting toolbar** — Bold, italic, underline, strikethrough, inline code, code blocks, spoilers, block quotes, headings (H1–H3), bullet and numbered lists
- **Keyboard shortcuts** — Ctrl/Cmd+B (bold), Ctrl/Cmd+I (italic), Ctrl/Cmd+U (underline)
- **Live preview** — See how your message will render in Discord as you type
- **Character counter** — Tracks the 2000-character Discord limit with a progress bar (yellow at 90%, red when over)
- **Timestamp generator** — Pick a date/time or enter a Unix timestamp, then insert Discord timestamp codes in any format (`<t:TIMESTAMP>`, `<t:TIMESTAMP:R>`, etc.)
- **Spell checker** — Toggle spell checking to flag potentially misspelled words (loads a local dictionary)
- **Copy to clipboard** — One-click copy from the toolbar

## Supported Discord Markdown

| Syntax | Result |
|--------|--------|
| `**text**` | **Bold** |
| `*text*` | *Italic* |
| `__text__` | Underline |
| `~~text~~` | ~~Strikethrough~~ |
| `\|\|text\|\|` | Spoiler |
| `` `code` `` | Inline code |
| ` ```code``` ` | Code block |
| `> text` | Block quote |
| `# H1` / `## H2` / `### H3` | Headings |
| `<t:TIMESTAMP:FORMAT>` | Dynamic timestamp |

## Timestamp Formats

| Code | Style | Example |
|------|-------|---------|
| `<t:1234567890>` | Default | November 28, 2018 9:30 PM |
| `<t:1234567890:t>` | Short Time | 9:30 PM |
| `<t:1234567890:T>` | Long Time | 9:30:00 PM |
| `<t:1234567890:d>` | Short Date | 11/28/2018 |
| `<t:1234567890:D>` | Long Date | November 28, 2018 |
| `<t:1234567890:f>` | Short Date/Time | November 28, 2018 9:30 PM |
| `<t:1234567890:F>` | Long Date/Time | Wednesday, November 28, 2018 9:30 PM |
| `<t:1234567890:R>` | Relative | 3 years ago |

## Tech

Single `index.html` file with no dependencies — runs entirely in the browser. Hosted on GitHub Pages.
