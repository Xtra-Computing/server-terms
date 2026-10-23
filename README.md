# Xtra Computing Server Docs

Terms of use and user guides for the Xtra Computing Server, built with
[Material for MkDocs](https://squidfunk.github.io/mkdocs-material/).

Site: https://xtra-computing.github.io/xtra-server-terms-mkdocs/

Content is migrated from [Xtra-Computing/xtra-server-terms](https://github.com/Xtra-Computing/xtra-server-terms).

## Local preview

```bash
pip install -r requirements.txt
mkdocs serve
```

## Editing

- Pages live in `docs/`. English is `foo.md`, Chinese is `foo.zh.md`
  (a page without a `.zh.md` falls back to English).
- New pages must be added to `nav` in `mkdocs.yml`.
- Push to `main` deploys to GitHub Pages via `.github/workflows/deploy.yml`.

## Adding a server notice

1. Copy [templates/news.md](templates/news.md) to
   `docs/news/YYYY-MM-DD-short-slug.md`, using the date the notice was sent.
2. If the notice was also sent in Chinese, add
   `docs/news/YYYY-MM-DD-short-slug.zh.md`. The site provides the language switcher.
3. Add the notice to both `docs/news/index.md` and `docs/news/index.zh.md`,
   newest first. Use the English `.md` filename in links in both indexes;
   the language plugin resolves the translated page.
4. Add the English path under `News` in `mkdocs.yml`, and the Chinese label
   under `nav_translations`.
5. If the notice changes policy, update the Terms of Use in the same commit.
6. Run `mkdocs build --strict` before publishing.

Do not put credentials, internal addresses, or individual users' names or
usage data in a notice — this repository is public.
