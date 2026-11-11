# renovate-config

Renovate configuration for the `sharkops-io` and `example` GitHub orgs,
run by [Mend's hosted Renovate app](https://github.com/apps/renovate).

| File | What it does |
|---|---|
| `default.json` | The shared preset: `config:recommended`, a 1-day minimum release age, and automerge for minor/patch updates in sharkops-io repos (except `.github`) |
| `org-inherited-config.json` | Applied to every repo in sharkops-io without a per-repo config: no onboarding PR, and extends `default.json` |

The `example` org has its own `renovate-config` repo whose
`org-inherited-config.json` extends this same preset, so both orgs share one
set of rules.

A repo can still add its own `renovate.json` to override anything here.

## License

Apache License 2.0. See [LICENSE](LICENSE).
