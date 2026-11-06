---
name: "Ian Trent"
title: "Senior Security Engineer | Security Platforms, Infrastructure & Automation"
email: "ian@brokengadgets.io"
phone: "+1 (681) 238-0204"
location: ""
website: "https://brokengadgets.github.io/ian"
github: "brokengadgets"
linkedin: ""
summary: >
  Staff-caliber security and platform engineer who architects and operates
  high-trust cloud services, cross-platform endpoint-security tooling,
  developer-identity systems, and deterministic AI-assisted engineering
  workflows across a global enterprise estate. Known for turning complex,
  high-toil operational processes into tested, least-privilege production
  systems in Go, Rust, and Python.
---

## Summary

Security and platform engineer specializing in cloud security architecture,
endpoint-protection engineering (Linux, Windows, macOS), developer tooling, and
deterministic AI-agent security. Track record of shipping production services,
multi-tenant CLIs, and infrastructure-as-code across 1,500+ tracked engineering
deliverables and 35+ internal tools and services, with a rigorous focus on
deny-by-default authorization, secret isolation, and repeatable validation.

## Professional Experience

### Microsoft Gaming — Activision Blizzard Publishing — Senior Security Engineer
*January 2023–Present*

- Architected and evolved a shared multi-service security platform spanning
  managed-identity authentication, deny-by-default authorization, secret
  isolation, issue automation, observability, risk evaluation, and AI inference
  across Azure, Google Cloud, and hybrid on-premises data centers and
  subsidiary networks.
- Built and shipped cross-platform endpoint-security tooling in Rust, Go, and
  Python across Linux, Windows, and macOS estates—including an `aarch64`/`x86_64`
  Linux onboarding and diagnostics suite, a KVM/libvirt dynamic-analysis lab for
  studying EDR internals, a Windows ETW/ETL trace analyzer attributing Defender
  scan overhead to root processes, and a multi-tenant exclusions CLI with
  merge-blocking integration tests.
- Unblocked a global Linux endpoint-security rollout across multiple business
  units by isolating and fixing a package-dependency failure that had crashed
  configuration management and halted fleet deployment.
- Created a polyglot source-security inspector and a deterministic
  Analyze → Implement → Review AI-agent orchestration framework with
  explicit phase gates, dependency-aware task graphs, and formal acceptance-criteria
  validation backpressure.
- Engineered multi-tenant Jira and Azure DevOps automation CLIs and an
  event-driven security support-bot architecture featuring zero plaintext PAT
  storage (1Password-injected auth), blueprint execution, idempotent request
  ledgers, and uncertain-write reconciliation.
- Authored a Go-based Git SSH and commit-signing identity router that
  transparently resolves credentials across personal and multi-org enterprise
  GitHub EMU tenants without URL rewrites.
- Led Security Platform-as-Code consolidation unifying Defender-as-Code
  (Microsoft Graph/Intune) and Sentinel/Cribl logging pipelines under federated
  identity and staged promotion guardrails.
- Drove incident response, blameless postmortems, and fleet support baselines—
  executing cloud control-plane purges for exposed AI credentials, recovering
  multi-board automation outages, and turning recurring architecture reviews
  into explainable risk-scoring engines.

## Earlier Experience

### Broken Gadgets Research and Development LLC — President and CEO
*January 2021–Present*

Own and maintain a mostly inactive consulting company used as a vehicle for
contract security, firmware-development, and embedded-systems research work.


Provided on-demand security-oriented firmware development and embedded-systems
research services, primarily for ARM Cortex platforms.

- Planned and developed expansions to the Tock OS real-time operating system.
- Developed and reported on radio-propagation trials across UHF bands,
  including Wi-Fi, Bluetooth Low Energy, 433 MHz, and 315 MHz.
- Built graphical interfaces and Rust hardware drivers for wearable ARM and ESP
  devices.
- Extended and maintained Docker-based build chains for portable Rust
  compilation.
- Consulted on embedded medical-device cybersecurity and implemented
  out-of-band Bluetooth authentication schemes.
- Researched radio range-extension attacks and modeled transmitter attenuation
  mathematically.
- Worked independently and on research teams of up to four people; wrote,
  reviewed, and submitted federal Other Transaction Authority proposals.

### Nebraska Applied Research Institute (NARI), University of Nebraska at Omaha — Cyber Engineer / Technical Project Designer
*October 2018–December 2020*

- Led security researchers in completing three DARPA SLCS research papers with
  accompanying technology demonstrations.
- Provided security guidance for cloud-based emulation technologies and
  supported emerging standards for hospital control systems.
- Developed attacks and embedded-system techniques for live purple-team and
  red-team exercises involving hospital ICS and power-grid targets, working
  with US Cyber Command, power providers, and hospital ICS staff.
- Defined sprint goals from broad program requirements and wrote proposals for
  federally funded projects.
- Supplied live attack traffic for web-application attack-detection machine
  learning models and deployed source- and binary-based coverage-guided
  fuzzers.
- Designed vulnerability mitigations for life-critical environments and
  reverse-engineered FreeRTOS, Zephyr, Tock, and Nordic SoftDevice deployments.
- Built cross-platform Docker development environments, performed static and
  dynamic analysis of proprietary ARM firmware, and maintained Azure DevOps
  build and test pipelines.

### Hack All the Things, LLC — Principal Courseware Developer
*April 2015–October 2019*

- Developed, tested, and taught cybersecurity workshops with a team of one to
  three developers for professional and Department of Defense audiences.
- Covered Linux-kernel customization, ARP-poisoning detection and deployment,
  advanced iptables, BACnet automation-control networks, SQL injection, and
  BACnet red teaming and incident response.

### Mindful Behavioral Healthcare — Network Administrator
*April 2016–June 2018*

- Deployed and operated a three-building medical-campus network serving more
  than 150 staff members across Windows, macOS, Android, iOS, Minix, and Linux.
- Integrated Linux server stacks, OAuth2 SSO, cloud-based EMR systems, MySQL,
  and SQLite with local infrastructure.
- Wrote Bash and Python systems scripts; performed vulnerability management;
  and improved internal and edge firewall rules.
- Maintained security cameras, occupancy sensors, and electronic locks, and
  advised on technology acquisitions.

### JTY Investment Inc. — General Manager, Multiple Locations
*April 2014–April 2016*

- Managed teams and operations at the downtown Orlando, Florida location, the
  company's second-highest-grossing Jimmy John's location nationwide.

## Selected Experience

### Shared security and engineering platform

- Architected and evolved a multi-service internal security platform into a
  coordinated ecosystem spanning authentication, authorization, secrets access,
  issue tracking, observability, risk evaluation, and AI inference.
- Designed and rolled out a shared AI-inference gateway featuring synchronous
  completion routing, deny-by-default per-deployment authorization, managed
  identities, 1Password-isolated external keys, JWT re-verification, RFC 7807
  structured errors, and upstream body-leakage prevention.
- Designed a Google Cloud to on-premises bridge with least-privilege IAM,
  artifact controls, and observability that decoupled generalized platform
  transport from environment-specific legacy dependencies.
- Consolidated Defender-as-Code (Microsoft Graph/Intune) and Sentinel/Cribl
  security-logging pipelines into a unified Security Platform-as-Code lifecycle
  (`PR → validate → plan → approve → staged deploy → verify`) with subscription-less
  MS Graph plan scoping and automated cloud-identity hand-back receivers.
- Coordinated delivery across Go handlers, gateways, SDKs, Terraform/Terragrunt
  modules, RBAC roles, templates, and architecture documentation.

### Endpoint-security deployment and operations

- Engineered and operated Microsoft Defender for Endpoint (MDE) deployment,
  policy automation, and diagnostics across Linux, Windows, and macOS estates
  spanning globally distributed business units and acquired subsidiary networks.
- Built a Rust-based Linux onboarding and diagnostics tool (`x86_64`/`aarch64`,
  MUSL/GitHub release pipelines) with tenant-aware configuration, URL/JSON
  validation, retry logic, and automated support-ticket integration.
- Built a Windows ETW/ETL trace reader that attributes Defender scan duration
  and CPU overhead to the originating process and extracts host/domain rundown
  telemetry for performance root-cause analysis.
- Built an OpenTofu/KVM/libvirt software dynamic-analysis lab with isolated
  network planes to inspect EDR internals, kernel/daemon behavior, tamper
  protection, package-manager updates, and policy uptake prior to fleet rollout.
- Unblocked a large enterprise Linux MDE onboarding program by diagnosing and
  fixing a package-dependency failure that had interrupted configuration
  management and halted new-host deployment.
- Built a multi-tenant endpoint-policy and exclusions CLI with testbed
  validation and merge-blocking integration tests.
- Established deduplicated canonical-event telemetry across Slack, Jira, and M365
  to measure MDE/MDO/MDC operational support load and separate steady-state
  volume from mass-migration surges.

### AI-agent security, local inference, and deterministic engineering workflows

- Built a polyglot source-security inspector that detects hazardous
  code patterns and antipatterns across Go, Python, TypeScript/JavaScript,
  PowerShell, Terraform, and AI-agent configuration surfaces, complete with
  parser hardening, canonical-path enforcement, and EDR-safe release packaging.
- Created a deterministic Analyze → Implement → Review orchestration framework
  for AI coding agents featuring explicit phase gates, dependency-aware
  task graphs, adversarial challenge passes, formal acceptance-criteria
  backpressure, and holdout-isolated verification.
- Built a local-first, standard-library-only Go CLI for hardware-aware
  quantized LLM evaluation and runtime boundary verification across GGUF/llama.cpp,
  AWQ, and EXL2 artifacts without hidden network egress or telemetry.
- Contributed C/C++ Wayland fractional-scaling, buffer-scale, and Vulkan
  window-surface state fixes to Blender on Linux.
- Shipped a cross-platform architecture, reliability, and operations advisor
  packaged across GitHub Copilot, Claude Code, Codex, and Pi on Linux, macOS,
  Windows, and WSL to evaluate SRE readiness, lifecycle ownership, tenant
  boundaries, and operational toil.

### Issue-management, support-bot, and risk-evaluation automation

- Developed multi-tenant Jira and Azure DevOps CLIs that enforce zero plaintext
  secret storage via 1Password secret references, per-tenant background auth
  agents, Markdown/Wiki/ADF document symmetry, WIQL/JQL search, and
  offline-tested YAML/JSON work blueprints.
- Designed and delivered a fail-closed security support-bot and Azure DevOps
  integration featuring a durable request/event/operation ledger,
  confirmed-ticket-before-work gating, bounded read-only reconciliation for
  uncertain mutations, and cross-platform artifact packaging.
- Launched a policy-aware ticket and incident dispatcher monitoring collaboration
  channels to classify requests, enforce organizational ticket-writing standards,
  and route work into issue trackers with full infrastructure-as-code and RBAC.
- Evolved firewall and security-approval workflows from manual review into an
  explainable risk-evaluation service with real-ticket integration, soak testing,
  production promotion, and metrics by outcome, failure mode, and reason code.

### Developer identity and repository workflows

- Built identity-routing tooling for engineers working across multiple
  organizational and personal Git identities.
- Preserved standard repository URLs while selecting the correct SSH and
  signing identity based on repository ownership.
- Added private-repository installation, interactive setup, cross-platform
  support, key verification, on-disk key storage, and release workflows.
- Improved onboarding documentation and diagnostics, reducing the risk of
  incorrect credentials or signing identities in enterprise development.

### Cloud infrastructure and security governance

- Designed and maintained infrastructure-as-code workflows for cloud
  services, shared networking, identity, authorization, observability,
  artifact storage, and deployment environments.
- Built cloud-native service templates and deployment paths for containerized
  workloads and event-driven systems.
- Improved CI/CD with protected promotion paths, multi-architecture builds,
  validation gates, release packaging, and environment-specific configuration.
- Rolled out a shared AI-inference service behind an identity-aware,
  credential-isolating gateway, validating the initial deployment and beginning
  consumer integration and documentation.
- Rewrote a serverless cloud function in Go and reported substantially better
  local performance, improving the maintainability and runtime foundation of a
  security-support service.
- Connected externally hosted event sources to internally hosted
  security-processing pipelines through an existing secure tunnel pattern,
  avoiding unnecessary infrastructure duplication.
- Supported cloud migration and integration work across multiple providers
  while documenting ownership boundaries and avoiding unnecessary coupling to
  legacy infrastructure.
- Improved operational visibility with structured logs, dashboards, metrics,
  and environment-specific views for service health, security events, and
  workflow behavior.
- Led incident response and blameless postmortems for cloud AI credential
  exposures, executing control-plane purges and establishing execution-boundary
  isolation standards for AI agents.
- Participated in security reviews, architecture assessments, firewall and
  network-approval processes, MCP security baseline evaluations, endpoint-policy
  decisions, and operational readiness work.
- Converted recurring review and approval patterns into reusable
  documentation, decision frameworks, scoring guidance, and automation-ready
  rules.
- Recovered a multi-board workflow outage by isolating multiple causes,
  coordinating fixes and permissions dependencies, and validating full service
  recovery with partner teams.
- Converted recurring security-operations knowledge into troubleshooting
  guides, live demonstrations, recordings, and reusable onboarding
  documentation, reducing dependence on individual subject-matter experts.
- Produced planning artifacts and technical briefs with implementation
  sequences, dependencies, acceptance criteria, and residual risks.
- Fixed and production-deployed a defect in an automated ticket-routing
  service, improving reliability in a workflow used by security operations.

## Core Strengths

- **Security by default:** Deny-by-default authorization, least privilege,
  managed identities, secret isolation, and bounded data exposure.
- **Operationalization:** Moving prototypes and one-off procedures toward
  tested services, reusable templates, documentation, dashboards, and support
  workflows.
- **Developer enablement:** Reducing friction in repository identity,
  installation, issue management, AI-assisted development, and cross-platform
  tooling.
- **Systems thinking:** Balancing delivery speed with supportability,
  lifecycle ownership, data architecture, tenant boundaries, and operational
  toil.
- **Quality:** Automated tests, linting, release validation, architecture
  review, threat modeling, and explicit failure-path analysis.

## Technical Focus

**Cloud & infrastructure:** Infrastructure as code, containerized workloads,
event-driven systems, CI/CD, identity and authorization, observability,
artifact management, and multi-cloud integration.

**Security:** Endpoint protection, policy enforcement, secure installation,
managed identities, secrets management, threat modeling, source inspection,
security architecture, vulnerability research, purple teaming, and secure
embedded systems.

**Embedded and reverse engineering:** ARM Cortex and ARM32 firmware, AVR, MIPS,
PPC, RTOS environments, hardware drivers, Ghidra, GDB, Pwndbg, QEMU, Unicorn,
coverage-guided fuzzing, static analysis, dynamic analysis, and network
protocol analysis.

**Engineering:** Python, C/C++, Rust, Go, assembly, Forth, shell scripting,
CLI design, APIs, service templates, embedded development, cross-platform
tooling, automated testing, release engineering, technical writing, and
AI-agent workflows. Familiar with GTest, Cargo Test,
Python unittest, Clang-Tidy, RustFmt, PyLint, Rudra, Yersinia, Z3, Scapy, Snort,
Nmap, Splunk, and Azure DevOps.

## Tools & Platforms

- **Operating systems and infrastructure:** Nix, NixOS, Terraform, Ansible,
  Salt, Puppet, libvirt, KVM, Docker, and Podman.
- **Languages and automation:** Python, Go, Rust, shell scripting, CLI
  development, APIs, infrastructure automation, and systems integration.
- **Azure:** Identity and access management, compute, storage, networking,
  containers, serverless workloads, monitoring, security, and AI services.
- **Google Cloud:** Identity and access management, compute, storage,
  networking, containers, serverless workloads, monitoring, security, and AI
  services.
- **Delivery and operations:** GitHub Actions, CI/CD, artifact management,
  observability, deployment automation, configuration management, and
  cross-platform release tooling.

## Professional Profile

Security engineer and platform builder who connects security policy to
reliable engineering workflows. Known for coordinating across platform,
infrastructure, security operations, endpoint, cloud, and application teams,
and for turning ambiguous operational problems into clear implementation
sequences, acceptance criteria, and supportable systems.

*This resume intentionally omits confidential company, organization,
repository, project, ticket, tenant, infrastructure, service, URL, and
operational-count details.*
