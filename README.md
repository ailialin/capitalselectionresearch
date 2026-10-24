# Capital Selection // Open Macroeconomic Research Data Room

The data behind the video essays on YouTube [@CapitalSelection](https://www.youtube.com/@CapitalSelection), published so that every figure on screen can be
checked against its source. Each investigation has its own dossier: the claims, their sources, a verification status
for every figure, the clean series behind each chart, and the raw extracts with their retrieval URL and sha256.
This repository holds data and methodology only: no video, script, code or audio.

## Citation and methodology

Every figure carries a source tier:

* **Tier 1.** Official sovereign / multilateral statistics and documents (World Bank, IMF, UN FAOSTAT, US EIA, Federal Reserve, national statistics offices).
* **Tier 2.** Independent demographic, academic and energy-data audits (e.g. Juan Carlos Albizu-Campos, Ember).
* **Tier 3.** Structured macro synthesis by the channel (reconstructed balance sheets, scenarios); no figure of its own.

Tier is about the source; verification status is about the channel's own check. Each dossier's `sources.csv` gives
both for every figure, with the result of each check (including figures the check contradicted); only figures with
status `fetched` have been matched against downloaded source data.
Official forecasts are used unchanged and labelled; series without one are not projected.

## Investigations

| Dossier | Video | Summary |
|---|---|---|
| [`cuba-2030/`](cuba-2030/) | Cuba 2030: The Anatomy of Systemic Exhaustion | How a state loses its people without a war, its grid without a single strike, and its currency without a formal default. This dossier publishes the series behind each chart and the source and verification status of every figure shown on screen, so the argument can be checked line by line, including where the official series and the on-island estimates disagree. |

*Not investment advice. Educational analysis of public data.*
