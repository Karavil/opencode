# School District Network Whitelist for Goblins

This document lists all Goblins domains that school districts need to whitelist.

---

## IMPORTANT: Use Wildcards When Possible

**We strongly recommend whitelisting `*.goblinsapp.com` instead of individual subdomains.**

If you whitelist only the explicit domains listed below, **your configuration WILL BREAK** when we add new subdomains or change our infrastructure. Using wildcard domains (`*.goblinsapp.com`) ensures continued access without requiring whitelist updates.

---

## Goblins Domains (Explicit List)

If your firewall does not support wildcards, whitelist ALL of the following:

### Primary Domains
```
goblinsapp.com
app.goblinsapp.com
api.goblinsapp.com
cdn.goblinsapp.com
turn.goblinsapp.com
gob.live
```

### Full Explicit List
| Domain | Description |
|--------|-------------|
| `goblinsapp.com` | Marketing website |
| `app.goblinsapp.com` | Main student/teacher application |
| `api.goblinsapp.com` | API endpoints |
| `cdn.goblinsapp.com` | Content delivery / static assets |
| `turn.goblinsapp.com` | WebRTC TURN server for voice features |
| `gob.live` | Short URL domain for sharing |

---

## Preferred Wildcard Configuration

```
*.goblinsapp.com
gob.live
```

**This is the recommended approach.** It covers all current and future subdomains automatically.

---

## Required Ports

| Port | Protocol | Purpose |
|------|----------|---------|
| 443 | TCP | HTTPS and WSS (WebSocket Secure) |
| 3478 | TCP/UDP | WebRTC TURN server (voice features) |

---

## Copy-Paste (Explicit)

```
goblinsapp.com
app.goblinsapp.com
api.goblinsapp.com
cdn.goblinsapp.com
turn.goblinsapp.com
gob.live
```

## Copy-Paste (Wildcard - Recommended)

```
*.goblinsapp.com
gob.live
```

---

*Last updated: March 2026*
*For questions, contact support@goblinsapp.com*
