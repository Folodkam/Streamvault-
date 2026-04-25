# StreamVault Website

This folder is a static GitHub Pages website for StreamVault.

## Files

- `index.html` is the main landing page.
- `styles.css` contains the full responsive design.
- `assets/streamvault-icon.png` is the app icon.
- `assets/hero-backdrop.png` is the hero artwork.
- `downloads/latest.yml` mirrors the latest installer metadata.

## Publish With GitHub Pages

1. Push this `docs` folder to your GitHub repository.
2. In GitHub, open `Settings > Pages`.
3. Set the source to your main branch and the `/docs` folder.
4. Save, then wait for GitHub to publish the site.

## Download Button

The download button currently points to:

```text
downloads/StreamVault-Setup-1.5.0.exe
```

The latest installer built locally is:

```text
C:\Users\Mr.Man\Downloads\StreamVault_v3\streamvault\dist\StreamVault-Setup-1.5.0.exe
```

That installer is `108,480,969` bytes, which is over GitHub's normal 100 MB file limit.

Recommended release setup:

1. Create a GitHub Release.
2. Upload `StreamVault-Setup-1.5.0.exe` as a release asset.
3. Change both download links in `index.html` to:

```text
https://github.com/YOUR_USERNAME/YOUR_REPO/releases/latest/download/StreamVault-Setup-1.5.0.exe
```

Alternative setup:

Use Git LFS, then place the installer at:

```text
docs/downloads/StreamVault-Setup-1.5.0.exe
```

With that layout, the current download button works without changing `index.html`.
