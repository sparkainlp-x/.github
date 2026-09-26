# Security policy

This policy applies to every public repository under [sparkainlp-x](https://github.com/sparkainlp-x) that does not ship its own `SECURITY.md`.

## Reporting a vulnerability

**Please do not open a public issue for security problems.**

Use GitHub **private vulnerability reporting**:

1. Go to the affected repository.
2. Open the **Security** tab.
3. Click **Report a vulnerability** and fill in the form.

Private vulnerability reporting is enabled on each public repository in this account. The report is visible only to the maintainer until an advisory is published.

If the form is unavailable for some reason, open a public issue that says only "security contact requested" (no details), or use the contact options listed at [sparkainlpx.xyz](https://sparkainlpx.xyz), and we will set up a private channel.

Helpful details:

- Affected repository, file(s), and commit or tag
- Steps to reproduce or a proof of concept
- Impact as you understand it

## What to expect

This is a small, founder-run research project. We aim to acknowledge reports within **7 days** (TARGET) and to agree on a fix and disclosure timeline with you. We will credit reporters in the advisory unless you prefer to stay anonymous.

## Scope

These repositories contain research prototypes (Python references, C++ testbenches, HLS/FPGA scripts). They are not production services and are not certified for safety-critical use. In scope:

- Code in the default branch and in published releases
- CI workflows (for example, unsafe triggers or secret exposure)
- Build and deployment scripts (for example, HLS/Vivado/PetaLinux scripts and self-hosted runner jobs)

Out of scope: findings that require a compromised developer machine, and issues in third-party dependencies that should be reported upstream (we still appreciate a heads-up).

## Supported versions

Only the latest release and the current `main` branch of each repository receive fixes.

## Build artifacts

Hardware build artifacts (bitstreams, boot images, `.xsa` files) are not published in these repositories. If a workflow uploads artifacts, they are retained for a limited time and are research outputs only.
