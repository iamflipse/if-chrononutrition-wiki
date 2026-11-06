# Chrononutrition & Intermittent Fasting Wiki

A curated wiki distilling:

> Ma M, Yuan J, Xu F, Zhou Y, Li T, Zhou D and Zhang X (2026). "Chrononutritional regulation of metabolic homeostasis: intermittent fasting through gut microbiota, circadian rhythms, and autophagy." *Front. Nutr.* 13:1964828. doi: [10.3389/fnut.2026.1964828](https://doi.org/10.3389/fnut.2026.1964828)

**Public copy:** https://iamflipse.github.io/if-chrononutrition-wiki/ (read-only; static build served from the `gh-pages` branch)

## Layout

- `src/` — wiki pages as markdown (`index.md`, `about.md`, `concepts/`, `sources/`)
- `book/` — mdbook-generated static site (committed for GitHub Pages)
- `tools/mdbook` — mdbook v0.4.21 binary (aarch64 Linux, built from source)

## Rebuild + republish

```sh
./tools/mdbook build -d book
git add -A && git commit -m "update" && git push origin main
# republish gh-pages: check out orphan branch, move book/* to root, force push
```
