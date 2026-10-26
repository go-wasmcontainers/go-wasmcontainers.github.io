# go-wasmcontainers.github.io

The landing page for [go-wasmcontainers](https://github.com/go-wasmcontainers),
built with Hugo and deployed by GitHub Actions. The design comes from the
shared [landingkit](https://github.com/go-fleettools/landingkit) Hugo module
(pinned in `go.mod`); the brand colours in `hugo.toml` are read from
`static/img/logo.svg` with `landingkit brand`, never chosen.

⚠ Pages must be set to **build from the workflow**, not from a branch:

```sh
gh api -X PUT repos/go-wasmcontainers/go-wasmcontainers.github.io/pages -f build_type=workflow
```

A repository left on the default (legacy Jekyll) builder publishes this
README **over** the Hugo output while the deploy workflow reports success, so
check the live page's `generator` meta rather than the workflow's green tick.

The page states only what exists: the engine's first milestone is in progress
and everything else is marked **planned**. Add a feature to the page when it
ships, not before.
