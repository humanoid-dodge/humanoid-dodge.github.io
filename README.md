# Humanoid Dodgeball

Anonymous project website for **Humanoid Dodgeball: Learning Fast Dynamic Obstacle Avoidance Motions for Humanoids**.

## Edit the page

- `index.html`: title, subtitle, anonymous author, overview figure and video section.
- `style.css`: colors, typography, header, cards and responsive video layout.
- `figs/humanoid-dodgeball-overview.png`: overview figure.
- `assets/videos/`: add your own video files here.

## Add videos

1. Copy your clips into `assets/videos/` using browser-compatible MP4 files (H.264 video and AAC audio).
2. Find `<section id="videos"` in `index.html`.
3. Duplicate its `<figure class="video-card">` block for each new clip.
4. Update the source and fallback download paths, dimensions, and accessible label. Add a `<figcaption>` if needed.

A single video spans the full width. Multiple videos appear in two columns on desktop and one on mobile.
Playback starts when the viewer presses Play, with audio enabled.

The current video is `assets/videos/ICRA_video_web.mp4`, optimized for browser playback with the playback metadata at the start of the file.
The original `ICRA_video_final.mp4` is retained locally and excluded from Git because it exceeds GitHub's 100 MiB file limit.

## Preview locally

Run this from the repository directory:

```bash
python3 -m http.server 8000 --bind 127.0.0.1
```

Open http://localhost:8000, then refresh after saving edits. Press Ctrl+C to stop the server.

## Publish

Push changes to `main`; the existing GitHub Pages workflow publishes the site at https://humanoid-dodge.github.io/.

## Template credits

The visual template was adapted from the [PolaRiS website](https://github.com/polaris-evals/polaris-evals.github.io), whose original README credits VideoMimic.
