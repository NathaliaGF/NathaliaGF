# Nathalia Gomes

**DevSecOps · Linux infrastructure · offensive security (in training)**

I build, ship and break what I build. I come from infrastructure: RHEL/Rocky in production, SELinux enforcing, nftables, CIS hardening and N2/N3 incident response with root-cause analysis. I know how systems are defended and how they break. Today I automate security in the pipeline (SARIF, secrets detection, container checks) and I'm building the offensive side with labs and write-ups.

🌐 [nathaliagf.dev](https://nathaliagf.dev) · 💼 [LinkedIn](https://www.linkedin.com/in/nathalia-gomes-felipe-32aa9b2a9)

---

## Featured projects

### 🐳 [docker-security-scanner](https://github.com/NathaliaGF/docker-security-scanner)
Static security scanner for `Dockerfile` and `docker-compose.yml`.

- 20 rules mapped to the **CIS Docker Benchmark**
- **SARIF** output, so findings show up in GitHub Code Scanning
- Ready-to-use **GitHub Action** for CI
- **MCP server**, so AI assistants can call the scanner as a tool
- AI explanations and suggested fixes that are **re-scanned before being accepted**, so a fix never introduces a new finding

`Python` · `Docker` · `SARIF` · `GitHub Actions` · `MCP`

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
| [🔐 secrets-scanner](https://github.com/NathaliaGF/secrets-scanner) | Finds exposed credentials and API keys in files, directories and **Git history** | Python |
| [🛰️ threat-intel-dashboard](https://github.com/NathaliaGF/threat-intel-dashboard) | Collects and visualizes threat intelligence indicators | JavaScript |
| [🐧 linuxwiki](https://github.com/NathaliaGF/linuxwiki) | Linux wiki: modules, simulated terminal, SM-2 flashcards, offline PWA | HTML · JS |
| [🎫 Helpdesk](https://github.com/NathaliaGF/Helpdesk) | Ticket dashboard with metrics, charts and a REST API | Python · Flask |

---

## What I work with

| | |
|---|---|
| **Linux** | RHEL/CentOS/Rocky, SELinux, nftables, auditd, CIS hardening, Bash |
| **Languages** | Python, Bash, JavaScript/TypeScript, SQL |
| **Databases** | PostgreSQL |
| **Containers** | Docker, Docker Compose, Kubernetes (learning) |
| **DevSecOps** | GitHub Actions, secrets detection, SARIF |
| **Offensive (learning)** | Burp Suite, Nmap, OWASP Top 10, MITRE ATT&CK |

---

## Roadmap

- Write-ups of retired HTB / TryHackMe machines
- A small end-to-end project with IaC and a CI pipeline gated by my own scanners, then attacking it and publishing the findings
- Kubernetes support in `docker-security-scanner`
