# cleat-site

The marketing and documentation site for [Cleat](https://github.com/cleat-lang/cleat) — a compiled orchestration language for auditable, safe AI agents. Reflects the **v0.1.1-alpha** release: eight compiler-enforced primitives (`agent`, `guard`, `tool`, `stream`, `state`, `chain`, `server`, `fn`), 826 tests, 15 stdlib packages, 29 example programs.

## Structure

Plain static HTML. No build step. No framework.

- `index.html` — landing page
- `why.html` — comparisons vs LangGraph, Temporal, Python + Pydantic
- `docs.html` — documentation
- `examples.html` — examples gallery
- `blog.html` — blog index
- `changelog.html` — release notes
- `sponsor.html` — sponsorship tiers
- `404.html` — not found (Cleat-style diagnostic)

## Source of truth

The canonical description of the language lives in the main repo's [README](https://github.com/cleat-lang/cleat#readme). When content drifts between the two, the language README wins — this site is a rendered view, not the spec.

## Local preview

```bash
python3 -m http.server 8000
# open http://localhost:8000
```

Or any static server will do — no build step, no dependencies.

## Deploying

Auto-deploys to Cloudflare Pages on every push to `main`.

## License

Site content: MIT. Code samples on the site are illustrative and match the compiler in the main repo at tag `v0.1.1-alpha`.
