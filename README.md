# Academic project-page template

A dependency-free static project page inspired by the structure of modern computer
vision and graphics paper websites. It includes:

- paper title, venue, authors, affiliations, and resource links
- teaser video and concise project statement
- abstract and contribution summary
- method figure
- accessible result carousel
- qualitative comparison video
- copyable BibTeX
- responsive desktop/mobile layout

## Customize it

1. Edit the title, authors, links, abstract, and BibTeX in `index.html`.
2. Replace `assets/method-placeholder.svg` with your method figure. Keep the same
   filename or update the `<img>` path.
3. Add videos listed in `media/README.md`.
4. Change the colors at the top of `styles.css`.
5. Update the description and `<title>` in the document `<head>`.

Preview locally:

```bash
cd project-page-template
python3 -m http.server 8000
```

Open `http://localhost:8000`.

## Publish with GitHub Pages

### Dedicated project-page repository

1. Create a public repository, for example `paper-project-page`.
2. Copy the **contents** of this directory into the repository root.
3. Commit and push to the `main` branch.
4. In GitHub, open **Settings → Pages**.
5. Under **Build and deployment**, choose **Deploy from a branch**, then select
   `main` and `/ (root)`.

The URL will normally be:

```text
https://YOUR-USERNAME.github.io/paper-project-page/
```

All asset paths in this template are relative, so it works under a repository
subpath without configuration.

## Before publication

- Verify every author name, affiliation, and link.
- Include captions that explain what each result demonstrates.
- Compress images and videos, and test playback in Safari, Chrome, and Firefox.
- Obtain permission for all portraits, datasets, logos, and third-party media.
- Add alt text that describes the scientific content of each figure.
