# AGENTS.md

## Purpose
Public API that returns client public IP and request/network metadata.

## Repository Role
- Category: `*.api.airat.top` (public API project).
- Deployment platform: Cloudflare Workers.
- Main files: `worker.js`, `wrangler.toml`.

## API Summary
- Live endpoints: `https://ip.api.airat.top`, alias `https://ip.airat.top`.
- Status page: `https://status.airat.top`.
- Routes: `/`, `/json`, `/text`, `/yaml`, `/xml`, `/health`.

## AI Working Notes
- Preserve plain text contract for `/text` (IP only).
- Keep JSON schema fields stable for existing clients.
- Keep CORS enabled and privacy posture (no request logging by project code).
