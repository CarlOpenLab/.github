# Contributing to Carl OpenLab

Thanks for taking the time to contribute. This document applies to every repository in the
[Carl OpenLab](https://github.com/CarlOpenLab) organization unless that repository has its own
`CONTRIBUTING.md`, which takes precedence.

## Before you open an issue

- **Search first.** Someone may have already reported it — adding detail to an existing issue is more
  useful than opening a duplicate.
- **Use the right repository.** Issues belong in the repository that owns the code. If a bug is in
  `@cc-heart/utils-client`, it belongs in [CarlOpenLab/utils-client](https://github.com/CarlOpenLab/utils-client),
  not here.
- **Never report a security vulnerability publicly.** See [SECURITY.md](./SECURITY.md).

## Reporting a bug

A good bug report is reproducible. Please include:

- What you did, what you expected, and what happened instead
- A minimal reproduction — a snippet, a failing test, or a small repository
- The affected package and its exact version (`npm ls <package>`, or the version in your lockfile)
- Your runtime: Node version, browser and OS, or the Electron version if relevant
- The full error text or stack trace, as text rather than a screenshot

## Requesting a feature

Describe the problem before the solution. What are you trying to do, and why do the current APIs not
let you do it? Concrete use cases carry more weight than abstract preferences. If you are proposing a
new public API, showing the call site you wish you could write is the most useful thing you can include.

## Pull requests

### Setting up

Each repository documents its own setup in its `README.md`. In general:

```bash
git clone https://github.com/CarlOpenLab/<repository>.git
cd <repository>
npm install        # or pnpm install / yarn — follow the committed lockfile
```

Use the package manager the repository's lockfile indicates, and leave that lockfile's format alone.
A pull request that regenerates a lockfile with a different tool will be asked to revert it.

### Before you open the pull request

- **Keep it focused.** One logical change per pull request. Unrelated reformatting makes a diff hard to
  review and is usually asked to be split out.
- **Run the checks.** Type-checking, linting and tests are expectations, not suggestions. If a check
  fails and you believe it is unrelated to your change, say so explicitly in the description.
- **Add a test** for a bug fix, and for new behavior where the repository has a test suite.
- **Match the surrounding code.** Naming, comment density and file layout should read like the code
  already there.
- **Write a clear description.** What changed, why, and anything a reviewer should look at closely.
  Link the issue it closes.

### Commit messages

The repositories follow [Conventional Commits](https://www.conventionalcommits.org/):

```
feat: add a namespace helper to the SCSS kit
fix(utils-client): stop the rAF scheduler dropping the final frame
docs: correct the storage-cache expiration example
```

Keep the subject in the imperative mood and under about 72 characters. Use the body to explain *why*
the change is needed when it is not obvious from the diff.

### Review

A maintainer will review as time allows — this is a small organization, so please be patient. Reviews
may request changes; that is a normal part of the process rather than a rejection. Once approved, a
maintainer merges the pull request.

## Releases

Maintainers publish to npm under the `@cc-heart` scope. Contributors do not need to bump versions or
edit changelogs in their pull requests unless a maintainer asks.
