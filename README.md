# `.github`

This is the **organization metadata repository** for [`thevoltcloud`](https://github.com/thevoltcloud). GitHub treats a repo named `.github` specially: the community health files here become the **default** for every other repo in the org. Any repo that does not ship its own copy of a file inherits the version in this repo.

If you landed here from a Volt repository looking for a `SECURITY.md`, `CODE_OF_CONDUCT.md`, or contribution guide and didn't find one there — it lives here.

## What's in this repo

| Path | Applies to | Purpose |
|---|---|---|
| `profile/README.md` | `github.com/thevoltcloud` | The org profile page. First thing visitors see. |
| `CODE_OF_CONDUCT.md` | All repos | Contributor Covenant 2.1. |
| `CONTRIBUTING.md` | All public repos | How to contribute, CLA expectations. |
| `SECURITY.md` | All repos | Vulnerability disclosure to `security@volt.cloud`. |
| `SUPPORT.md` | All repos | Where to get help. |
| `GOVERNANCE.md` | OSS components | How decisions get made. |
| `ISSUE_TEMPLATE/` | All repos | Bug / feature / question forms + config. |
| `PULL_REQUEST_TEMPLATE.md` | All repos | Default PR template (Conventional Commits + CLA tick). |
| `workflows/` | Called by other repos | Reusable workflows: license check, SLSA provenance, secret scan. |

## How inheritance works

- A repo with **no** `SECURITY.md` of its own shows the one in this repo.
- A repo that ships its **own** `SECURITY.md` overrides this one.
- Reusable workflows under `workflows/` are not auto-applied. Other repos call them explicitly (see each workflow's header for the `uses:` line).

## Owners

VP Engineering + Head of Compliance (once hired). Until then: CEO (Angel Ramirez, angel@cuemby.com).

Updated infrequently. Changes here affect the whole org — open a PR, get two reviewers.

## License

Apache-2.0. See [`LICENSE`](LICENSE).
