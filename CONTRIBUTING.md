# Contributing Guide


* [New Contributor Guide](#contributing-guide)
  * [Ways to Contribute](#ways-to-contribute)
  * [Find an Issue](#find-an-issue)
  * [Ask for Help](#ask-for-help)
  * [Pull Request Lifecycle](#pull-request-lifecycle)
  * [Development Environment Setup](#development-environment-setup)
  * [Sign Your Commits](#sign-your-commits)
  * [Pull Request Checklist](#pull-request-checklist)

Welcome! We are glad that you want to contribute to our project! 💖

As you get started, you are in the best position to give us feedback on areas of
our project that we need help with including:

* Problems found during setting up a new developer environment
* Gaps in our Quickstart Guide or documentation
* Bugs in our automation scripts

If anything doesn't make sense, or doesn't work when you run it, please open a
bug report and let us know!

## Ways to Contribute


We welcome many different types of contributions including:

* New features
* Builds, CI/CD
* Bug fixes
* Documentation
* Issue Triage
* Answering questions on Slack/Mailing List
* Web design
* Communications / Social Media / Blog Posts
* Release management

Not everything happens through a GitHub pull request. Please come to our
[Discussions](https://github.com/orgs/thevoltcloud/discussions) or [contact us](mailto:oss@voltcloud.ai) and let's discuss how we can work
together. 

### Come to Meetings


Absolutely everyone is welcome to come to any of our meetings. You never need an
invite to join us. In fact, we want you to join us, even if you don’t have
anything you feel like you want to contribute. Just being there is enough!

Community syncs are announced on the developer mailing list (oss@voltcloud.ai) and in GitHub Discussions. You don’t have to turn on
your video. The first time you come, introducing yourself is more than enough.
Over time, we hope that you feel comfortable voicing your opinions, giving
feedback on others’ ideas, and even sharing your own ideas, and experiences.

## Find an Issue


We have good first issues for new contributors and help wanted issues suitable
for any contributor. [good first issue](https://github.com/search?q=org%3Athevoltcloud+label%3A%22good+first+issue%22+state%3Aopen&type=issues) has extra information to
help you make your first contribution. [help wanted](https://github.com/search?q=org%3Athevoltcloud+label%3A%22help+wanted%22+state%3Aopen&type=issues) are issues
suitable for someone who isn't a core maintainer and is good to move onto after
your first pull request.

Sometimes there won’t be any issues with these labels. That’s ok! There is
likely still something for you to work on. If you want to contribute but you
don’t know where to start or can't find a suitable issue, you can ask in [GitHub Discussions](https://github.com/orgs/thevoltcloud/discussions) and a maintainer will point you somewhere.

Once you see an issue that you'd like to work on, please post a comment saying
that you want to work on it. Something like "I want to work on this" is fine.

## Ask for Help


The best way to reach us with a question when contributing is to ask on:

* The original GitHub issue
* [GitHub Discussions](https://github.com/orgs/thevoltcloud/discussions)
* The developer mailing list: oss@voltcloud.ai

## Pull Request Lifecycle


1. Fork the repository and create a branch off `main`.
2. Make your change. Keep commits focused and write [Conventional Commits](https://www.conventionalcommits.org/) messages (`feat:`, `fix:`, `docs:`, ...).
3. Open a pull request against `main` using the default PR template. Fill in every section.
4. Automated CI runs (lint, tests, license check, secret scan, SLSA provenance). All checks must pass.
5. A maintainer reviews. Public repos require two approving reviews; `docs` and `handbook` require one.
6. Once approved and green, a maintainer merges. We squash-merge by default so the Conventional Commit title becomes the changelog entry.

## Development Environment Setup


Setup is per-repository. Each repo's `README.md` has a **Getting Started** section with the exact toolchain (Go, Python, Node, etc.) and commands. If a repo is missing those instructions, that itself is a good first issue — open one.

## Sign Your Commits

All commits must be **cryptographically signed** (GPG or Sigstore/gitsign) — unsigned commits are rejected by branch protection.

```
git config commit.gpgsign true
git commit -m 'feat: add the thing'
```

### Contributor License Agreement

We require every contributor to sign Volt's Contributor License Agreement (CLA) before we can merge your work. The CLA bot comments on your first pull request with a one-click signing link; sign in with GitHub and the check turns green. Corporate contributors should email oss@voltcloud.ai to set up a company CLA covering their team.

## Pull Request Checklist

When you submit your pull request, or you push new commits to it, our automated
systems will run some checks on your new code. We require that your pull request
passes these checks, but we also have more criteria than just that before we can
accept and merge it. We recommend that you check the following things locally
before you submit your code:

- [ ] Commits follow Conventional Commits and are signed (GPG/Sigstore).
- [ ] Tests added or updated, and the full suite passes locally.
- [ ] Linters pass (`golangci-lint`, `ruff`, `eslint`, etc. — see the repo).
- [ ] Docs / README / examples updated if behavior changed.
- [ ] CLA signed.
- [ ] PR description explains the *why*, not just the *what*.
