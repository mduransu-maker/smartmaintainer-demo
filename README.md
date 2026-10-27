# SmartMaintainer · Interactive demo

**From a reported issue to a clear next step.**

[Open the demo ↗](https://mduransu-maker.github.io/smartmaintainer-demo/) · [Original project](https://github.com/alem187/SmartMaintainer) · [Merged contribution](https://github.com/alem187/SmartMaintainer/pull/1)

![Demo workspace with synthetic maintenance tickets](https://raw.githubusercontent.com/alem187/SmartMaintainer/main/docs/workspace-desktop.png)

Try the actual demo workspace: create tickets, assign a team, update status, write notes, plan next steps, filter the board and export CSV reports. Switch to analytics to inspect the same example tickets.

This is a static build of the existing project's demo workspace and analytics. The contribution covers that workspace, analytics improvements and tests; it does not claim the entire pre-existing application.

All tickets, teams and properties are synthetic. Changes stay in memory until reload. There is no account, backend, real AI inference, email or notification delivery. CSV exports contain the example data and any local edits.

## Run and verify

```sh
npm ci
npm test
npm run typecheck
npm run build
```

The build exports to `out/`, with `/smartmaintainer-demo` as the default project path. Override `PAGES_BASE_PATH` for another host. GitHub Actions runs the 14 regression tests, TypeScript and static export, then deploys to GitHub Pages.

See [ATTRIBUTION.md](ATTRIBUTION.md) for provenance. Existing upstream rights remain unchanged.
