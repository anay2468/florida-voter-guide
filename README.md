# Florida 2026 Voter Guide

A single-page, plain-English dashboard for the **August 18, 2026 primary** and **November 3, 2026 general election** in Florida.

**Live site:** _https://anay2468.github.io/florida-voter-guide/_

## What's covered

- **Overview** — election dates, closed-primary rules, big-issue themes, race ratings
- **Governor** — profiles, polling, and stance summaries for the top Republican and Democratic candidates
- **U.S. Senate** — the special election to fill Marco Rubio's seat (Moody, Vindman, Nixon, GOP primary challengers)
- **Compare Issues** — toggle-able side-by-side stance table for Governor and Senate candidates
- **Other Races** — Cabinet (Attorney General, CFO, Agriculture Commissioner), with clickable candidate modals
- **Ballot Amendments** — the two certified 2026 constitutional amendments (Agriculture tangible property; Budget Stabilization Fund), with plain-language YES/NO explainers and the 60% threshold
- **Local Elections** — county-by-county breakdown for Manatee, Sarasota, Hillsborough, Pasco, Pinellas, Orange, Seminole, and Duval. Includes county offices on the ballot, qualifying dates, Supervisor of Elections contact info, races to watch, **city/municipal elections**, and **U.S. House + state legislative districts** (with notes on the May 2026 congressional redistricting)
- **How to Vote** — primary and general deadlines, mail/early/in-person voting, ID rules, and a full Sources & Bias Transparency block

## Stack

Plain HTML, CSS, and vanilla JavaScript. No build step, no dependencies, no tracking — everything lives in `index.html`.

To preview locally:

```bash
# any static file server works
python3 -m http.server 8000
# then open http://localhost:8000
```

## Repository layout

```
.
├── index.html              # the full dashboard
├── README.md               # this file
├── LICENSE                 # MIT
├── .gitignore
└── .github/
    └── workflows/
        └── pages.yml       # auto-deploys to GitHub Pages on push to main
```

## Deploying to GitHub Pages

The included workflow at `.github/workflows/pages.yml` deploys the site whenever you push to `main`.

After your first push:

1. Go to **Settings → Pages**
2. Under **Build and deployment**, set **Source** to **GitHub Actions**
3. The next push to `main` will publish the site automatically. The URL appears in the workflow's deploy step.

## Sources

All data is from public sources — Florida Division of Elections, Ballotpedia, Wikipedia, candidate campaign sites, university polling (Emerson, UNF, Stetson), Florida-focused outlets (Florida Politics, Florida Phoenix, Tampa Bay Times, WUSF, WLRN, Jacksonville Today, WSLR), and national outlets (NBC, CBS, CNN, PBS). A full Sources & Bias Transparency section with per-source ratings is included in the dashboard itself under **How to Vote → Sources**.

## Updating

This dashboard is a snapshot. Numbers (polling, fundraising, candidate fields) change quickly. Before relying on it for voting decisions, cross-check with:

- [Florida Division of Elections](https://dos.fl.gov/elections/)
- Your county [Supervisor of Elections](https://dos.fl.gov/elections/contacts/supervisor-of-elections/)
- [Ballotpedia: Florida elections, 2026](https://ballotpedia.org/Florida_elections,_2026)

## Disclaimer

This dashboard is not affiliated with any candidate, party, or political committee. It is informational only and does not endorse any candidate or ballot measure. Positions are summarized; always read a candidate's own platform and the full ballot text before voting.

## License

MIT — see [LICENSE](LICENSE).
