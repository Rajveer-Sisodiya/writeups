---
title: Example: Hack Smarter Lab
platform: Hack Smarter
difficulty: hard
date: 2026-09-28
tags: [red-team, lateral-movement]
summary: Example writeup showing the structure for a Hack Smarter lab.
sample: true
---
## Summary

One short paragraph: what the target was, the weakness that mattered, and the path from first scan to root. Replace this example with your own notes.

> [!NOTE]
> Everything here is a placeholder. Delete this file when you add your first real writeup.

## Recon

Start with a full port scan, then a service scan on the open ports.

```bash
nmap -p- --min-rate 2000 -oN all-ports.txt 10.10.10.10
nmap -sC -sV -p 22,80 -oN services.txt 10.10.10.10
```

| Port | Service | Notes |
|------|---------|-------|
| 22   | SSH     | Version noted, no creds yet |
| 80   | HTTP    | Web app, worth enumerating |

## Enumeration

Explain what you tried, what you found and why it mattered. Screenshots go in an `images/` folder next to this file:

```markdown
![Directory listing](images/dirs.png)
```

## Foothold

Describe how you got the first shell or credentials, in your own words and with the evidence (commands, output, screenshots).

> [!WARNING]
> Only attack systems you own or have written permission to test.

## Privilege escalation

How you went from a low-privilege user to the highest privilege, and what you checked along the way.

## Lessons learned

- What slowed you down and what you would check earlier next time
- Tools or techniques worth remembering

## Defence

How the weakness could be prevented or detected.
