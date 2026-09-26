# Media files

Add these files to this directory:

- `teaser.mp4` — short overview video used near the top of the page
- `result-01.mp4`, `result-02.mp4`, `result-03.mp4` — carousel results
- `comparison.mp4` — side-by-side qualitative comparison

Recommended encoding for browser playback:

```bash
ffmpeg -i input.mp4 -c:v libx264 -crf 22 -preset slow \
  -pix_fmt yuv420p -movflags +faststart -an output.mp4
```

Keep individual files reasonably small. GitHub warns about files above 50 MB and
blocks ordinary Git files above 100 MB. Consider compressed clips, Git LFS, or
external video hosting for large assets.
