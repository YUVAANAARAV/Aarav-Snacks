Video gallery — quick run & troubleshooting

This repo contains `video.html`, a static gallery that expects your video files to be present locally.

Quick test (recommended):
1. Open PowerShell in the repository root (c:\Users\Aarav Gupta\code\Aarav-Snacks).
2. Run a tiny HTTP server so browsers reliably load media:

```powershell
# Python 3
python -m http.server 8000
```

3. Open http://localhost:8000/video.html in your browser.

Notes & tips:
- The page will try to find files in `videos/` (videos/<name>.mp4) and also in the repo root (<name>.mp4). If files are missing youll see a diagnostic message under each card and a banner at the top.
- If your files use other extensions (.mov, .mkv) you can rename them to .mp4 or re-encode to .mp4/.webm for broad browser compatibility.
- For mobile testing, run the HTTP server on your PC and open http://<your-pc-ip>:8000/video.html on the phone (on the same Wi‑Fi network). Example: http://192.168.1.25:8000/video.html

If you'd like, I can:
- Move found mp4 files into a `videos/` folder for you (confirm before I modify files).
- Add poster thumbnails and graceful fallbacks for missing videos.
- Add an auto-enumeration server script that serves a JSON manifest and a nicer dynamic page.

Tell me what you'd like next.