# 🔍 osintracker

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.8%2B-blue?style=for-the-badge&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/Platform-Linux%20%7C%20macOS%20%7C%20Windows-lightgrey?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Version-4.0.0-green?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/OSINT-Framework-red?style=for-the-badge"/>
</p>

<p align="center">
  <b>OSINT Recon Framework — Username Enumeration · Email Analysis · Domain/IP Recon</b><br/>
  <sub>Built for security researchers, CTF players, and penetration testers.</sub>
</p>

---

## ✨ Features

| Module | Description |
|--------|-------------|
| 👤 **Username Scan** | Search across **100+ platforms** simultaneously using multi-threading |
| 📧 **Email Analysis** | Gravatar profile lookup + HaveIBeenPwned breach detection |
| 🌐 **Domain Recon** | DNS records (A/AAAA/rDNS), port scanning, HTTP headers, WHOIS |
| 🇸🇦 **Arabic Platforms** | Dedicated coverage for MENA platforms (Snapchat AR, TikTok AR, Jawaker, Webook.sa) |
| 📊 **HTML Report** | Auto-generated visual report with full scan results |
| 💾 **JSON Export** | Machine-readable output for pipeline integration |

---

## 🖥️ Preview

```
  ███████╗ █████╗ ██╗   ██╗███████╗██████╗
  ██╔════╝██╔══██╗██║   ██║██╔════╝██╔══██╗
  ███████╗███████║██║   ██║█████╗  ██████╔╝
  ╚════██║██╔══██║██║   ██║██╔══╝  ██╔══██╗
  ███████║██║  ██║╚██████╔╝██║     ██████╔╝
  ╚══════╝╚═╝  ╚═╝ ╚═════╝ ╚═╝     ╚═════╝
          OSINT Recon Framework  v4.0.0
       [ For Educational & Authorized Use Only ]
```

---

## 📦 Installation

```bash
# Clone the repo
git clone https://github.com/saufb/osintracker.git
cd osintracker

# No external dependencies needed — uses Python stdlib only
python3 --version  # Requires 3.8+
```

---

## 🚀 Usage

```bash
# Scan a username across 100+ platforms
python3 osintracker.py -u johndoe

# Analyze an email address
python3 osintracker.py -e user@example.com

# Run domain/IP recon
python3 osintracker.py -d example.com

# Full combo scan
python3 osintracker.py -u johndoe -e user@example.com -d example.com

# Interactive mode (no arguments)
python3 osintracker.py
```

---

## 📋 Options

| Flag | Long | Description |
|------|------|-------------|
| `-u` | `--username` | Target username to enumerate |
| `-e` | `--email`    | Target email address to analyze |
| `-d` | `--domain`   | Target domain or IP for recon |

---

## 📁 Output

Reports are saved automatically in a `reports/` folder next to the script:

```
reports/
├── johndoe_20250101_120000.html   ← Visual report (open in browser)
└── johndoe_20250101_120000.json   ← Raw data export
```

Open the HTML report:
```bash
firefox reports/*.html
```

---

## 🌍 Platforms Covered

<details>
<summary>Click to expand full list</summary>

**Development**
GitHub, GitLab, Bitbucket, Stack Overflow, Codepen, Replit, Dev.to, HackerNews, LeetCode, Codeforces, Kaggle, HuggingFace, DockerHub, npm, PyPI, and more...

**Social Media (Global)**
Twitter/X, Instagram, TikTok, Reddit, Pinterest, Snapchat, Facebook, Telegram, Tumblr, VK, Mastodon...

**Arabic / MENA Platforms**
Snapchat AR, TikTok AR, Jawaker, Webook.sa, Vibehut...

**Gaming**
Steam, Twitch, Roblox, Chess.com, Minecraft, Lichess, PSNProfiles, Faceit, HackTheBox, TryHackMe...

**Creative**
DeviantArt, Behance, Dribbble, ArtStation, 500px, Flickr, Wattpad...

**Music**
SoundCloud, Last.fm, Bandcamp, Audiomack, Mixcloud...

**Professional**
LinkedIn, AngelList, Fiverr, Freelancer, BugCrowd, HackerOne, Keybase...

**And many more...**

</details>

---

## 🔬 Domain Recon Module

The `-d` flag runs a full passive/active recon on a domain:

- ✅ **DNS** — A, AAAA, reverse DNS
- ✅ **Port Scan** — 15 common ports (21, 22, 25, 80, 443, 3306, 8080...)
- ✅ **HTTP Headers** — Server, X-Powered-By, security headers
- ✅ **WHOIS** — Registrar, creation date, expiry, registrant

---

## ⚠️ Legal Disclaimer

> This tool is intended for **educational purposes** and **authorized security testing only**.
>
> Do **NOT** use this tool against targets you do not have explicit permission to test.
> The author is not responsible for any misuse or damage caused by this software.
>
> Always comply with applicable laws and regulations.

---

## 📄 License

```
MIT License — Copyright (c) 2026 saufb
```

---

<p align="center">
  Made with ☕ by <b>saufb</b> · Star ⭐ if you find it useful
</p>
