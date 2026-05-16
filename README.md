# 🛡️ Cloud Security Engineering Lab

> Hands-on cloud security engineering lab built on a production Ubuntu VPS. Documenting my journey from IT graduate to Security Engineer.

![Status](https://img.shields.io/badge/Status-In_Progress-yellow)
![Phase](https://img.shields.io/badge/Current_Phase-1_VPS_Hardening-blue)
![Last Updated](https://img.shields.io/badge/Updated-May_2026-green)

---

## 📖 Overview

This project is my hands-on cloud security engineering lab built on a production Ubuntu VPS (Hostinger). 

The goal is to gain **real-world, production-grade experience** in:

- ☁️ Cloud security engineering
- 🐧 Linux hardening (CIS Benchmarks)
- 🐳 Docker container security
- 📊 SIEM monitoring with Wazuh
- 🚨 Incident response
- 🔔 Monitoring and alerting
- ⚙️ DevSecOps fundamentals
- 🤖 Security automation

---

## 🛠️ Technologies Used

| Category | Tools |
|----------|-------|
| **OS** | Ubuntu Server 22.04 LTS |
| **Containers** | Docker, Docker Compose |
| **SIEM/XDR** | Wazuh |
| **Firewall** | UFW (Uncomplicated Firewall) |
| **Intrusion Prevention** | fail2ban |
| **Auditing** | Lynis, Nessus Essentials |
| **Version Control** | Git, GitHub |
| **Scripting** | Bash, Python |
| **Monitoring** | Wazuh Dashboard, Sysmon |

---

## 🎯 Project Goals

- ✅ Build practical, hands-on cybersecurity skills
- ✅ Create portfolio projects that demonstrate real ability to employers
- ✅ Document security configurations and decisions
- ✅ Practice incident response in a controlled environment
- ✅ Prepare for SOC Analyst and Security Engineer roles

---

## 📅 Phase 1 — VPS Hardening

**Status:** 🚧 In Progress  
**Goal:** Apply CIS Benchmarks to harden a production Ubuntu VPS

### Tasks
- [ ] Secure Ubuntu VPS baseline
- [ ] Create non-root user with sudo privileges
- [ ] Disable root SSH login
- [ ] Configure SSH key-based authentication (disable password auth)
- [ ] Install and configure UFW firewall
- [ ] Enable fail2ban for brute-force protection
- [ ] Enable automatic security updates
- [ ] Run Lynis audit and document score improvement

### Deliverables
- 📄 `phase-1-vps-hardening/ssh-hardening.md`
- 📄 `phase-1-vps-hardening/ufw-configuration.md`
- 📄 `phase-1-vps-hardening/fail2ban-setup.md`
- 📸 Before/after Lynis screenshots

---

## 🐳 Phase 2 — Docker Security

**Status:** ⏳ Upcoming  
**Goal:** Deploy and secure containerized workloads

### Tasks
- [ ] Install Docker Engine on hardened VPS
- [ ] Understand Docker networking and isolation
- [ ] Secure the Docker daemon
- [ ] Run containers with security best practices (non-root, read-only, resource limits)
- [ ] Scan container images with Trivy
- [ ] Document findings and remediation

---

## 📊 Phase 3 — Wazuh SIEM Deployment

**Status:** ⏳ Upcoming  
**Goal:** Deploy enterprise-grade SIEM and respond to real attacks

### Tasks
- [ ] Deploy Wazuh manager + dashboard on VPS
- [ ] Configure Wazuh agents on endpoints
- [ ] Forward logs (SSH, fail2ban, system events)
- [ ] Create custom detection rules
- [ ] Map detections to MITRE ATT&CK framework
- [ ] Simulate brute-force attack → detect and investigate
- [ ] Document incident response process

---

## 📸 Screenshots

*Screenshots and dashboards coming as I complete each phase.*

---

## 📚 Learning Resources

- [TryHackMe — Security Engineer Path](https://tryhackme.com)
- [CIS Benchmarks for Ubuntu](https://www.cisecurity.org/benchmark/ubuntu_linux)
- [Wazuh Documentation](https://documentation.wazuh.com)
- [OWASP Top 10 (2025)](https://owasp.org)

---

## 🔗 Connect with Me

- 🐙 **GitHub:** [@derejetadesse](https://github.com/derejetadesse)
- 🎯 **TryHackMe:** [Your TryHackMe profile link]
- 💼 **LinkedIn:** [Your LinkedIn link]
- 📧 **Email:** [Your email]

---

## 👤 Author

**Dereje Deressa**  
Aspiring Cloud Security Engineer | B.S. IT (Cybersecurity Concentration)

> *"The best way to learn security is to build it, break it, and fix it."*
