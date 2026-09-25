# StudioSpend public files

Published from the public repo `Leonardo-Labs/studiospend-public` by Cloudflare Pages
(project `studiospend-public`, `https://studiospend-public.pages.dev/`; later also on the product domain). This folder in the private repo is
the source of truth; copy changes there.

- `oauth/client-metadata.json` — StudioSpend's OAuth Client ID Metadata Document. Its URL
  is the app's client id at platforms that use metadata documents instead of registration
  (ElevenLabs). **Never move or rename it**: the URL is baked into the app
  (`mcp_auth::CLIENT_METADATA_URL`) and changing it signs everyone out of those platforms.
  `redirect_uris` must match `mcp_auth::CIMD_PORT`.
- Later: app update files (`latest.json` and release downloads) — see DECISIONS.md.

Nothing private goes here: this repo is public.
