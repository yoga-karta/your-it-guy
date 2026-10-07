<h1 align="center">Dwiyoga Nurkhoiri Fahmi</h1>
<p align="center"><b>Senior IT Infrastructure / DevSecOps Engineer</b></p>
<p align="center">Yogyakarta, Indonesia (GMT+7) · Open to Remote — SEA / EU / US</p>

<p align="center">
  <a href="mailto:fahmieyoga46@gmail.com"><img src="https://img.shields.io/badge/Email-fahmieyoga46%40gmail.com-D14836?logo=gmail&logoColor=white" /></a>
  <a href="https://linkedin.com/in/yoganur"><img src="https://img.shields.io/badge/LinkedIn-yoganur-0A66C2?logo=linkedin&logoColor=white" /></a>
</p>

---

I design and run the infrastructure other people's uptime depends on — multi-tenant automation that isolates every client's credentials, load-balanced edge networks, and the quiet scripts that watch root access at 3am so someone else doesn't have to. Currently working fully remotely for a Singapore-based managed multi-cloud firm, collaborating async across SEA/EU/US time zones.

## Featured Projects

### 🏦 ParseBankers
Bank statement reconciliation engine — matches EJ (ATM switch logs) against RC (settlement/cash) records. Started as a web app, ported to a native Windows desktop tool (**Go + Wails + WebView2**, ~50MB vs 150MB+ for an Electron equivalent) for offline single-user use. Parser validated against real production data: **990 EJ transactions, 98.6% exact match against 717 RC records**. CI/CD via **GitHub Actions** builds signed Windows installers (NSIS) on every push/tag.
`Go` `Wails` `React` `DuckDB` `GitHub Actions`

### 🔐 zero-ssl-renew
Multi-tenant SSL certificate automation — renews ZeroSSL certificates across hundreds of domains (wildcard + subdomain), validates via Cloudflare DNS CNAME, and deploys to origin servers over SSH. Every tenant (client) gets fully isolated credentials, database, and Telegram bot — **zero shared state between clients**, auditable with a single `diff -r`. Entirely operated through a Telegram bot: expiry alerts, interactive renewal, emergency download/deploy.
`Bash` `SQLite` `Telegram Bot API` `Cloudflare API` `systemd`

### 🌐 MikroTik 3-ISP Load Balancing & Security Audit
Designed PCC (Per-Connection Classifier) + policy routing across 3 concurrent ISPs on a RouterOS edge router (RB5009UG+S+) for continuous uptime under link failure. Independently audited the resulting configuration as a senior-level review — identified and documented a critical firewall bypass (an unconditional `accept` rule shadowing the entire drop chain, exposing Winbox to the public internet) with concrete remediation steps.
`RouterOS` `PCC` `Firewall Auditing`

### 🛡️ root-monitor
A self-installing systemd service that watches every `root`/`sudo`/`su` command in real time via a bash prompt hook + `journald`, and pushes it straight to Telegram — so privileged access on a box is never silent. Includes rate-limiting and a periodic heartbeat so "no alerts" never gets confused with "the monitor died."
`Bash` `systemd` `journald` `Telegram Bot API`

### 🖥️ OpenVPN Management Dashboard
Full-stack platform for centrally managing distributed OpenVPN infrastructure — real-time monitoring (CPU/memory/bandwidth) of multiple geographically distributed nodes via a lightweight Python agent, VPN profile lifecycle (create/distribute/revoke with AES encryption), and live dashboards over WebSocket. Hardened with Google OAuth + 2FA (TOTP) + reCAPTCHA, plus automatic IP whitelisting tied directly to the node registry. Full backup/restore, Telegram reporting, Dockerized deployment.
`Next.js` `PostgreSQL` `Prisma` `Python` `Docker` `WebSocket`

## Tech Stack

![Go](https://img.shields.io/badge/-Go-00ADD8?logo=go&logoColor=white)
![Bash](https://img.shields.io/badge/-Bash-4EAA25?logo=gnubash&logoColor=white)
![Nginx](https://img.shields.io/badge/-Nginx-009639?logo=nginx&logoColor=white)
![SQLite](https://img.shields.io/badge/-SQLite-07405E?logo=sqlite&logoColor=white)
![Cloudflare](https://img.shields.io/badge/-Cloudflare-F38020?logo=cloudflare&logoColor=white)
![AWS](https://img.shields.io/badge/-AWS-FF9900?logo=amazonaws&logoColor=white)
![AWS CloudFront](https://img.shields.io/badge/-CloudFront-FF9900?logo=amazoncloudfront&logoColor=white)
![Next.js](https://img.shields.io/badge/-Next.js-000000?logo=nextdotjs&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/-PostgreSQL-4169E1?logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/-Docker-2496ED?logo=docker&logoColor=white)
![Linux](https://img.shields.io/badge/-Linux-FCC624?logo=linux&logoColor=black)
![GitHub Actions](https://img.shields.io/badge/-GitHub%20Actions-2088FF?logo=githubactions&logoColor=white)
![MikroTik](https://img.shields.io/badge/-MikroTik%20RouterOS-293239?logo=mikrotik&logoColor=white)
![Telegram](https://img.shields.io/badge/-Telegram%20Bot%20API-26A5E4?logo=telegram&logoColor=white)

## Certifications

AWS Cloud Practitioner · Cyber Security / Linux+ (Kominfo RI) · DevOps Fundamentals (Dicoding)

---

<p align="center"><i>Full resume (ATS / remote-tailored versions) available on request.</i></p>
