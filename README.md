# YouTube Toolkit 🎬

**10 free tools for YouTube creators. No signup. No backend. Everything runs in your browser.**

Built because I kept switching between 5 different websites while making YouTube content. Mainly needed a thumbnail previewer and a deeplink generator that actually opens the YouTube app instead of Instagram's terrible in-app browser.

🔗 **Live site:** [youtubekit.vercel.app](https://youtubekit.vercel.app)

---

## Tools

| Tool | What it does |
|---|---|
| 🖼️ **Thumbnail Previewer** | See your thumbnail on Home, Search, Recommendations and End Screen across Desktop, Tablet and Mobile. Dark and light mode. Shuffle position. |
| 🆚 **A/B Thumbnail Tester** | Upload two thumbnails, get an automatic score and winner based on title length, power words, CTR signals |
| 🎨 **Color Palette Extractor** | Extract dominant HEX colors from your thumbnail for consistent channel branding |
| 📺 **Channel Art Previewer** | Preview your banner with safe zone marked across Desktop, Tablet, TV and Mobile |
| 📱 **Shorts Previewer** | See how your Short looks on the mobile player and home feed card |
| ✅ **Upload Checklist** | 30-point SEO checklist before you hit publish |
| 🔗 **Deeplinks Generator** | Generate a Smart Link that opens the YouTube app on Android and iOS, and falls back to YouTube.com on desktop. Perfect for Instagram Stories. |
| 🔍 **Video SEO Audit** | Paste your video URL, auto-fetches the title, scores your SEO across 12 criteria |
| 📊 **Channel Audit** | Rate your channel on branding, consistency, upload frequency, playlists and more |
| ⬇️ **Thumbnail Downloader** | Paste any YouTube URL and download thumbnails in all available sizes |

---

## The Deeplink Problem

When you share a YouTube link in your Instagram Story, it opens inside Instagram's in-app browser. Viewers are not logged into YouTube there, so they cannot like, subscribe or comment without extra steps. Engagement drops to near zero.

YouTube Toolkit generates a **Smart Link** that detects the device:

```
Android  →  intent:// fires  →  YouTube app opens directly
iOS      →  vnd.youtube:// fires  →  YouTube app opens directly  
Desktop  →  redirects to youtube.com normally
```

One link. Works for everyone.

---

## How it works

The entire app is two static HTML files. No framework. No build step. No dependencies to install.

- `index.html` — the full toolkit (10 tools)
- `go.html` — the deeplink redirect handler

Everything runs in the browser. Images never leave your device. No data is collected.

---

## Run locally

Just download and open `index.html` in your browser. That is it.

```bash
git clone https://github.com/UtsavCodesZero/youtube-toolkit.git
cd youtube-toolkit
# Open index.html in your browser
```

Note: The Smart Link deeplinks only work after deploying to a live URL (Vercel, Netlify, etc.) since they need a public address to redirect from.

---

## Deploy

```bash
# Push to GitHub, then import on Vercel
# No settings needed — just deploy as a static site
```

The Smart Link in the Deeplinks Generator will automatically use your deployed domain.

---

## Tech stack

| Layer | Technology |
|---|---|
| Frontend | HTML, CSS, Vanilla JavaScript |
| Fonts | Google Fonts (Geist) |
| Thumbnail fetch | YouTube oEmbed API (public) |
| Thumbnail images | YouTube CDN (public) |
| Hosting | Vercel (free tier) |

No frameworks. No build step. No npm. No node_modules.

---

## Also built by me

[**I Love CV**](https://ilovecv.vercel.app) — Free resume builder, 5 templates, ATS score checker, PDF and DOCX export. No signup, no watermark.

---

## Support

YouTube Toolkit is completely free and always will be. If it helped you, consider supporting via eSewa:

**eSewa:** `9823418816`

---

## License

MIT — free to use, modify and share.

---

Built with ❤️ from Kathmandu, Nepal.
