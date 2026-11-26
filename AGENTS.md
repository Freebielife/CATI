# CATI Observatory repository instructions

This is the project repository for the Catizen (CATI) TON observatory. The
standalone page is `index.html`; `project.json` holds token identity, branding,
confirmed pools, data sources and methodology. Shared source snapshots and
factory references retained from the initial repository setup are not live site
configuration. Do not use this repository as the canonical factory for other
tokens or copy its CATI data into another observatory.

## CATI project identity

- Jetton master: `EQD-cvR0Nz6XAyRBvbhz-abTrRC6sI5tvHvvpeQraV9UAAD7`
- Symbol: `CATI`; decimals: `9`
- Hero artwork and section flag: user-provided file, embedded locally in `web/`
- Official channel: `https://t.me/CatizenAnn`

Treat `project.json` as the project source of truth. Verify on-chain identities
before changing the contract or pool set. Do not invent labels, service roles,
links, or token functions; keep source attribution with any added information.
Do not add credentials to source files or the page.

## Build and verification

Before committing site changes:

1. Run `python3 -m scripts.refresh_observatory` when fresh chain data is needed.
2. Run `python3 build.py` and `python3 verify.py`.
3. Check the page at desktop and mobile sizes, all internal links and controls,
   RU/EN content, holder expansion, and absence of horizontal overflow.
4. Confirm the output uses the configured CATI contract and pools, records source
   freshness and partial-history status, and has no external rendering assets.
5. Preserve the last working snapshot if a data source fails. Do not describe
   incomplete trade history as complete.

## Publishing and updates

A commit to `main` stores project code in GitHub. It does not by itself publish a
new page to TON Storage / Resistance Tools or prove that a scheduled refresh ran.
Report code commits, HTML verification, TON publication, and automated-refresh
verification as separate states. Do not change other token repositories or the
shared Cloudflare scheduler from work on this project.
