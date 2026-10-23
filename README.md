# Xtra Computing Server Docs

[Terms, user guides, and server news](https://xtra-computing.github.io/server-terms/).

```bash
pip install -r requirements.txt
mkdocs serve
```

Edit pages in `docs/` (`foo.md` for English, `foo.zh.md` for Chinese) and navigation in `mkdocs.yml`.
For news, use [the template](templates/news.md) and update both archive indexes in `docs/news/`.
Run `mkdocs build --strict` to check changes; pushes to `main` deploy automatically.
