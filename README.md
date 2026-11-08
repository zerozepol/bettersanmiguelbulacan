# Better San Miguel

Independent community transparency portal for **San Miguel, Bulacan**, maintained by [@zerozepol](https://github.com/zerozepol). Work in Progress. Not an official LGU website and not yet registered with or endorsed by BetterGov.

## Run locally

No package installation is required. Build using `node build.mjs`, then run `python3 -m http.server 4173 --directory dist` and open http://localhost:4173. Node.js 18+ and Python 3 are sufficient.

## Scope

This is an independent repository, with its own initial commit, source, LGU data and build. No dependency on the previous shared portal or another LGU repository. Relative asset paths support both domain-root and subpath hosting.

Seven sections follow the [BetterGov LGU guide](https://lgu.bettergov.ph/GUIDE): offices, service guides, barangays, officials, budget/expenditure sources, project records and ordinance archive. Adapted from the BetterSolano static HTML template. Upstream styles and component structures are retained, with LGU-specific content and the sourced directory behavior. See TEMPLATE.md and LICENSES/BetterSolano.txt for provenance and license details.

## Data

208 sourced listings: 33 offices, 49 barangay names, 10 elected officials, 25 Citizen’s Charter links, 5 detailed service guides, 29 projects, 17 ordinances, 34 resolutions 3 LGSF report links and 3 historical appropriation references. See `src/data.json` for per-entry sources, review dates and caveats. Contact numbers have not been telephone-tested. Public source information was reviewed 8 November 2026. Barangay listings are names only, not verified contact listings. Historical procurement records do not establish delivery or completion. No current financial dataset or complete recent ordinance archive is claimed.

## Contribute

Open an issue or PR with a public source for corrections. Add the source URL, `reviewed` date, and a note explaining uncertainty. Rebuild and check search, all seven sections, dialogs, CSV and mobile before publishing. Review public sources quarterly; no automatic monitoring is configured.

## Deployment

Live site: https://bettersanmiguelbulacan.vercel.app/

Hosted on Vercel from this repository (production branch: `main`; build command: `node build.mjs`; output: `dist/`). No paid domain was purchased. This repository contains no hosting credentials or inherited Sites project ID. See `BETTERGOV-SUBMISSION.md` for a draft registration row. Do not claim Active while the public portal is not live.

## Sources

- https://bulacan.gov.ph/cities-and-municipalities/san-miguel/
- https://bulacan.gov.ph/contact-us/
- https://www.sanmiguelbulacan.gov.ph/government/offices
- https://www.sanmiguelbulacan.gov.ph/government/nationaloffices
- https://www.sanmiguelbulacan.gov.ph/government/officials
- https://www.sanmiguelbulacan.gov.ph/transparency/citizens-charter
- https://www.sanmiguelbulacan.gov.ph/government/projects
- https://www.sanmiguelbulacan.gov.ph/transparency/sangguniang-bayan
- https://www.sanmiguelbulacan.gov.ph/transparency/local-government-support-fund

See SOURCE-AUDIT.md for the distinction between index metadata, reviewed charter text, and unreviewed document contents.

## Template
[BetterSolano](https://github.com/BetterSolano/bettersolano), static main branch, adapted with attribution. See TEMPLATE.md for the pinned commit and exact changes. The existing LGU data and Git history are preserved.
