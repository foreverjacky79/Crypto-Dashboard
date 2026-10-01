# AI agent collaboration guide

This repository is intentionally dependency-free: the dashboard is a static site in
`index.html`. Keep it deployable on GitHub Pages without a build step.

## Working agreement

- Before editing, read the relevant section of `index.html` and preserve the
  Traditional Chinese interface language unless a task calls for a copy change.
- Do not add API secrets, tokens, or private endpoints. The app must use only
  public browser-safe APIs.
- Keep all browser persistence behind the `storage` adapter, so GitHub Pages and
  local previews behave the same way.
- Validate HTML and manually smoke-test interactive changes in a local server.
- When altering deployment, keep `.github/workflows/deploy-pages.yml` compatible
  with GitHub Pages' official Actions deployment flow.

## Parallel work

When several agents contribute, each agent should work in a focused branch or
commit, avoid unrelated reformatting of the single-file app, and describe its
changed UI behavior plus validation in its handoff. Resolve overlapping edits by
re-reading the final file before committing.
