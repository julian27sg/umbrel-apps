# Julian's Umbrel App Store

Community app store for umbrelOS. Add it in umbrelOS under **App Store → ⋯ → Community App Stores** with the URL of this repository, then install the apps from the store page.

## julian-api-pool

One Anthropic API key in front of several Console organizations, routed by remaining monthly credit. Source and documentation: private repository `julian27sg/api-pool`; the image is public at `ghcr.io/julian27sg/api-pool`.

After installing, put these files into the app's data folder (umbrelOS Files app → Apps → API Pool → data):

- `secrets/keys.json` — `{ "<name>": "sk-ant-…" }`, one line per organization (the name is any label, e.g. the account's e-mail)
- `config/config.json` — optional overrides only (e.g. `monthlyUsd: 500` for a Team plan), see `julian-api-pool/config.example.json`

Then restart the app. The generated pool key is in `db/pool.key`.
