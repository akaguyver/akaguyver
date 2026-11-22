<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="assets/banner-black.png">
    <source media="(prefers-color-scheme: light)" srcset="assets/banner-white.png">
    <img alt="akaguyver: honeycomb logo with trend bot, notebook transcriber, Sortovia, Xbox apps, DJ and home automation icons" src="assets/banner-white.png" width="100%">
  </picture>
</p>

## About me

Designing and engineering solutions you can count on. I bring a builder's mindset from years of carpentry, trim and cabinets, low voltage and home automation to software: plan it right, build it solid and make it work every time.

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

## More projects

### Notebook Transcriber
A phone web app that turns handwritten lyric notebooks into searchable, reusable lines. Photograph a page, AI transcribes it, and you review it line by line against the handwriting.

- **AI transcription** of notebook photos, with line-by-line review beside the original page: fix, split and join lines, add notes and keep alternate versions
- **Rhyme analysis** from the CMU Pronouncing Dictionary: perfect rhymes, rap-style slant rhymes and multi-word rhymes, with handling for slang and the writer's own spellings
- **Matching bars across ideas:** cuts every notebook into rhyming 2–4 bar sets, sorted by style, so like bars from different ideas and pages can be put together
- **Song compilation:** build songs from whole ideas or single lines pulled from anywhere, and reuse one line in several songs
- **Recommended edits:** automatic proofreading (rhyme partners far apart in syllables, near rhymes) plus suggested rewrites, saved as alternate versions so the original wording is never lost
- **Line ideas:** ask for new versions of a line, or a new line to follow it
- **Held notes:** mark syllables to hold, with beat counts
- **Tags** for genres, uses and themes, with AI-suggested tags you keep or drop
- **Export and backup:** download every line and photo as a zip, plus private backups

### Idea Ladder (business idea transcriber)
A private phone web app that turns handwritten business ideas into a ranked plan of what to start first.

- **Photo transcription:** photograph idea pages, Claude reads them, and you check each line against the photo
- **Learns from corrections:** keeps a list of commonly misread words to improve future reads
- **Business models:** drafts a short business model for every idea
- **The ladder:** ranks ideas by what you can start with the resources you have today, and re-ranks when your resources change
- **Deep dives:** web research on the ideas you choose, sending only that idea's text
- **Two built-in chats:** "Ask Claude" works only with your own data and never posts, contacts anyone or spends money; "Change the app" edits the app's own code and runs its tests
- **Private by design:** runs on the phone only, with backups to a private repo

### Trend Bot
A Python crypto trading platform: build strategies, backtest them, paper trade and go live, all from a TradingView-style chart on the phone.

- **Strategy builder:** combine entry triggers, filters on any timeframe and exits (ATR stop, trailing stop, take-profit, opposite signal), then save, load and paper trade your strategies
- **Multiple indicators at once:** 14 chart indicators with adjustable settings, including line-by-line Pine Script ports that match TradingView (Zeiierman Trend Speed Analyzer, LuxAlgo Range Detector, KhanSaab Sniper), plus EMA, Supertrend, RSI, ADX, VWAP, Bollinger/Keltner squeeze, Donchian channels and AI indicators
- **Backtesting:** bar by bar with fees, slippage, maker orders, funding, borrow costs and liquidation; tested to never use future prices; walk-forward tests on data the settings never saw; side-by-side mode comparisons and parameter sweeps
- **Exchange trading:** charts, backtests and paper trading on 17 exchanges, and live trading through exchange APIs with trade-only keys and a typed confirmation
- **DEX and wallet trading:** swaps from your own wallet, with MetaMask-style wallets on Uniswap (Base, Arbitrum, Ethereum) and Phantom wallets on Jupiter (Solana), plus swap-only safety checks, per-trade caps and slippage limits
- **Wallet view:** read-only balances across your exchanges and wallets
- **Paper and live bots** running in the background, several at once, each with its own account and trade log
- **Mobile chart:** exchange and market picker, watchlist, drawing tools (trend lines, channels, Fibonacci, risk:reward), light and dark modes
- **Alerts:** price levels, crosses of lines you draw, and strategy position changes, with Android notifications
- **Extras:** leveraged token (3x/5x) backtests, venue rules by country, TradingView CSV comparison and a guide for converting your own Pine indicators

### Sortovia Playlist (in progress)
A web app that keeps your playlists in sync across streaming services. Spotify and Tidal come first, with Deezer, YouTube and SoundCloud support in progress.

- Smart track matching, with a review step for uncertain matches (like live or remix versions)
- Two-way sync, including removals, with a guard that asks before large deletions
- Scheduled syncs, encrypted service logins, and safe recovery if a sync is interrupted

### DJ / Turntables
The Sortovia Android app (APK) includes a full-featured turntable with automix that uses real DJ-style transitions. It also has genre lookup from multiple sources, a full tag editor, phrase analysis, beatgrid editing, key detection and export to a Rekordbox XML file.

### Xbox Apps
More native Xbox apps planned.

### Home Automation
Building open-source home automation tools and voice control integration to use one seamless interface to control every smart device in your home. Using Arduino, Raspberry Pi and custom-built control hardware to make your life easier.

## Skills

Python · Java · Android · Bash · Git and GitHub Actions · Kodi add-ons · WebDAV · automated testing
