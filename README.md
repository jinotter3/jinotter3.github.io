# Seonghyun Jin Personal Website

Static GitHub Pages site for `https://jinotter3.github.io/`.

## Edit Before Publishing

- Replace `assets/profile.jpg` with your profile image. The page falls back to `assets/profile-placeholder.svg` until this file exists.
- Add your CV at `assets/Seonghyun_Jin_CV.pdf`.
- Replace the CRePE placeholder once the arXiv page is live.

## Publish

```bash
cd /home/jin/dev/ECCV2026/jinotter3.github.io
git init
git add .
git commit -m "Initial personal website"
git branch -M main
git remote add origin https://github.com/jinotter3/jinotter3.github.io.git
git push -u origin main
```
