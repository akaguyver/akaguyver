
# Hi there

I build practical software that solves real problems, and I test it on the hardware it has to run on.

## Featured project: Sortovia

**[Sortovia](https://github.com/sortovia/sortovia)** is a free add-on for Kodi that turns a pile of downloads into a tidy library that Kodi can read. It shows the full plan first, and nothing moves until you approve it.

I built it to manage a large media library on an Xbox, using only an Android phone, with no PC available.

- About 21,000 lines of Python, with over 500 automated tests that run against a simulated Kodi
- An Android companion app in Java (about 18,000 lines), with a DJ deck screen and its own audio engine, plus phone tools that share files over Wi-Fi
- Automatic updates verified by checksum, and sorts that can resume if Kodi closes
- Optional passcode encryption for saved passwords, and a problem-report tool that removes private details from logs before anyone sees them

The [engineering notes](https://github.com/sortovia/sortovia/blob/main/DEVELOPMENT.md) explain the design, including the Xbox behaviour I had to find by reading real device logs. For example, renames always fail on its removable drives, and a missing file reports a size of 0 instead of an error.

I built Sortovia with [Claude Code](https://claude.com/claude-code), an AI coding tool, as a development partner. I set the direction, tested it on real hardware, and drove the fixes from what I found.

## Skills

Python · Java · Android · Bash · Git and GitHub Actions · Kodi add-ons · WebDAV · automated testing

