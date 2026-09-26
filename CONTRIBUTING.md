# Contributing

Thank you for your interest in Spark AI NLP research software. These guidelines apply to every public repository under [sparkainlp-x](https://github.com/sparkainlp-x) that does not provide its own `CONTRIBUTING.md`.

## Before you start

- Read the repository README, especially **What it is / What it is NOT** and **Evidence tags**.
- For anything larger than a typo, open an issue first so we can agree on scope.
- Be kind. All participation is covered by our [Code of Conduct](CODE_OF_CONDUCT.md).

## How to propose a change

1. Fork the repository and create a topic branch from `main`.
2. Keep the change focused: one topic per pull request.
3. Run the repository's tests locally (see its **Tests** section) and make sure they pass.
4. Open a pull request and complete the checklist in the template.

`main` is protected: every change lands through a pull request, history is kept linear (squash merge), and CI must pass where a workflow exists.

## Claim hygiene (fail-closed)

These repositories hold research prototypes. We would rather under-claim than over-claim.

- **Every number carries an evidence tag**: `SYNTHETIC`, `REPORTED`, `TARGET`, or `UNRUN` (definitions in the [README](README.md#evidence-tags)).
- `REPORTED` numbers need the host, toolchain versions, command, and raw data or a link to them.
- Do not add claims of real qubit or QPU runs, hardware readiness, medical or therapeutic effect, certifications, revenue, or peer review unless a public, verifiable source is linked and the maintainer agrees. By default, such text will be removed.
- Simulation output is never presented as hardware or clinical evidence.
- The normative OES-32 residual definition is [oes32-residual@b77b612](https://github.com/sparkainlp-x/oes32-residual/tree/b77b61254f15778c6ae221843dceac7a8571158e) (ADR-001). Other OES-32 implementations are Profile A sidecars and must say so.

If you find an existing claim that breaks these rules, please open a **Claim correction** issue.

## Style

- Python: standard library first, type hints welcome, tests with `pytest` or `unittest`.
- C++: follow the existing style of the repository; keep testbenches runnable with a stock `g++`/CMake toolchain where possible.
- Documentation: plain language, English first. French versions are welcome.

## Licensing

Unless a repository says otherwise, contributions are accepted under the repository's license (MIT). By submitting a pull request you confirm that you have the right to contribute the code or text.

## Privacy

Do not include personal email addresses, phone numbers, or other personal data in commits, issues, or files.
