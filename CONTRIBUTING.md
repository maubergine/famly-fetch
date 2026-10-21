# Contributing

A command-line tool that fetches your (kid's) images from famly.co (a fork of jacobbunk/famly-fetch).

Bug reports and feature requests are welcome as [issues](https://github.com/maubergine/famly-fetch/issues). Pull requests are
welcome too; CI on a pull request from a fork may wait for the maintainer to approve it.

## Commits

Use [Conventional Commits](https://www.conventionalcommits.org/): `fix:`, `feat:`, `chore:`, `docs:` and so on. This fork doesn't use semantic-release, so commits don't cut releases. CI checks
every commit (`commitlint.yml`). To check them locally before you push:

```sh
npm install   # installs commitlint and turns on .githooks/commit-msg
```

Commits to `main` must be signed.

## Tests

Install the dev tools with `pip install -e .[dev]`, then run `ruff check` and `ruff format --diff`. CI also builds the package with `python -m build` and runs `twine check dist/*`. There are no unit tests yet.
