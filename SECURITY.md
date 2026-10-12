# Security Policy

This policy applies to every repository in the [Carl OpenLab](https://github.com/CarlOpenLab)
organization and to every package published under the `@cc-heart` npm scope.

## Reporting a vulnerability

**Please do not report security vulnerabilities in a public issue, discussion, or pull request.**

Report privately through GitHub's private vulnerability reporting:

1. Open the **Security** tab of the affected repository.
2. Click **Report a vulnerability**.
3. Describe the issue, the affected version, and the impact you believe it has.

If the **Report a vulnerability** button is not available on that repository, open a
[new issue here](https://github.com/CarlOpenLab/.github/issues) that says only that you have a security
report and would like a private channel. Do not include any details in that issue — a maintainer will
follow up and move the conversation somewhere private.

## What to include

- The affected package or project, and the version you tested
- A minimal reproduction, or a precise description of the conditions required
- The impact as you understand it — what an attacker gains, and what they need to start
- Any suggested fix or mitigation, if you have one

## What to expect

This is a small, volunteer-run organization, so please allow time for a response.

- **Acknowledgement** of your report.
- **An assessment** — whether it is reproducible, and how severe it appears.
- **A fix and a release**, with credit to you in the release notes unless you ask to remain anonymous.
- **Coordination on disclosure.** Please give us a reasonable window to ship a fix before publishing
  details. We will not ask you to stay silent indefinitely, and we are happy to agree a date with you.

## Scope

In scope: the code in our public repositories and the packages published to npm under `@cc-heart`.

Out of scope: vulnerabilities in third-party dependencies (report those upstream, though a heads-up is
welcome), and issues that require an already-compromised machine or a modified local build.

Note that several of our tools are deliberately local-first and are designed to bind to `127.0.0.1`.
A design decision that a local service is reachable from the local machine is not, by itself, a
vulnerability — but reachability from a remote origin, or from another local user, is.
