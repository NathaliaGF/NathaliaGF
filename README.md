# Nathalia Gomes

**DevSecOps · Linux infrastructure · Offensive security**

I build, ship and break what I build. I come from infrastructure, with RHEL/Rocky in production, SELinux enforcing, nftables, CIS hardening and N2/N3 incident response with root-cause analysis, so I know both sides of the same system. Today I automate security in the pipeline (SARIF, secrets detection, container checks) and I'm building the offensive side with labs and write-ups.

🌐 [nathaliagf.dev](https://nathaliagf.dev) · 💼 [LinkedIn](https://www.linkedin.com/in/nathalia-gomes-felipe-32aa9b2a9)

---

## Featured projects

### 🚀 [secure-delivery-lab](https://github.com/NathaliaGF/secure-delivery-lab)
A small service delivered the way production software should be: scanned by gates that **block** the release, signed, deployed to a provisioned environment, smoke-tested, and promoted only after approval.

- Pipeline with blocking gates (**dockerscan**, **secrets-scanner**, **Trivy**). The image is scanned first and the *same* image is pushed, signed with **cosign** (keyless) and verified before it is deployed
- **Terraform** provisions staging; smoke tests and a hardening check run against the live container; manual approval to promote; rollback by digest
- **Ansible** role `rhel_cis_hardening` (SSH, firewall, auditd, sysctl...) tested in a Rocky Linux 9 container: idempotence and the effective `sshd` configuration
- Every GitHub Action pinned to a commit SHA, hash-locked dependencies, Dependabot
- The README says what it is *not*: "production" is a promoted tag, not a server

`Terraform` · `Ansible` · `GitHub Actions` · `Docker` · `cosign` · `Trivy` · `Prometheus`

### 🐳 [docker-security-scanner](https://github.com/NathaliaGF/docker-security-scanner)
Static security scanner for `Dockerfile` and `docker-compose.yml`.

- 20 rules mapped to the **CIS Docker Benchmark**
- **SARIF** output, so findings show up in GitHub Code Scanning
- Ready-to-use **GitHub Action** for CI
- **MCP server**, so AI assistants can call the scanner as a tool
- AI explanations and suggested fixes that are **re-scanned before being accepted**, so a fix never introduces a new finding

`Python` · `Docker` · `SARIF` · `GitHub Actions` · `MCP`

### 🔐 [secrets-scanner](https://github.com/NathaliaGF/secrets-scanner)
Finds hard-coded secrets in files, directories, **staged changes** and **Git history**. Zero dependencies.

- 30 rules (cloud, Git hosts, payment, LLM and package-registry keys, private keys, DB URLs, generic `.env`/YAML/JSON assignments)
- Reports a secret at the commit that introduced it; `--staged` works as a **pre-commit hook**
- **SARIF** output, **GitHub Action**, baseline and `.secretsignore` to adopt it on existing repos
- Low-noise filters for placeholders and code; every secret is masked in the output
- 200+ tests on Python 3.9-3.13, and it scans its own repository in CI

`Python` · `Git` · `SARIF` · `GitHub Actions` · `pre-commit`

### 🌐 [wikinet (RedesWiki)](https://github.com/NathaliaGF/wikinet) · [▶ live demo](https://nathaliagf.github.io/wikinet/)
Interactive networking course, from zero to CCNA. 100% frontend, no backend, works offline.

- 9 modules: TCP/IP, OSI, IPv4/IPv6 and CIDR, DNS, DHCP, TLS, firewalls, troubleshooting
- **SM-2 spaced-repetition** flashcards, quizzes, mock exams and guided troubleshooting exercises
- Subnet calculator and a 113-term glossary
- Installable **PWA** with service worker (offline after first visit), dark/light theme

`JavaScript` · `PWA` · `Service Worker` · `HTML/CSS`

---

## Other projects

| Project | What it does | Stack |
|---|---|---|
| [🛰️ threat-intel-dashboard](https://github.com/NathaliaGF/threat-intel-dashboard) | Collects and visualizes threat intelligence indicators | JavaScript |
| [🐧 linuxwiki](https://github.com/NathaliaGF/linuxwiki) | Linux wiki: modules, simulated terminal, SM-2 flashcards, offline PWA | HTML · JS |
| [🎫 Helpdesk](https://github.com/NathaliaGF/Helpdesk) | Ticket dashboard with metrics, charts and a REST API | Python · Flask |

---

## What I work with

| | |
|---|---|
| **Linux** | RHEL/CentOS/Rocky, SELinux, nftables, auditd, CIS hardening, Bash |
| **Languages** | Python, Bash, JavaScript/TypeScript, SQL |
| **Databases** | PostgreSQL, Mongo, NoSQL |
| **Containers** | Docker, Docker Compose, Kubernetes |
| **DevSecOps** | GitHub Actions, secrets detection, SARIF, Trivy, cosign, SBOM |
| **IaC & delivery** | Terraform, Ansible, Docker Compose, Prometheus, Grafana |
| **Offensive** | Burp Suite, OWASP ZAP, Nmap, ffuf, sqlmap, Wireshark, OWASP Top 10, MITRE ATT&CK |

---
