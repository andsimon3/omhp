# Open Media Host Protocol

Diplodoc documentation project for the Open Media Host Protocol (OMHP) — a specification for
hosting, discovering, and streaming media over HTTP-compatible endpoints.

## Structure

```
.
├── src/
│   ├── .yfm      # Diplodoc project config
│   ├── toc.yaml  # Navigation table of contents
│   └── index.md  # First page (Overview)
├── LICENSE       # CC BY 4.0 full text
└── build/        # Build output (generated)
```

## Getting started

Requires Node 22+.

```bash
npm install       # install @diplodoc/cli
npm run build     # build docs to ./build
npm run dev       # build in watch mode
npm run preview   # serve ./build locally
```

## Adding pages

1. Create a Markdown file in `src/` (e.g. `src/quick-start.md`).
2. Add it to `src/toc.yaml`:

```yaml
items:
  - name: Overview
    href: index.md
  - name: Quick start
    href: quick-start.md
```

## License

Documentation is licensed under
[Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).
See the [LICENSE](LICENSE) file for the full text.
