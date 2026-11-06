---
name: "Ian Trent"
title: "Senior Security Engineer | Infrastructure, Cloud & DevSecOps"
email: "ian@brokengadgets.io"
phone: "+1 (681) 238-0204"
location: ""
website: "https://brokengadgets.github.io/ian"
github: "brokengadgets"
linkedin: ""
summary: >
  Staff-caliber infrastructure and security platform engineer specializing in
  multi-cloud IaC, federated identity, Security Platform-as-Code consolidation,
  and cross-platform endpoint fleet operations across Azure, Google Cloud,
  Linux, Windows, and macOS.
---

## Professional Experience

### Microsoft Gaming — Activision Blizzard Publishing — Senior Security Engineer
*January 2023–Present*

- Led Security Platform-as-Code consolidation unifying Defender-as-Code
  (Microsoft Graph/Intune) and Sentinel/Cribl security-logging pipelines under
  federated identity, subscription-less MS Graph plan scoping, and staged
  promotion guardrails (`PR → validate → plan → approve → staged deploy → verify`).
- Architected infrastructure-as-code and Go service templates for a shared
  multi-service security platform across Azure, Google Cloud, and hybrid
  on-premises data centers and subsidiary networks using managed identities,
  1Password secret isolation, and deny-by-default RBAC.
- Engineered cross-platform Microsoft Defender for Endpoint (MDE) deployment and
  fleet automation across Linux, Windows, and macOS—including a Rust Linux
  onboarding/diagnostics suite (`x86_64`/`aarch64`), an OpenTofu/KVM/libvirt
  dynamic-analysis lab for inspecting EDR internals, an ETW/ETL
  process-attribution trace analyzer, and a multi-tenant exclusions CLI with
  merge-blocking integration tests.
- Unblocked a multi-unit enterprise Linux MDE onboarding program by diagnosing
  and fixing a package-dependency failure that had crashed configuration
  management and halted fleet rollout.
- Built a Go-based multi-org Git SSH and commit-signing identity router,
  multi-tenant Jira and Azure DevOps CLIs, and cloud control-plane remediation
  workflows for exposed-credential purges and multi-board service recovery.

### Nebraska Applied Research Institute, University of Nebraska at Omaha — Cyber Engineer / Technical Project Designer
*October 2018–December 2020*

- Developed cross-platform Docker build environments and maintained Azure DevOps
  build and test pipelines.
- Provided security guidance for cloud-based emulation technologies and supported
  standards work for hospital control systems.
- Defined project sprint goals from broad program requirements and documented
  dependencies, acceptance criteria, and residual risks.

### Mindful Behavioral Healthcare — Network Administrator
*April 2016–June 2018*

- Operated a three-building medical-campus network serving more than 150 staff
  across Windows, macOS, Android, iOS, Minix, and Linux.
- Integrated Linux servers, OAuth2 SSO, cloud EMR systems, MySQL, and SQLite;
  maintained firewalls, security cameras, sensors, and electronic locks.

## Technical Focus

**Infrastructure:** Terraform, Terragrunt, Nix, NixOS, Ansible, Salt, Puppet,
Docker, Podman, libvirt, KVM, infrastructure as code, configuration management,
and release engineering.

**Cloud and delivery:** Azure, Google Cloud, Microsoft Graph, Sentinel, Cribl,
GitHub Actions, Azure DevOps, CI/CD, containers, serverless workloads,
event-driven systems, federated identity, networking, and observability.

**Engineering:** Go, Rust, Python, shell scripting, APIs, multi-tenant CLI
design, automated testing, cross-platform tooling, and systems integration.
