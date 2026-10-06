# Tracy (Huiwen) Han — personal website

A single static page (`index.html`) served by GitHub Pages. No build step. The illustrations come from the Cabbageland art library (`~/cabbageland/cabbageland-art-library`).

## Editing

- **Bio**: the three paragraphs under `<!-- DRAFT BIO: edit freely -->` in `index.html`.
- **Highlights**: the `news-list` under "Highlights", newest first.
- **Publications**: one `<article class="pub-card">` per paper. Own name goes in `<u>…</u>`, `*` marks first or co-first author, and link buttons go in `pub-links`. Papers without a figure use a `thumb-placeholder` box; replace it with `<img src="imgs/publications/…">` once a figure is public.
- **Avatar**: `imgs/avatar.webp` (currently Cabbageclaw in a bow tie). Swap in a square photo of about 480 px.
- **CV**: `Tracy_Han_CV.pdf`, copied from `Tracy_Han_CV/cvs/cv6`. Re-copy after CV edits.

## Images

Images are WebP made with `cwebp`, for example:

```bash
cwebp -q 82 -resize 1200 0 figure.png -o imgs/publications/name.webp
```

## Preview locally

```bash
python3 -m http.server 8765
```

Then open <http://localhost:8765>.
