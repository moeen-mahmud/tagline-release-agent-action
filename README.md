# tagline-release-agent-action

> **This is a build-artifact repository.** The bundled action code lives here so consumers can pin it from their workflows. The source, documentation, and issue tracker live upstream in **[HelicanHQ/tagline-sh](https://github.com/HelicanHQ/tagline-sh)**.

A full version-aware README is published automatically with each release. Until the first stable release lands, please refer to [the upstream README](https://github.com/HelicanHQ/tagline-sh#readme) for setup, slash commands, and architecture.

## What lives in this repo

- **`action.yml`** — the GitHub Action manifest.
- **`dist/index.js`** — the bundled action code, rebuilt and pushed by upstream on every stable release.
- **`README.md`** — this file (replaced on each release with a version-pinned README).
- **`LICENSE`** — MIT.

These files are **never edited by hand** — they are produced and pushed by [`HelicanHQ/tagline-sh/.github/workflows/release.yml`](https://github.com/HelicanHQ/tagline-sh/blob/main/.github/workflows/release.yml). Please contribute upstream, not here.

## Quick reference

```yaml
- uses: HelicanHQ/tagline-release-agent-action@v1
  with:
      github-token: ${{ secrets.GITHUB_TOKEN }}
```

For the full workflow + install steps, see the [upstream getting-started guide](https://github.com/HelicanHQ/tagline-sh#readme).

## License

MIT — identical to the [upstream license](https://github.com/HelicanHQ/tagline-sh/blob/main/LICENSE).
