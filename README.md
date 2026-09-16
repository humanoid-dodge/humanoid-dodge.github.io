# Humanoid Dodgeball

Anonymous project website for **Humanoid Dodgeball: Learning Fast Dynamic Obstacle Avoidance Motions for Humanoids**.

## Edit the page

- `index.html`: title, subtitle, anonymous author, overview figure and video section.
- `style.css`: colors, typography, header, cards and responsive video layout.
- `figs/humanoid-dodgeball-overview.png`: overview figure.
- `assets/videos/`: add your own video files here.

## Add videos

1. Copy your clips into `assets/videos/`.
2. Find `<section id="videos"` in `index.html` and remove its `hidden` attribute.
3. Uncomment the example `<figure class="video-card">` block inside `.video-grid`.
4. Replace `your-video.mp4` with the clip's filename and write its caption.
5. Duplicate the card for additional clips. Cards appear in two columns on desktop and one on mobile.

The sample card is commented out so the empty template loads no missing videos.

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
