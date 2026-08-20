<h1 align="center">👋 Mudassar Khalid</h1> <h3 align="center"><code>SOC Analyst · Network Engineer · Blue Team by trade, breaker by curiosity</code></h3> <p align="center"> 📍 Islamabad, Pakistan &nbsp;|&nbsp; 🎓 CS Graduate, FAST NUCES &nbsp;|&nbsp; 🟢 Open to Tier 1 SOC / Network Engineer / NOC roles </p> <p align="center"> <a href="mailto:mdsrkhalid0@gmail.com">✉️ mdsrkhalid0@gmail.com</a> &nbsp;·&nbsp; <a href="https://linkedin.com/in/mudassar-khalid-sec">💼 LinkedIn</a> &nbsp;·&nbsp; <a href="https://github.com/mdsr-1">🐙 github.com/mdsr-1</a> </p>

  $ whoami
  > CS graduate who got hooked on the moment logs stop being noise
    and start telling a story.

  $ cat interests.txt
  > SIEM detection engineering · network architecture & hardening
    packet forensics · threat intel · automating the boring parts

  $ status --current
  > Available now. Rotational shifts welcome.

I like the two ends of the same problem: building networks that are hard to break, and watching the logs for the moment someone tries anyway. Most of what's below comes from labs I built myself, not just courses I finished — I wanted evidence I could point to, not just a certificate.

🧪 Labs & Projects

Each of these started as "I wonder if I could build this at home" and turned into something I'd actually defend in an interview.

<details open> <summary><b>🔎 SIEM Threat Detection & Alert Triage Home Lab</b></summary> <br>

The idea: could I build a real detection pipeline — not just read about one — with nothing but a home lab budget?

I stood up the Elastic Stack (ELK) to centralize Syslog and OS event data, then went on the offensive against my own environment: SSH brute-force attempts, Nmap sweeps, the kind of noisy recon that should light up a dashboard. From that telemetry I wrote 5+ custom Kibana detection rules, tuning thresholds until false positives dropped and real anomalies actually stood out.

Then I switched hats — L1 analyst mode — and triaged the alerts I'd just generated: mapped raw log timelines, wrote up incident notes, and timed how fast I could get from "alert fires" to "root cause identified."

Elastic Stack (ELK) Kibana Logstash Linux Bash

</details> <details> <summary><b>🏢 Enterprise Network Architecture & Forensics Lab — CCNA Capstone</b></summary> <br>

The idea: design a network the way an actual enterprise would need it — then attack it like an actual adversary would.

In GNS3, I built a multi-site Head Office + Branch topology across 10+ devices, with departmental VLAN segmentation and OSPF handling the routing. That's the "make it work" half. The "make it survive contact" half came next: DHCP Snooping, Dynamic ARP Inspection (DAI), and explicit ACLs to lock traffic down to least-privilege.

The most satisfying part was forensic, not architectural — capturing PCAPs in Wireshark and watching plaintext Telnet credentials sail across the wire in the clear, right next to an SSH session giving up nothing. That contrast is why I configured a site-to-site IPsec VPN tunnel afterward, to actually encrypt inter-branch traffic instead of just knowing I should.

GNS3 Cisco IOS Wireshark IPsec VPN DHCP Snooping DAI ACLs

</details> <details> <summary><b>🐍 Network Vulnerability Scanner — Python Automation Tool</b></summary> <br>

The idea: manual recon doesn't scale, so build a tool that does the first pass for you.

A CLI-based Python scanner that automates reconnaissance across local subnet ranges — multi-threaded port scanning and banner grabbing, then cross-referenced against the Shodan API for automated CVE correlation on whatever it finds. Results land in structured JSON and SQLite, ranked so the highest-risk assets surface first instead of getting buried in a wall of scan output.

The goal wasn't just "find open ports" — it was building something that tells you which open ports actually matter.

Python Scapy Nmap Shodan API SQLite JSON

</details>
💼 Where I've applied this

Junior Developer — Security & Network Focus, Quantum's Tech, Rawalpindi — Nov 2024 to May 2025

Real client environments, real consequences for getting it wrong:

Built secure backend modules for 5+ client web apps (Node.js, MongoDB) with JWT auth, RBAC, and proper session management
Ran vulnerability assessments on 3 client applications with OWASP ZAP and Burp Suite, then hardened access controls to match
Remediated 12+ critical XSS/CSRF findings and killed off broken-auth and default-credential risks across 5+ environments
Locked down network-facing infrastructure — TLS everywhere, IP restrictions, firewall rules — and inspected API traffic to catch insecure transport before it shipped
🧰 Toolbox
Domain	Tools & Concepts
Security Operations	ELK Stack, Splunk, Microsoft Sentinel, Alert Triage, IoC Tracking, Incident Response Lifecycle
Threat Intel & Recon	VirusTotal, AbuseIPDB, Shodan, Phishing Analysis, OWASP Top 10
Network Architecture	OSPF, EIGRP, VLANs, STP, GRE, VRF, Inter-VLAN Routing, FHRP
Network Security	ACLs, DHCP Snooping, DAI, Port Security, Site-to-Site IPsec VPN, SSH Hardening
Vuln Assessment	Nmap, Burp Suite, OWASP ZAP, Nessus
Scripting & Ops	Python, Bash, PowerShell, Ansible, Terraform, Docker, Git
Platforms	Kali Linux, Windows, Cisco IOS, Oracle VirtualBox
🎓 Background

BS Computer Science — FAST NUCES, Islamabad (Class of 2026) Networks · Ethical Hacking · Information Security · Operating Systems · Database Systems

✅ CCNA (200-301) curriculum completed
✅ TryHackMe — SOC Level 1 path completed
✅ Python Programming & Scripting Foundations — Imagine AI, Islamabad
<p align="center"> <i>Urdu (Native) · English (Fluent) — always happy to talk logs, topologies, or why Telnet still shouldn't exist.</i> </p> <p align="center"> <a href="mailto:mdsrkhalid0@gmail.com"><img src="https://img.shields.io/badge/Say%20hello-mdsrkhalid0%40gmail.com-black?style=flat-square" /></a> </p>
