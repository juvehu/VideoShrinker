# Video Shrinker

A single-page tool that re-encodes videos to a smaller resolution and file size directly in the browser, using the WebCodecs API. Nothing is uploaded; files stay on your computer.

**Live:** https://juvehu.github.io/VideoShrinker/

## Features

- Drop several MP4 / MOV / M4V files at once; each shows its resolution, codec, frame rate, length, size and bitrate
- Output resolution by short side: Original, 1080p, 720p, 540p, 480p (portrait clips handled)
- Size by **target MB** (default 12 MB, under WhatsApp's ~16 MB re-compression limit) or by quality level
- H.264 output using the browser's hardware encoder where available
- Remove-audio option; otherwise AAC/Opus audio is copied unchanged
- Editable output file name, preview player, per-file Download and **Download all**
- **Drag to folder** (Chrome/Edge) and an **output folder** that converted files save into automatically (Chrome/Edge)

## Use offline

`index.html` is fully self-contained. Download it and open it locally in Chrome, Edge or Safari.

## Third-party code (embedded)

- [mp4box.js](https://github.com/gpac/mp4box.js) 0.5.2 — BSD-3-Clause
- [mp4-muxer](https://github.com/Vanilagy/mp4-muxer) 5.1.3 — MIT
