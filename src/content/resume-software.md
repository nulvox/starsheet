---
name: "Ian Trent"
title: "Senior Security Engineer | Software & Platform Engineering"
email: "ian@brokengadgets.io"
phone: "+1 (681) 238-0204"
location: ""
website: "https://brokengadgets.github.io/ian"
github: "brokengadgets"
linkedin: ""
summary: >
  Staff-caliber security and platform software engineer who architects and
  ships high-reliability cloud gateways, multi-tenant CLIs, developer tooling,
  and deterministic automation in Go, Rust, and Python. Focused on explicit
  failure boundaries, zero-plaintext credential models, and repeatable delivery.
---

## Professional Experience

### Microsoft Gaming — Activision Blizzard Publishing — Senior Security Engineer
*January 2023–Present*

- Architected and evolved a shared multi-service platform spanning
  managed-identity authentication, deny-by-default authorization, secret
  isolation, issue tracking, observability, risk evaluation, and AI inference,
  with Go handler templates, JWT re-verification, and RFC 7807 structured errors.
- Engineered multi-tenant Jira and Azure DevOps CLIs with 1Password-backed
  credential isolation, background auth agents, Markdown/Wiki/ADF document
  converters, and offline-tested blueprint planners.
- Built a fail-closed security support-bot and Azure DevOps adapter featuring a
  durable request/event/operation ledger, at-most-once mutation dispatch,
  bounded read-only reconciliation for uncertain writes, and zero-I/O boundary
  guards.
- Authored a Go-based Git SSH and commit-signing identity router, a Rust Linux
  MDE onboarding/diagnostics binary (`x86_64`/`aarch64` MUSL builds), a Windows
  ETW/ETL process-attribution trace reader, and a standard-library-only Go CLI
  for local quantized LLM evaluation.
- Rewrote a legacy serverless bucket-proxy function in Go for substantially
  faster execution and improved CI/CD with multi-architecture release matrices,
  merge-blocking integration suites, and staged promotion gates.

### Broken Gadgets Research and Development LLC — President and CEO
*January 2021–Present*

Maintain a contract-work vehicle for firmware development, Rust engineering, and
embedded-systems research.

### Nebraska Applied Research Institute, University of Nebraska at Omaha — Cyber Engineer / Technical Project Designer
*October 2018–December 2020*

- Built cross-platform Docker development environments and maintained Azure
  DevOps build and test pipelines.
- Provided cloud-emulation guidance, defined sprint goals from broad requirements,
  and wrote proposals for federally funded projects.
- Deployed source- and binary-based coverage-guided fuzzers and developed
  static and dynamic analysis workflows for ARM firmware.

## Technical Focus

**Languages:** Python, Go, Rust, C/C++, assembly, Forth, and shell scripting.

**Software engineering:** API and CLI design, service templates, cross-platform
tooling, infrastructure automation, automated testing, release engineering,
Git, CI/CD, and technical writing.

**Tools:** Cargo Test, GTest, Python unittest, Clang-Tidy, RustFmt, PyLint,
Docker, Podman, GitHub Actions, and Azure DevOps.

**Cloud:** Azure and Google Cloud services, identity, containers, serverless
workloads, observability, artifact management, and event-driven systems.
