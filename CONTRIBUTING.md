# Contributing

Thank you for your interest in contributing to Safe. This guide applies to every repository in this organization that does not have its own `CONTRIBUTING.md`. It is written for contributors outside Safe Labs. A repository with its own guide follows that guide instead, and setup instructions in a repository's `README.md` always apply.

Some repositories are forks of other projects. Send changes that are not specific to Safe to the upstream project.

## Before You Start

- **Questions and support** do not belong in issues. See the [support guide](SUPPORT.md).
- **Security vulnerabilities** must not be reported in public. See the [security policy](SECURITY.md).
- **Check what exists.** Search the open issues and pull requests first. Your idea may already be in progress or have been discussed.
- **Talk before large changes.** For a new feature, a refactor, or a change to critical behavior, open an issue first so we can agree on the direction before you invest time.

## What We Accept

We welcome bug fixes, tests, documentation improvements, and features that fit the direction of the project.

We do not accept:

- Pull requests that only fix a typo, change wording, or reformat code. They are typically automated activity. If you find a typo, open an issue. This includes pull requests that fix one.
- Large refactors or redesigns that were not discussed first.
- Changes to dependencies, lockfiles, CI workflows, or build and release scripts that were not agreed in an issue first.
- Changes without tests where tests are possible, or without a meaningful description.
- Contributions that you do not understand or cannot explain. You may use AI tools, but you are responsible for every line you submit, and you must be able to answer review questions yourself.

A merged pull request does not entitle you to any reward, token, or other benefit.

## Licensing and CLA

Each repository states its license in its `LICENSE` file, and in a `NOTICE` file where one exists. Licenses differ between repositories, and some repositories changed license over time, so read the files of the repository you contribute to.

By submitting a pull request, you agree that your contribution is licensed under the license in that repository's `LICENSE` file as it stands when your pull request is merged. If the repository has no license file, ask in an issue before you contribute. Only submit work that you have the right to submit, including code written with AI tools or copied from elsewhere.

Where a repository requires the Safe Labs Contributor License Agreement (CLA), a check on your pull request asks you to sign it. You sign by posting a comment on the pull request. Your GitHub username and signature are stored in a public repository. Read the agreement before you sign. If its link does not load, do not sign, and tell us in the pull request. Your pull request cannot be merged until you have signed.

## Making a Change

1. Fork the repository and create a branch from its default branch, unless the repository's own guide names a different base branch.
2. Follow the setup instructions in the repository's `README.md`.
3. Keep the change focused. One pull request addresses one bug, feature, or improvement.
4. Follow the existing code style, and run the linters and tests locally.
5. Add or update tests for the behavior you change, and update the documentation where behavior changes.

## Opening a Pull Request

- Use a [Conventional Commits](https://www.conventionalcommits.org) title, such as `fix: handle empty owner list`, where the repository follows that convention. Pull requests are squash merged, so the title becomes the commit message.
- Fill in the pull request template if the repository has one. Otherwise describe what changed and why, and link the related issue, for example `Fixes #123`.
- Mark the pull request as a draft while it is still in progress.
- Automated checks on a pull request from a fork may wait until a maintainer approves the run.
- A maintainer reviews the pull request. Please respond to review comments, and keep the branch up to date with the base branch.

## Code of Conduct

Everyone taking part in this project is expected to follow the [Code of Conduct](CODE_OF_CONDUCT.md).
