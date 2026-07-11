# RiftHub Status

Public uptime monitor and status page for [RiftHub](https://rifthub.app), powered by [Upptime](https://upptime.js.org).

**Live:** https://status.rifthub.app

## Monitors

| Name | Target |
|------|--------|
| Application | `https://rifthub.app/up` |
| Landing Page | `https://rifthub.app` |
| Mailtrap SMTP | `live.smtp.mailtrap.io:587` (TCP) |

## One-time setup

1. Add repository secret **`GH_PAT`** — fine-grained GitHub PAT with read/write on Actions, Contents, Issues, and Workflows for this repo only.
2. Enable **GitHub Actions** on this repository.
3. Run the **Setup CI** workflow (or push a change to `.upptimerc.yml`).
4. Enable **GitHub Pages** → deploy from branch **`gh-pages`** / root (created after first Setup CI run).
5. Add DNS: `status.rifthub.app` CNAME → `buttonsoup.github.io`
6. In Pages settings, set custom domain `status.rifthub.app` and enforce HTTPS.

Incidents auto-open and close as GitHub Issues when monitors fail or recover.
