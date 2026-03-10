# Goblins School Network Whitelist

**Last Updated:** March 2026

This document lists all domains that school districts need to whitelist for Goblins to work properly.

> **IMPORTANT:** We strongly recommend using wildcard domains (e.g., `*.goblinsapp.com`) where your firewall supports it. If you whitelist explicit subdomains instead, **things WILL break when we add new subdomains or change infrastructure**. Wildcard whitelisting future-proofs your configuration.

---

## Quick Copy-Paste Lists

### Wildcard Version (RECOMMENDED)

```
*.goblinsapp.com
gob.live
*.gob.live
*.clerk.com
*.clerk.dev
*.clerkstage.dev
*.google.com
*.googleapis.com
*.gstatic.com
*.googleusercontent.com
*.openai.com
*.anthropic.com
*.elevenlabs.io
*.vercel.app
*.vercel-storage.com
*.vercel.com
*.modal.run
*.modal.com
*.cloudflare.com
*.cloudflareinsights.com
*.clever.com
*.classlink.com
*.sentry.io
*.posthog.com
*.intercom.io
*.intercomcdn.com
*.twilio.com
*.livekit.cloud
*.daily.co
*.agora.io
*.hcaptcha.com
*.stripe.com
*.amazonaws.com
*.s3.amazonaws.com
```

### Explicit Domains (if wildcards not supported)

```
goblinsapp.com
www.goblinsapp.com
app.goblinsapp.com
api.goblinsapp.com
cdn.goblinsapp.com
assets.goblinsapp.com
static.goblinsapp.com
media.goblinsapp.com
ws.goblinsapp.com
realtime.goblinsapp.com
turn.goblinsapp.com
stun.goblinsapp.com
auth.goblinsapp.com
learn.goblinsapp.com
play.goblinsapp.com
dashboard.goblinsapp.com
admin.goblinsapp.com
support.goblinsapp.com
help.goblinsapp.com
docs.goblinsapp.com
status.goblinsapp.com
gob.live
app.gob.live
api.gob.live
clerk.com
clerk.dev
accounts.clerk.dev
api.clerk.dev
api.clerk.com
js.clerk.com
www.clerk.com
accounts.google.com
apis.google.com
oauth2.googleapis.com
www.googleapis.com
fonts.googleapis.com
fonts.gstatic.com
lh3.googleusercontent.com
accounts.youtube.com
ssl.gstatic.com
www.google.com
stun.l.google.com
stun1.l.google.com
stun2.l.google.com
stun3.l.google.com
stun4.l.google.com
api.openai.com
cdn.openai.com
oaiusercontent.com
files.oaiusercontent.com
api.anthropic.com
cdn.anthropic.com
api.elevenlabs.io
storage.elevenlabs.io
vercel.app
vercel.com
vercel-storage.com
public.blob.vercel-storage.com
assets.vercel.com
modal.run
modal.com
api.modal.com
cloudflare.com
challenges.cloudflare.com
static.cloudflareinsights.com
clever.com
www.clever.com
api.clever.com
schools.clever.com
classlink.com
www.classlink.com
launchpad.classlink.com
sentry.io
o0.ingest.sentry.io
browser.sentry-cdn.com
posthog.com
app.posthog.com
us.i.posthog.com
intercom.io
api.intercom.io
widget.intercom.io
api-iam.intercom.io
intercomcdn.com
js.intercomcdn.com
twilio.com
api.twilio.com
video.twilio.com
global.vss.twilio.com
livekit.cloud
turn.livekit.cloud
daily.co
api.daily.co
agora.io
api.agora.io
hcaptcha.com
api.hcaptcha.com
newassets.hcaptcha.com
stripe.com
js.stripe.com
api.stripe.com
m.stripe.com
m.stripe.network
amazonaws.com
s3.amazonaws.com
s3.us-east-1.amazonaws.com
s3.us-west-2.amazonaws.com
```

---

## Detailed Breakdown by Category

### 1. Goblins Primary Domains

| Domain | Description |
|--------|-------------|
| `goblinsapp.com` | Main marketing site |
| `www.goblinsapp.com` | Marketing site (www) |
| `app.goblinsapp.com` | Main student/teacher application |
| `api.goblinsapp.com` | Backend API |
| `cdn.goblinsapp.com` | Content delivery |
| `assets.goblinsapp.com` | Static assets (images, JS, CSS) |
| `static.goblinsapp.com` | Additional static content |
| `media.goblinsapp.com` | Media files (audio, video) |
| `ws.goblinsapp.com` | WebSocket connections |
| `realtime.goblinsapp.com` | Real-time features |
| `turn.goblinsapp.com` | WebRTC TURN server |
| `stun.goblinsapp.com` | WebRTC STUN server |
| `auth.goblinsapp.com` | Authentication service |
| `learn.goblinsapp.com` | Learning content |
| `play.goblinsapp.com` | Interactive features |
| `dashboard.goblinsapp.com` | Teacher/admin dashboard |
| `admin.goblinsapp.com` | Admin panel |
| `support.goblinsapp.com` | Support portal |
| `help.goblinsapp.com` | Help center |
| `docs.goblinsapp.com` | Documentation |
| `status.goblinsapp.com` | Service status page |

### 2. Short Domain

| Domain | Description |
|--------|-------------|
| `gob.live` | Short URL domain for sharing |
| `app.gob.live` | App short links |
| `api.gob.live` | API short links |

### 3. Authentication - Clerk

| Domain | Description |
|--------|-------------|
| `clerk.com` | Clerk authentication |
| `clerk.dev` | Clerk development |
| `accounts.clerk.dev` | Clerk accounts |
| `api.clerk.dev` | Clerk API |
| `api.clerk.com` | Clerk API (production) |
| `js.clerk.com` | Clerk JavaScript SDK |
| `www.clerk.com` | Clerk website |

### 4. Authentication - Google OAuth

| Domain | Description |
|--------|-------------|
| `accounts.google.com` | Google sign-in |
| `apis.google.com` | Google APIs |
| `oauth2.googleapis.com` | OAuth2 authentication |
| `www.googleapis.com` | Google API services |
| `fonts.googleapis.com` | Google Fonts |
| `fonts.gstatic.com` | Google Fonts static |
| `lh3.googleusercontent.com` | Google user content |
| `accounts.youtube.com` | YouTube accounts (linked) |
| `ssl.gstatic.com` | Google static content |
| `www.google.com` | Google main |

### 5. Authentication - Clever SSO

| Domain | Description |
|--------|-------------|
| `clever.com` | Clever SSO |
| `www.clever.com` | Clever website |
| `api.clever.com` | Clever API |
| `schools.clever.com` | Clever schools portal |

### 6. Authentication - ClassLink SSO

| Domain | Description |
|--------|-------------|
| `classlink.com` | ClassLink SSO |
| `www.classlink.com` | ClassLink website |
| `launchpad.classlink.com` | ClassLink launchpad |

### 7. AI Services - OpenAI

| Domain | Description |
|--------|-------------|
| `api.openai.com` | OpenAI API (GPT, Whisper, TTS) |
| `cdn.openai.com` | OpenAI CDN |
| `oaiusercontent.com` | OpenAI user content |
| `files.oaiusercontent.com` | OpenAI files |

### 8. AI Services - Anthropic (Claude)

| Domain | Description |
|--------|-------------|
| `api.anthropic.com` | Anthropic Claude API |
| `cdn.anthropic.com` | Anthropic CDN |

### 9. AI Services - ElevenLabs (Voice)

| Domain | Description |
|--------|-------------|
| `api.elevenlabs.io` | ElevenLabs voice synthesis API |
| `storage.elevenlabs.io` | ElevenLabs audio storage |

### 10. AI Services - Modal (Compute)

| Domain | Description |
|--------|-------------|
| `modal.run` | Modal serverless functions |
| `modal.com` | Modal platform |
| `api.modal.com` | Modal API |

### 11. Infrastructure - Vercel

| Domain | Description |
|--------|-------------|
| `vercel.app` | Vercel deployments |
| `vercel.com` | Vercel platform |
| `vercel-storage.com` | Vercel storage |
| `public.blob.vercel-storage.com` | Vercel blob storage |
| `assets.vercel.com` | Vercel assets |

### 12. Infrastructure - Cloudflare

| Domain | Description |
|--------|-------------|
| `cloudflare.com` | Cloudflare services |
| `challenges.cloudflare.com` | Cloudflare bot verification |
| `static.cloudflareinsights.com` | Cloudflare analytics |

### 13. Infrastructure - AWS

| Domain | Description |
|--------|-------------|
| `amazonaws.com` | AWS services |
| `s3.amazonaws.com` | AWS S3 storage |
| `s3.us-east-1.amazonaws.com` | AWS S3 US East |
| `s3.us-west-2.amazonaws.com` | AWS S3 US West |

### 14. WebRTC - Voice/Video Communication

| Domain | Description |
|--------|-------------|
| `turn.goblinsapp.com` | Goblins TURN server |
| `stun.goblinsapp.com` | Goblins STUN server |
| `stun.l.google.com` | Google STUN server |
| `stun1.l.google.com` | Google STUN server 1 |
| `stun2.l.google.com` | Google STUN server 2 |
| `stun3.l.google.com` | Google STUN server 3 |
| `stun4.l.google.com` | Google STUN server 4 |
| `global.vss.twilio.com` | Twilio video/voice |
| `video.twilio.com` | Twilio video |
| `api.twilio.com` | Twilio API |
| `turn.livekit.cloud` | LiveKit TURN |
| `livekit.cloud` | LiveKit real-time |
| `api.daily.co` | Daily.co API |
| `daily.co` | Daily.co video |
| `api.agora.io` | Agora real-time |
| `agora.io` | Agora services |

### 15. Payments - Stripe

| Domain | Description |
|--------|-------------|
| `stripe.com` | Stripe payments |
| `js.stripe.com` | Stripe JavaScript |
| `api.stripe.com` | Stripe API |
| `m.stripe.com` | Stripe mobile |
| `m.stripe.network` | Stripe network |

### 16. Analytics & Monitoring

| Domain | Description |
|--------|-------------|
| `sentry.io` | Error tracking |
| `o0.ingest.sentry.io` | Sentry data ingestion |
| `browser.sentry-cdn.com` | Sentry browser SDK |
| `posthog.com` | Product analytics |
| `app.posthog.com` | PostHog app |
| `us.i.posthog.com` | PostHog US ingestion |

### 17. Support - Intercom

| Domain | Description |
|--------|-------------|
| `intercom.io` | Intercom support chat |
| `api.intercom.io` | Intercom API |
| `widget.intercom.io` | Intercom widget |
| `api-iam.intercom.io` | Intercom IAM |
| `intercomcdn.com` | Intercom CDN |
| `js.intercomcdn.com` | Intercom JavaScript |

### 18. Security - hCaptcha

| Domain | Description |
|--------|-------------|
| `hcaptcha.com` | hCaptcha verification |
| `api.hcaptcha.com` | hCaptcha API |
| `newassets.hcaptcha.com` | hCaptcha assets |

---

## Required Ports

| Port | Protocol | Purpose |
|------|----------|---------|
| 443 | TCP | HTTPS / WSS (all web traffic) |
| 80 | TCP | HTTP (redirects to HTTPS) |
| 3478 | TCP/UDP | WebRTC TURN server |
| 5349 | TCP | WebRTC TURN over TLS |
| 19302 | UDP | Google STUN servers |
| 10000-20000 | UDP | WebRTC media (if TURN is unavailable) |

---

## Firewall Configuration Notes

### If Using Category-Based Filtering

Many school firewalls use URL categories. Ensure these categories are allowed:
- Education / E-Learning
- Business / Technology
- Cloud Services
- Streaming Media (for voice features)

### Deep Packet Inspection (DPI)

If your firewall performs DPI, ensure it allows:
- WebSocket connections (wss://)
- HTTP/2 and HTTP/3 (QUIC)
- WebRTC traffic

### SSL/TLS Inspection

If performing SSL inspection, ensure certificates are properly trusted for all listed domains to avoid connection failures.

---

## Testing Connectivity

After whitelisting, verify connectivity by:

1. Opening https://goblinsapp.com - should load the marketing site
2. Opening https://app.goblinsapp.com - should load the app login
3. Logging in via Google/Clever/ClassLink - should complete SSO flow
4. Starting a tutoring session - voice features should work

If voice features don't work, check that WebRTC ports (3478, 5349, 19302) are open.

---

## Contact

For questions about network requirements:
- **Support:** support@goblinsapp.com
- **IT Help:** help@goblinsapp.com
