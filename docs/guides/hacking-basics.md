# Hacking Basics in Grey Hack

This guide introduces the fundamental concepts of hacking in Grey Hack, covering reconnaissance, gaining access, and maintaining persistence.

## Understanding the Hacking Process
Hacking in Grey Hack follows a structured process:

1. **Reconnaissance** – Gathering information about targets.
2. **Exploitation** – Using vulnerabilities to gain access.
3. **Privilege Escalation** – Gaining higher-level permissions.
4. **Persistence** – Maintaining access to a compromised system.

## Reconnaissance
Before hacking, you need to gather information about your target. Common techniques include:

- **Scanning the Network**: Use `nmap <IP>` to identify open ports and services.
- **Checking System Info**: Commands like `uname -a` reveal OS details.
- **Exploring Directories**: Look for configuration files or logs with `ls -la`.

## Exploiting Vulnerabilities
Once you have gathered information, you can look for weaknesses:

- **Default Credentials**: Some systems use weak or default passwords.
- **Exploitable Services**: Open ports running outdated services may have known exploits.
- **Brute Force Attacks**: Tools like `hydra` can attempt to crack passwords.

## Gaining Access
To break into a system, you can:

- Use known exploits (`exploit <target>` if available).
- Try SSH or FTP login with discovered credentials (`ssh user@IP`).
- Inject malicious scripts if permissions allow.

## Privilege Escalation
After gaining initial access, escalate privileges to control the system:

- **Check User Permissions**: Use `whoami` and `sudo -l`.
- **Search for Misconfigurations**: Some files may have improper permissions.
- **Use Kernel Exploits**: Outdated kernels might have vulnerabilities.

## Maintaining Persistence
To keep access after a reboot:

- **Create a Backdoor**: Add a new user or set up SSH keys.
- **Modify System Services**: Hide processes or modify startup scripts.
- **Cover Your Tracks**: Clear logs using `rm /var/log/*` (but be careful!).

## Next Steps
Now that you understand the basics, explore:

- [Networking](networking.md) – Learn about connections, IP addresses, and firewalls.
- [Exploits](reference/exploits.md) – A list of known exploits within Grey Hack.

---
**Practice your skills ethically and experiment within the game!**

