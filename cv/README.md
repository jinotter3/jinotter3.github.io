# CV Source

Edit `Seonghyun_Jin_CV.tex`, then rebuild the website PDF with:

```bash
cd /home/jin/dev/ECCV2026/jinotter3.github.io
latexmk -pdf -interaction=nonstopmode -halt-on-error -outdir=assets cv/Seonghyun_Jin_CV.tex
```

The homepage links to `assets/Seonghyun_Jin_CV.pdf`.
