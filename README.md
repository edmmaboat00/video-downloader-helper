# Video Downloader Helper

A small Windows app for the **Video Downloader** browser extension (Chrome, Edge, Brave and Firefox).

The extension finds the videos on a page. The helper saves the ones a browser can't save by itself:

- YouTube videos and Shorts
- TikTok, Facebook, Instagram, X and Reddit posts
- full videos on sites that play them in pieces (HLS or DASH), joined into one MP4

It uses [yt-dlp](https://github.com/yt-dlp/yt-dlp), plus FFmpeg to join picture and sound.

## Download

**[Download the latest setup](https://github.com/edmmaboat00/video-downloader-helper/releases/latest/download/Video-Downloader-Helper-Setup.exe)** (about 30 MB, Windows 10 or 11).

Older versions and their checksums are on the [Releases](https://github.com/edmmaboat00/video-downloader-helper/releases) page.

## Install

1. Run `Video-Downloader-Helper-Setup.exe`. The setup is not code-signed, so Windows SmartScreen may warn you: click **More info → Run anyway**.
2. Click **Install**. No administrator rights are needed; it installs into `%LOCALAPPDATA%\Programs\Video Downloader Helper`.
3. Only if your PC lacks them, setup downloads Deno (needed for YouTube, about 41 MB) and FFmpeg (HD video and MP3, about 28 MB) from their official releases, and checks each against its published SHA-256 checksum.
4. Restart the browser. When the extension finds the helper, its **Install helper** banner disappears.

## Privacy

The helper runs only on your PC, started by the extension when you download something. It sends nothing to the extension's author. It connects to the sites you download from, and to GitHub to update yt-dlp at most once a week. Its download log (`download-log.jsonl`) stays in its install folder.

## Remove

Windows **Settings → Apps → Installed apps → Video Downloader Helper → Uninstall**.

## Third-party software

See [THIRD-PARTY-NOTICES.txt](THIRD-PARTY-NOTICES.txt).
