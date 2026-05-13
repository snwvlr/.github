# Contributing

Thanks for taking the time to consider contributing. This document covers
the defaults that apply to every project under
[@snwvlr](https://github.com/snwvlr),
[@Orlixys](https://github.com/Orlixys) and
[@Korppi-Mail](https://github.com/Korppi-Mail). Individual repositories may
override these rules with their own `CONTRIBUTING.md`.

---

## Before you open an issue

1. **Search first.** A quick search of open and closed issues usually shows
   whether the topic has been raised before.
2. **One issue, one topic.** Separate concerns into separate issues so they
   can be triaged and tracked independently.
3. **Security issues do not go here.** Anything that could expose users to
   harm goes through the responsible disclosure process described in
   [`SECURITY.md`](./SECURITY.md). Do **not** open public issues for
   vulnerabilities.

## Filing a useful bug report

Include, at minimum:

- The project name and version (or commit hash)
- What you expected to happen
- What actually happened
- Minimal, deterministic steps to reproduce
- Environment details that matter (OS, browser, runtime version)
- Logs, screenshots or recordings when relevant

## Proposing a feature

Feature proposals are welcome, but please understand:

- Most projects here are intentionally small and opinionated. "It would be
  nice if it also did X" is usually not enough — explain the underlying
  problem.
- For Korppi Mail specifically: features that require persisting data on
  disk are not features. They are architectural changes that contradict the
  project's reason for existing. The answer will be no.
- Proprietary projects (Orbit, Photon, anything under Orlixys) accept ideas
  but generally do not accept external code contributions.

---

## Pull requests

When external contributions are accepted, the following applies:

1. **Open an issue first** for anything larger than a typo. Aligning on
   approach before code saves everyone time.
2. **One logical change per pull request.** Smaller PRs are easier to
   review, easier to revert and easier to merge.
3. **Write a clear commit history.** Squash noise commits before opening
   the PR. Commit subjects in imperative mood ("add", "fix", "remove") and
   under ~72 characters.
4. **Match the existing style.** Formatting, linting and naming conventions
   should follow whatever the repository already does.
5. **Include tests** where the project has them, and update documentation
   in the same PR.
6. **Sign off your work.** By opening a pull request you confirm that you
   wrote the code yourself or have the right to contribute it under the
   project's licence.

## Review process

- All pull requests are reviewed manually.
- Response times are best-effort. These projects are maintained solo.
- Feedback is meant for the code, not the contributor.

---

## Code of conduct in two lines

Be technical. Be respectful. Anything else gets the issue or PR closed
without further discussion.

## Contact

- General: **snwvlr@orlixys.com**
- Security: see [`SECURITY.md`](./SECURITY.md)
