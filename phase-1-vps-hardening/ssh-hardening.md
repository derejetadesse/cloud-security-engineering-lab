**Why:** Reduces noise from automated bots scanning port 22. Security by obscurity — not a real defense, but cuts log volume significantly.

### Step 6: Configure UFW firewall

```bash
sudo ufw default deny incoming
sudo ufw default allow outgoing
sudo ufw allow 2222/tcp     # SSH (new port)
sudo ufw allow 80/tcp       # HTTP
sudo ufw allow 443/tcp      # HTTPS
sudo ufw allow 5678/tcp     # n8n
sudo ufw enable
sudo ufw status verbose
```

### Step 7: Install and configure Fail2Ban

```bash
sudo apt update && sudo apt install fail2ban -y
sudo systemctl enable --now fail2ban
sudo fail2ban-client status sshd
```

**Why:** Auto-bans IPs after repeated failed login attempts. Critical defense against brute-force.

---

## 📸 Screenshots

*To be added as each step is completed:*
- [ ] `screenshots/01-non-root-user-created.png`
- [ ] `screenshots/02-ssh-key-login.png`
- [ ] `screenshots/03-sshd-config-hardened.png`
- [ ] `screenshots/04-ufw-status.png`
- [ ] `screenshots/05-fail2ban-status.png`

---

## 📚 Lessons Learned (so far)

- **Separate the user from the action.** Even on a personal VPS, working as root is a bad habit. A non-root user with `sudo` adds friction in the right places.
- **Document before you finish.** Writing the plan in this file forced me to think about *why* each step matters — not just *how*.

---

## 🔗 References

- [CIS Ubuntu Linux Benchmark](https://www.cisecurity.org/benchmark/ubuntu_linux)
- [OpenSSH Hardening Guide (ssh-audit.com)](https://www.ssh-audit.com/hardening_guides.html)
- [DigitalOcean — Initial Server Setup with Ubuntu](https://www.digitalocean.com/community/tutorials/initial-server-setup-with-ubuntu-22-04)

---

**Next task in Phase 1:** `ufw-configuration.md`
