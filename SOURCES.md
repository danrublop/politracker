# Data sources

Every outside source PoliTracker uses. Each source's own terms apply. No data is stored in this repository.

## Campaign money (FEC)

| Source | Used for | Coverage | Terms | Fetched |
|---|---|---|---|---|
| [FEC bulk files](https://www.fec.gov/data/browse-data/?tab=bulk-data) | contributions, transfers, committee and candidate records, summaries | 2023–24 | public domain | 2026-10-29 |
| [FEC committee summary file](https://www.fec.gov/files/bulk-downloads/2024/committee_summary_2024.csv) | each committee's totals as filed | 2023–24 | public domain | 2026-11-03 |
| [FEC raw e-filings](https://docquery.fec.gov/) | itemized rows missing from the bulk files | 2023–24 | public domain | 2026-11-03 |
| [openFEC API](https://api.open.fec.gov/developers/) | report totals, committee details, receipts by giver | current | public domain | 2026-11-03 |
| [FEC independent and operating expenditures](https://www.fec.gov/files/bulk-downloads/2024/independent_expenditure_2024.csv) | outside spending for and against candidates; vendor payments | 2023–24 | public domain | 2026-10-29 |

- Federal law (52 U.S.C. § 30111(a)(4)) bars using names from FEC reports to solicit contributions or for commercial
  purposes. Donor addresses and contact details are never published.
- Gifts of $200 or less aren't itemized, so those donors have no names.

## Congress, elections and districts

| Source | Used for | Coverage | Terms | Fetched |
|---|---|---|---|---|
| [unitedstates/congress-legislators](https://github.com/unitedstates/congress-legislators) | members, terms, IDs, committee seats | current | CC0 | 2026-10-30 |
| [Voteview](https://voteview.com/data) | ideology scores (DW-NOMINATE), roll-call votes | 118th–119th | cite Lewis et al. (2026) | 2026-10-30 |
| [congress.gov bill status (GovInfo)](https://www.govinfo.gov/bulkdata/BILLSTATUS) | bill titles, stages, sponsors | 119th | public domain | 2026-10-30 |
| [Census Bureau](https://www.census.gov/geographies/mapping-files.html) | district shapes, ZIP-to-district file, district areas | 119th | public domain | 2026-10-30 → 11-07 |
| [MIT Election Data and Science Lab](https://doi.org/10.7910/DVN/PEJ5QU) | Senate election results | 2020–24 | CC0 | 2026-11-07 |
| [House Clerk election statistics](https://clerk.house.gov/member_info/electionInfo/2024/statistics2024.pdf) | House election results | 2022, 2024 | public, with citation | 2026-11-07 |
| [Alaska Division of Elections](https://www.elections.alaska.gov/results/24GENR/RCV-USRep.pdf) | final ranked-choice rounds (Alaska) | 2022, 2024 | public record | 2026-11-08 |
| [Center for Effective Lawmaking](https://thelawmakers.org/data-download) | Legislative Effectiveness Scores | 118th | cite Volden & Wiseman | 2026-11-07 |
| [Stanford DIME](https://data.stanford.edu/dime) | donor IDs, used to check that two donor records are one person | 1979–2024 | ODC-BY 1.0; cite Bonica (2024) | 2026-11-05 |
| [unitedstates/images](https://github.com/unitedstates/images) | member portraits | current | public domain | 2026-11-02 |

- ZIP codes are placed in districts by land area, so "in-district" shares are approximate.
- Members who arrived by special election in 2025–26 have no 2024 result.

## Lobbying

| Source | Used for | Coverage | Terms | Fetched |
|---|---|---|---|---|
| [Senate LDA (lda.gov)](https://lda.gov/api/) | lobbying spending, issues and bills named, by client | 2023–25 | public | 2026-10-30 |
| [LDA contribution reports (LD-203)](https://lda.gov/api/v1/contributions/) | lobbyists' own political contributions | 2023–24 | public | 2026-11-04 |

- Retrieved from LDA.gov 2026-10-30 to 2026-11-05. "The Senate Office of Public Records cannot vouch for the data or
  analyses derived from these data after the data have been retrieved from LDA.gov."
- Reports name bills and issues, not the side a group took.

## Organizations

| Source | Used for | Coverage | Terms | Fetched |
|---|---|---|---|---|
| [IRS Exempt Organizations Business Master File](https://www.irs.gov/charities-non-profits/exempt-organizations-business-master-file-extract-eo-bmf) | whether a donor organization is tax-exempt, and its type | snapshot 2026-10-29 | public domain | 2026-10-29 |
| [IRS Form 990 e-files](https://www.irs.gov/charities-non-profits/form-990-series-downloads) | nonprofits' grants to political groups, revenue, mission | tax years 2022–24 | public domain | 2026-11-03 |
| [IRS Forms 8871/8872](https://forms.irs.gov/app/pod/dataDownload/fullData) | political organizations that report to the IRS | 2023–24 | public domain | 2026-11-03 |
| [ProPublica Nonprofit Explorer](https://projects.propublica.org/nonprofits/api) | finding nonprofits' tax IDs | current | cite ProPublica | 2026-11-03 |
| [SEC EDGAR](https://www.sec.gov/edgar/sec-api-documentation) | company names and industry codes | current | public | 2026-11-04 |
| [GLEIF](https://api.gleif.org/api/v1/lei-records) | company legal names and parent companies | current | CC0 | 2026-11-05 |
| [Wikidata](https://www.wikidata.org/) | IDs linking companies to their official records and websites | current | CC0 | 2026-11-04 |
| [LittleSis](https://littlesis.org/) | people's positions, as evidence of who works where | current | CC BY-SA 4.0 | 2026-11-03 |
| [Wikimedia Commons](https://commons.wikimedia.org) | photos of a few public-figure donors | current | per file, credited | 2026-11-05 |
| [Simple Icons](https://simpleicons.org/) and organizations' websites | logos, for identification only | current | CC0 / owners' trademarks | 2026-11-04 |

- Donors to nonprofits aren't public, so money from nonprofits is labeled "donors not disclosed".
- Form 990s arrive up to about 18 months late.
- No Wikipedia content is used.

## Checks only

| Source | Used for | Terms |
|---|---|---|
| [OpenSecrets bulk data](https://www.opensecrets.org/open-data/bulk-data) | a local cross-check of industry labels | CC BY-NC-SA; nothing derived from it is published |

## Planned

- House lobbying filings, congressional financial disclosures, House office spending, FEC electioneering
  communications, and earlier election cycles.
