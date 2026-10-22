# JobPilot

**Download page: https://akshayan03.github.io/jobpilot/**

JobPilot is a Mac app that reads a job posting, checks whether you fit, writes a tailored one-page resume and cover letter from your real experience, fills in the application, and stops so you can review it and press Submit yourself.

This repository hosts the download page (`index.html`, `assets/`) and the macOS builds ([Releases](https://github.com/Akshayan03/jobpilot/releases)). The app's source code isn't public.

## Download

| Mac | File |
|---|---|
| Apple silicon (M1 and later) | [JobPilot-mac-arm64.dmg](https://github.com/Akshayan03/jobpilot/releases/latest/download/JobPilot-mac-arm64.dmg) |
| Intel | [JobPilot-mac-x64.dmg](https://github.com/Akshayan03/jobpilot/releases/latest/download/JobPilot-mac-x64.dmg) |

Each release lists the files' SHA-256 checksums (`SHA256SUMS.txt`). Check yours with `shasum -a 256 ~/Downloads/JobPilot-mac-*.dmg`.

## You need

- macOS 13 Ventura or later
- A Claude Pro or Max subscription, with [Claude Code](https://claude.com/product/claude-code) installed and signed in (`curl -fsSL https://claude.ai/install.sh | bash`, then `claude auth login`). JobPilot checks this when it opens.
- Python 3 (if macOS offers to install the command line developer tools the first time you build a resume, say yes)

## First launch

JobPilot isn't notarized by Apple, so macOS asks you to confirm it once: open it, click **Done**, then go to System Settings → Privacy & Security and click **Open Anyway** next to "JobPilot was blocked". The download page shows each step.

## Privacy

Everything stays on your Mac (`~/Library/Application Support/JobPilot`). There's no JobPilot server, account or analytics. Writing goes through Claude Code on your Mac, under your own Claude account.

## Review-first

JobPilot never submits an application for you, never invents employers, dates, titles or numbers, never answers work authorization, sponsorship, self-identification or legal questions you haven't answered yourself, and never automates LinkedIn or solves CAPTCHAs.

## License

All rights reserved; free to download and use. See [LICENSE](LICENSE).
