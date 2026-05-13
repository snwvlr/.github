# Security Policy

Security is a first-class design constraint across every project I build.
If you've found something that shouldn't be there, this document explains how
to tell me about it without putting users at risk.

---

## Reporting a Vulnerability

**Do not open public GitHub issues for security concerns.**
Public issues expose users before a fix is shipped.

Send a detailed report by email to:

**`snwvlr@orlixys.com`**

Use the subject line: `[SECURITY] <project> — <short summary>`

A good report includes:

- The affected project, component and version (or commit hash, if available)
- A clear description of the vulnerability and its impact
- Steps to reproduce — ideally a minimal proof of concept
- Any logs, payloads, screenshots or recordings that help
- Your assessment of severity
- Suggested remediation (optional, always appreciated)

If the issue is sensitive enough to need encryption, mention it in your first
message and I'll reply with a PGP key.

---

## Scope

Security reports are welcome for any of the following:

| Project | URL |
|---|---|
| Korppi Mail (web) | https://korppimail.com |
| Korppi Mail (Chrome extension) | [Chrome Web Store](https://chromewebstore.google.com/detail/korppi-mail/jlnnniihabchoaocbpfmecnkekdgnhgp) |
| Korppi-Mail organization | https://github.com/Korppi-Mail |
| Orlixys / Orbit | https://github.com/Orlixys |
| Orlixys / Photon | https://github.com/Orlixys |
| Personal repositories | https://github.com/snwvlr |

Out of scope:

- Vulnerabilities in third-party dependencies that have not been integrated
  into the projects above
- Social engineering, physical attacks, or anything requiring access to
  developer machines
- Denial of service that requires more resources than a normal user would have
- Reports generated only from automated scanners without manual validation

---

## Response Times

| Stage | Target |
|---|---|
| Initial acknowledgment | 72 hours |
| Triage and severity assessment | 7 days |
| Fix or mitigation plan | Depends on severity |
| Public disclosure | Coordinated with the reporter |

I work on these projects solo. Response times are best-effort, not contractual.

---

## Recognition

Researchers who report valid vulnerabilities through this process and
practice responsible disclosure will be credited (with permission) in:

- Release notes for the affected project
- A dedicated acknowledgments section once the project grows enough to
  warrant one

There is no paid bug bounty program at this time. If a report leads directly
to a real fix that protects users, I will say so publicly and link to your
work or handle if you'd like.

---

## Korppi Mail — A Note On Threat Model

Korppi Mail is built on the premise that nothing should persist on disk:
mailboxes, messages, tokens and attachments live only in volatile memory,
behind 512-bit cryptographic tokens that are never stored in plaintext.
A reboot wipes the entire service. Reports that argue Korppi *should* have
persistence are not vulnerabilities — they are feature requests, and the
answer is no.

What *is* in scope for Korppi:

- Token leakage, predictability or reuse
- Memory disclosure between mailboxes
- Side channels (timing, length, error messages) that distinguish mailboxes
- Browser extension permission abuse or content-script escape
- TLS/transport issues
- Anything that breaks the "if it isn't in RAM, it doesn't exist" promise

Thanks for keeping these projects honest.
