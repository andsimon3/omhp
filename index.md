# Open Media Host Protocol

Open Media Host Protocol (OMHP) is a specification for hosting, discovering, and streaming media
over HTTP-compatible endpoints.

## What is this?

OMHP defines a small set of endpoints that any media host can implement:

- **Manifests** — a single document describing available renditions and their locations.
- **Segments** — immutable, byte-addressable chunks of media referenced by the manifest.
- **Discovery** — resolving a media id to its current manifest URL.

## Project status

| Stage       | Status  |
| ----------- | ------- |
| Draft       | Current |
| First draft | 2026    |

> The specification is a work in progress. Sections may change between revisions.

## Conventions

Examples in this documentation use `https://media.example.com` as the default host:

```http
GET /v1/manifests/42 HTTP/1.1
Host: media.example.com
Accept: application/vnd.omhp.manifest+json
```

## License

Documentation in this project is licensed under
[Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).
The full license text is in the `LICENSE` file at the root of this project.
