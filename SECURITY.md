# Security Policy / Chính sách bảo mật

## Supported Versions

Only the latest commit on the `main` branch is supported.

## Reporting a Vulnerability / Báo cáo lỗ hổng

If you discover a security vulnerability in this project, please report it
**privately** rather than opening a public issue:

1. Go to the [Security tab](../../security/advisories) of this repository
2. Click **"Report a vulnerability"**
3. Provide a clear description, affected versions, and reproduction steps

Nếu bạn phát hiện lỗ hổng bảo mật, vui lòng báo cáo **riêng tư** qua tab
"Security" của repo này, không mở public issue.

## Site Hardening Measures Already in Place

This is a static, single-file HTML page hosted on GitHub Pages. The page
itself implements:

- **Content Security Policy (CSP)** — restricts resource origins to self
  + Google Fonts only
- **X-Frame-Options: DENY** — prevents clickjacking via iframe
- **X-Content-Type-Options: nosniff** — disables MIME sniffing
- **Strict referrer policy** — limits cross-origin URL leaks
- **Permissions-Policy** — disables camera, microphone, geolocation,
  payment, USB, sensors
- **No external runtime dependencies** — no third-party JS executed
- **No user input handling** — page reads no user data; nothing to inject
- **Upgrade-insecure-requests** — forces HTTPS for any sub-resources

## Account-Level Recommendations

This repository owner has enabled (or should enable):

- [ ] **Two-factor authentication (2FA)** on the GitHub account
- [ ] **Settings → Pages → Enforce HTTPS** for `*.github.io` site
- [ ] **Branch protection** on `main` (require PR review)
- [ ] **Secret scanning** alerts (Settings → Code security)
- [ ] **Dependabot** alerts (no deps to scan, but enable for future)
- [ ] **Code scanning** with CodeQL (free for public repos)
- [ ] Periodic review of OAuth apps and Personal Access Tokens

## License & Liability

See the disclaimer at the bottom of [index.html](index.html). The
software is provided "AS IS" without warranty.

Last updated: 2026-05-17
