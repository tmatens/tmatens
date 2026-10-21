# Todd Matens

Security engineering director by day, self-hoster by night. I build the tooling I wish existed
for the infrastructure I actually run, and I hold it to the bar I'd expect at work: tests,
signed releases, written decisions.

## What I'm building

- **[compose-lint](https://github.com/tmatens/compose-lint)** — security linter for Docker Compose
  files, grounded in OWASP and the CIS Docker Benchmark. SARIF output, GitHub Action, dry-run
  auto-fix. Every release is cosign-signed and traceable to the CI run that built it, and security
  advisories are published on GitHub. Backed by a study of 11,000 public Compose files —
  [9 in 10 skip the basic security flags](https://dev.to/tmatens/9-in-10-docker-compose-files-skip-the-basic-security-flags-2dpf).
- **[container-sec-derive](https://github.com/tmatens/container-sec-derive)** — runtime observation
  tool (Go, eBPF via Inspektor Gadget) that watches a container run and derives the minimum
  security config it actually needs — capabilities, read-only filesystem, devices — instead of
  guessing.
- **[container-security-profiles](https://github.com/tmatens/container-security-profiles)** —
  evidence-backed least-privilege profiles for common self-hosted images, each with drop-test
  proof that the image still works.
- **[ig-advise-gadgets](https://github.com/tmatens/ig-advise-gadgets)** — Inspektor Gadget
  advisor gadgets that derive capabilities, read-only rootfs and device grants from live eBPF
  observation.

The thread through all four: least privilege should be *measured*, not guessed.

## Elsewhere

- Wrote the Compose-file scanner list (Rule 9) in the
  [OWASP Docker Security Cheat Sheet](https://cheatsheetseries.owasp.org/cheatsheets/Docker_Security_Cheat_Sheet.html).
- Writing: [dev.to/tmatens](https://dev.to/tmatens) · Docs: [tmatens.github.io/compose-lint](https://tmatens.github.io/compose-lint/)
- [LinkedIn](https://www.linkedin.com/in/toddmatens/)

Personal projects, personal views — not affiliated with my employer.
