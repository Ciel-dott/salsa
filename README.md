# SALSA project page

## How to put it online (GitHub Pages)

1. Drop your 14 mp4 files into `clips/` using the exact names in `clips/PUT-VIDEOS-HERE.txt`
   (spaces -> hyphens). Compress each to UNDER 25 MB so the GitHub web uploader accepts it:
   ffmpeg -i in.mp4 -vf scale=-2:720 -c:v libx264 -crf 28 -an clips/out.mp4
2. Open index.html and replace the placeholder arXiv link (search "arxiv") with your real link.
3. On GitHub: New repository (PUBLIC). Then Add file -> Upload files -> drag in EVERYTHING
   in this folder (index.html, all salsa_*.html, and the clips/ folder) -> Commit.
4. Repo Settings -> Pages -> Source: Deploy from a branch -> Branch: main, folder: / (root) -> Save.
5. Wait ~1-2 min; the URL appears at the top of the Pages settings:
   https://<your-username>.github.io/<repo>/   <- share this link.

Notes
- Host THIS (linked) index.html, not the single-file standalone (videos can't be embedded).
- The bottom montage strip plays 9 short clips live; if it's heavy on mobile, tell me and
  we can switch to poster images or fewer clips.
- Filenames with spaces will NOT load on the web — keep them hyphenated as listed.
