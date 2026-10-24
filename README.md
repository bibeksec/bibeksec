<!-- ═══════════════════════════ HEADER ═══════════════════════════ -->
<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:00ff9c,50:0a7d5a,100:0d1117&height=230&section=header&text=BIBEKSEC&fontSize=76&fontColor=ffffff&fontAlignY=38&desc=Penetration%20Tester%20%C2%B7%20Python%20%C2%B7%20Detection%20Engineering&descSize=20&descAlignY=60&animation=fadeIn" alt="BibekSec banner" width="100%"/>

<a href="https://github.com/bibeksec">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=20&pause=1200&color=00FF9C&center=true&vCenter=true&width=760&lines=Attack+%E2%86%92+Understand+%E2%86%92+Detect+%E2%86%92+Defend;Penetration+Tester+%7C+BIT+Student+%7C+Nepal+%F0%9F%87%B3%F0%9F%87%B5;I+break+it%2C+then+I+write+the+detection+for+it;Fundamentals+first.+Evidence+always." alt="Typing animation" />
</a>

<br/><br/>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Bibek%20Tamata-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/bibek-tamata-2b1808446/)
[![Portfolio](https://img.shields.io/badge/Portfolio-bibeksec.github.io-00ff9c?style=for-the-badge&logo=githubpages&logoColor=black)](https://bibeksec.github.io/bibeksec.github.io./)
[![YouTube](https://img.shields.io/badge/YouTube-@BibekSec-ff0000?style=for-the-badge&logo=youtube&logoColor=white)](https://youtube.com/@BibekSec)

[![TryHackMe](https://img.shields.io/badge/TryHackMe-bibektamata012-212c42?style=for-the-badge&logo=tryhackme&logoColor=white)](https://tryhackme.com/p/bibektamata012)
[![Hack The Box](https://img.shields.io/badge/Hack%20The%20Box-Profile-9fef00?style=for-the-badge&logo=hackthebox&logoColor=black)](https://app.hackthebox.com/users/3290646)
[![PortSwigger](https://img.shields.io/badge/PortSwigger-Web%20Security%20Academy-ff6633?style=for-the-badge&logo=portswigger&logoColor=white)](https://portswigger.net/web-security)
[![LeetCode](https://img.shields.io/badge/LeetCode-Problem%20Solving-FFA116?style=for-the-badge&logo=leetcode&logoColor=black)](https://leetcode.com/u/NwLnFoZCvI/)

![Profile views](https://komarev.com/ghpvc/?username=bibeksec&label=Profile%20Views&color=00ff9c&style=flat-square)
![Focus](https://img.shields.io/badge/Focus-Offensive%20%2B%20Defensive-0a7d5a?style=flat-square)
![OS](https://img.shields.io/badge/OS-Linux%20Mint-87cf3e?style=flat-square&logo=linuxmint&logoColor=white)

</div>

---

## 🧬 Identity

```text
$ whoami
bibek_tamata

$ cat profile.txt
role        : Penetration Tester · BIT student · Builder
location    : Nepal 🇳🇵
offense     : Web app testing · enumeration · exploitation in authorized labs
defense     : Log analysis · detection rules · MITRE ATT&CK mapping
languages   : Python · Bash · JavaScript · C++
philosophy  : Understand the fundamentals. Write my own code. Test it. Document it.
rule_one    : Authorization first. Always.
```

I'm **Bibek Tamata**, a penetration tester and BIT student from Nepal. I work on both sides of the fence: I practice offensive techniques in authorized labs, then build tools that **detect** the same attacks. Knowing how an attack works makes better detections, and knowing how detections work makes better attackers *and* better defenders.

<div align="center">

```text
┌───────────────────────────────────────────────────────────┐
│  BIBEKSEC :: OFFENSIVE + DEFENSIVE SECURITY               │
│                                                           │
│   [ ATTACK ] ──▶ [ UNDERSTAND ] ──▶ [ DETECT ] ──▶ [ DEFEND ]   │
│                                                           │
│   Focus       : Pentesting | Python | Detection           │
│   Environment : Linux Mint | Terminal | Security Labs     │
│   Philosophy  : Fundamentals first. Evidence always.      │
└───────────────────────────────────────────────────────────┘
```

</div>

---

## 🎯 How I Work: Pentest Methodology

```mermaid
flowchart LR
    A[Scope &<br/>Authorization] --> B[Recon &<br/>Enumeration]
    B --> C[Vulnerability<br/>Analysis]
    C --> D[Exploitation]
    D --> E[Privilege<br/>Escalation]
    E --> F[Evidence &<br/>Reporting]
    F --> G[Remediation &<br/>Detection]
    G -.->|retest| B
```

Every finding I work on ends the same way: **evidence, impact, a fix, and a detection idea.** A vulnerability that can't be explained and defended isn't finished.

---

## 🚀 Featured Projects

### 🛡️ [Sentinel Detect](https://github.com/bibeksec/sentinel-detect): Lightweight Log-Based Threat Detection Engine

![Python](https://img.shields.io/badge/Python%203.10+-3776AB?style=flat-square&logo=python&logoColor=white)
![Dependencies](https://img.shields.io/badge/Dependencies-zero-00ff9c?style=flat-square)
![MITRE](https://img.shields.io/badge/MITRE%20ATT%26CK-mapped-d9534f?style=flat-square)
![Reports](https://img.shields.io/badge/Reports-Terminal%20%7C%20JSON%20%7C%20HTML-555?style=flat-square)

A Python tool that reads SSH and web-server logs, spots attack patterns, and prints an alert saying **who attacked, how, how serious it is, and which MITRE ATT&CK technique it matches.** Built from the attacker's point of view: if I can run the attack in a lab, I can write the rule that catches it.

| Rule | Detection | Severity | MITRE ATT&CK |
|:--|:--|:--:|:--|
| `SSH-001` | SSH brute force | High | T1110.001 |
| `SSH-002` | Password spraying | High | T1110.003 |
| `SSH-003` | Successful login after brute force | **Critical** | T1110 / T1078 |
| `WEB-002` | SQL injection indicators | High | T1190 |
| `WEB-003` | Path traversal / sensitive-file access | High | T1190 / T1083 |
| `WEB-006` | Command injection / webshell probes | High | T1190 / T1059 |

<sub>…plus root-login, web-scanner/404-flood, offensive-tool user-agent, and XSS rules (10 detections total).</sub>

**Highlights:** stateful sliding-window detection · event correlation · alert cooldowns · IP allowlisting · custom rules · follow mode for live monitoring · firewall-block suggestions · built-in synthetic attack demo · automated self-tests

```bash
git clone https://github.com/bibeksec/sentinel-detect.git && cd sentinel-detect
python3 sentinel.py --demo      # run the synthetic attack demo
python3 sentinel.py selftest    # run the self-test suite
```

<br/>

### 🔍 [Nepal ScamWatch](https://github.com/bibeksec/nepal-scamwatch-a): Live Scam Reporting Platform

![Cloudflare Workers](https://img.shields.io/badge/Cloudflare%20Workers-F38020?style=flat-square&logo=cloudflare&logoColor=white)
![D1](https://img.shields.io/badge/D1%20SQL-F38020?style=flat-square&logo=cloudflare&logoColor=white)
![R2](https://img.shields.io/badge/R2%20Storage-F38020?style=flat-square&logo=cloudflare&logoColor=white)
![Status](https://img.shields.io/badge/Status-Live-00ff9c?style=flat-square)

A deployed web app that makes scam awareness more accessible in Nepal. People can submit and search scam reports with evidence uploads, and an admin moderation panel (token-protected) reviews them. Built serverless on **Cloudflare Workers + D1 + R2**, with the security thinking up front: input validation, moderation workflow, abuse prevention, and careful handling of submitted data.

**[→ Live demo](https://nepal-scamwatch.bibektamata012.workers.dev/)** · **[→ Source](https://github.com/bibeksec/nepal-scamwatch-a)**

<br/>

### 🌐 [GOD'S-EYE NEPAL](https://github.com/bibeksec/god-eye): Cyber & Airspace Situational-Awareness Dashboard

![MapLibre](https://img.shields.io/badge/MapLibre%20GL-396CB2?style=flat-square&logo=maplibre&logoColor=white)
![OSINT](https://img.shields.io/badge/OSINT-6f42c1?style=flat-square)
![License](https://img.shields.io/badge/License-MIT-0a7d5a?style=flat-square)

A Nepal-focused dashboard on **MapLibre GL** with real 3D terrain and buildings, **live aircraft from the OpenSky Network's public ADS-B data**, animated threat arcs, a province-filtered heatmap, and a **traffic analyzer** (throughput, top talkers, protocol/port mix, spike and **port-scan detection**). Cyber and fleet data is clearly labeled as simulated unless you connect your own feed, and the project states plainly that it does no public vehicle or camera surveillance.

```bash
python3 -m http.server 8000   # then open http://localhost:8000
```

<br/>

### 💻 [BibekSec Portfolio](https://bibeksec.github.io/bibeksec.github.io./)

My hub for write-ups, lab notes, and security experiments.

<br/>

<div align="center">

<a href="https://github.com/bibeksec/sentinel-detect"><img src="https://github-readme-stats.vercel.app/api/pin/?username=bibeksec&repo=sentinel-detect&theme=tokyonight&hide_border=true&bg_color=0d1117&title_color=00ff9c&icon_color=00ff9c" alt="sentinel-detect" /></a>
<a href="https://github.com/bibeksec/nepal-scamwatch-a"><img src="https://github-readme-stats.vercel.app/api/pin/?username=bibeksec&repo=nepal-scamwatch-a&theme=tokyonight&hide_border=true&bg_color=0d1117&title_color=00ff9c&icon_color=00ff9c" alt="nepal-scamwatch" /></a>
<a href="https://github.com/bibeksec/god-eye"><img src="https://github-readme-stats.vercel.app/api/pin/?username=bibeksec&repo=god-eye&theme=tokyonight&hide_border=true&bg_color=0d1117&title_color=00ff9c&icon_color=00ff9c" alt="god-eye" /></a>

</div>

---

## 🏴‍☠️ Offensive Security Focus

| Area | What I practice in authorized labs |
|:--|:--|
| 🌐 **Web application security** | OWASP Top 10 classes: injection, XSS, broken access control, auth flaws, path traversal (PortSwigger Academy + THM) |
| 🔎 **Recon & enumeration** | Port/service discovery with Nmap, directory and content discovery, service fingerprinting |
| 🔧 **Traffic & proxy analysis** | Intercepting and manipulating requests with Burp Suite; protocol analysis with Wireshark |
| 🐧 **Linux & privilege escalation** | Linux internals, permissions, misconfiguration hunting |
| 🐍 **Tooling** | Writing my own Python and Bash utilities instead of only running other people's |
| 🛡️ **Detection mindset** | Turning every technique I learn into a log signature or detection rule (see Sentinel Detect) |

### 📊 Lab Progress

<div align="center">

<a href="https://tryhackme.com/p/bibektamata012"><img src="https://tryhackme-badges.s3.amazonaws.com/bibektamata012.png" alt="TryHackMe badge" height="120"/></a>

</div>

<!--
  FILL THESE IN with your real numbers (don't guess, keep it honest):
  | Platform        | Progress                          |
  | TryHackMe       | Rank / rooms completed / streak   |
  | Hack The Box    | Machines owned / challenges       |
  | PortSwigger     | Labs solved (Apprentice/Practitioner/Expert) |
  | LeetCode        | Problems solved                   |
-->

| Platform | Progress |
|:--|:--|
| TryHackMe | [bibektamata012](https://tryhackme.com/p/bibektamata012): *add rank · rooms completed* |
| Hack The Box | [Profile](https://app.hackthebox.com/users/3290646): *add machines owned · challenges* |
| PortSwigger Academy | *add labs solved by level* |
| LeetCode | [Profile](https://leetcode.com/u/NwLnFoZCvI/): *add problems solved* |

---

## 🧰 Technical Arsenal

<div align="center">

| Category | Tools |
|:--|:--|
| **Programming** | ![Python](https://skillicons.dev/icons?i=py) ![C++](https://skillicons.dev/icons?i=cpp) ![JavaScript](https://skillicons.dev/icons?i=js) |
| **Systems & Networking** | ![Linux](https://skillicons.dev/icons?i=linux) ![Bash](https://skillicons.dev/icons?i=bash) |
| **Web & Cloud** | ![HTML](https://skillicons.dev/icons?i=html) ![CSS](https://skillicons.dev/icons?i=css) ![Cloudflare](https://skillicons.dev/icons?i=cloudflare) ![Nodejs](https://skillicons.dev/icons?i=nodejs) |
| **Collaboration** | ![Git](https://skillicons.dev/icons?i=git) ![GitHub](https://skillicons.dev/icons?i=github) |

![Nmap](https://img.shields.io/badge/Nmap-004100?style=for-the-badge&logo=nmap&logoColor=white)
![Burp Suite](https://img.shields.io/badge/Burp%20Suite-FF6633?style=for-the-badge&logo=burpsuite&logoColor=white)
![Wireshark](https://img.shields.io/badge/Wireshark-1679A7?style=for-the-badge&logo=wireshark&logoColor=white)
![OWASP](https://img.shields.io/badge/OWASP-000000?style=for-the-badge&logo=owasp&logoColor=white)
![MITRE ATT&CK](https://img.shields.io/badge/MITRE%20ATT%26CK-d9534f?style=for-the-badge)

<sub>*My toolkit reflects hands-on practice and ongoing learning, not a claim of mastery in every technology.*</sub>

</div>

---

## 📡 Current Operations

| Status | Mission |
|:--:|:--|
| 🟢 | Practicing web app penetration testing in authorized labs |
| 🟢 | Expanding Sentinel Detect with new detection rules |
| 🟢 | Strengthening Python fundamentals and security tooling |
| 🟡 | Linux administration, privilege escalation, and hardening |
| 🟡 | Networking, traffic analysis, and system security |
| 🟡 | SOC analysis and incident investigation foundations |
| 🟡 | Writing lab write-ups and improving documentation |

<sub>🟢 active practice · 🟡 learning in progress</sub>

---

## 🧠 Learning in Public

A strong security engineer should understand **why** a vulnerability exists, **how** it can be verified safely, **how** it can be detected, and **how** it can be prevented.

```python
class BibekSec:
    mission = "Attack. Understand. Detect. Defend."

    principles = [
        "Understand before automating",
        "Practice before claiming expertise",
        "Test before trusting",
        "Document before publishing",
        "Respect authorization and privacy",
    ]

    def next_step(self):
        return "Learn something. Build something. Prove it."
```

---

## ⚖️ Rules of Engagement

```text
[✔] Only test systems I own or have explicit written permission to test
[✔] Labs and CTFs: TryHackMe, Hack The Box, PortSwigger Academy, my own VMs
[✔] Simulated data unless a real feed is explicitly connected and authorized
[✔] Responsible disclosure if I ever find a real issue
[✘] No unauthorized scanning, no real-world targets, no surveillance of people
```

---

## 🤝 Let's Connect

I'm interested in **open-source security tools**, **Python automation**, **detection engineering**, **responsible OSINT**, and **practical cybersecurity education**. If you're building something useful in security, or want to exchange ideas, reach out:

<div align="center">

[![LinkedIn](https://img.shields.io/badge/Connect%20on-LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/bibek-tamata-2b1808446/)
[![GitHub](https://img.shields.io/badge/Follow%20on-GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/bibeksec)
[![YouTube](https://img.shields.io/badge/Watch%20on-YouTube-ff0000?style=for-the-badge&logo=youtube&logoColor=white)](https://youtube.com/@BibekSec)

<br/>

**CURIOUS BY NATURE. DISCIPLINED BY PRACTICE.**

`ATTACK` · `UNDERSTAND` · `DETECT` · `DEFEND`

*Building skills. Writing code. Earning trust.*

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:0a7d5a,100:00ff9c&height=120&section=footer" alt="footer" width="100%"/>

</div>
