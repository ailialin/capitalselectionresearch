# Cuba 2030: The Anatomy of Systemic Exhaustion

How a state loses its people without a war, its grid without a single strike, and its currency without a formal default. This dossier publishes the series behind each chart and the source and verification status of every figure shown on screen, so the argument can be checked line by line, including where the official series and the on-island estimates disagree.

The video is released on YouTube at [@CapitalSelection](https://www.youtube.com/@CapitalSelection); its direct link is added here on release.

*Generated 2026-10-25 by the channel's export pipeline. Do not edit by hand: regenerate.*

## Production Baseline & Rapid Deterioration Note

The master video (v1.0, 10:32) is locked and will not be re-rendered: it is a timestamped analytical baseline. Its on-screen figures reflect indicators from mid-2024 to 2025, as supplied to production. This dossier is the living record: it shows where later data has moved, including where it disagrees with the video.

* **Currency.** The informal rate used on screen (~410 CUP/USD, which puts a 4,800 CUP surgeon's wage at ~$12) has since reached ~800 CUP/USD (elTOQUE, October 2026), putting the same wage at ~$6 a month. Against the 24 CUP official rate of 2021 the loss of purchasing power is now about -97%, not -94%.
* **Demographics.** The video showed -1.1M (-10%). ONEI's official effective population, as reported from its statements, went from ~11.11M at end-2021 to 9,748,532 at end-2024: about -1.36M (-12%). ONEI's tables were checked through reporting that quotes them; the independent Albizu-Campos estimate (8.62M for 2023) is lower still.
* **Capital allocation.** ONEI's combined share of hotels and restaurants plus business services and real estate was 33.5% of all investment in 2023 and 37.4% in 2024, consistent with the 35.6% shown on screen; health stayed near 2% and agriculture near 3%. The 2020-2022 tables behind the on-screen 2020-2024 average have not yet been retrieved, and the GAESA attribution is the channel's reading, not an ONEI category.
* **Mining.** USGS Mineral Commodity Summaries 2026 confirms Cuba in the top 5 for cobalt reserves (500,000 t, 5th). For nickel, the 2026 edition no longer lists Cuba separately (it falls under "Other countries"), so the on-screen "nickel & cobalt: USGS top 5" holds for cobalt only; the nickel ranking dates from earlier editions.
* **Figures the checks did not support.** Some on-screen figures were contradicted or could not be sourced, among them remittances of $2.5bn (independent estimates: $1.8-2.1bn), a 400,000 t sugar consumption baseline (the 2022 plan allotted 500,000 t), and the Torre K cost and occupancy. Every check, with its date and sources, is in `sources.csv`.

## Core theses

### 1. The Demographic Exodus

The official international series (World Bank WDI, based on UN WPP) and the on-island estimate (ONEI / Albizu-Campos) disagree on the size of the loss since 2021. Both are published side by side in `data/population_trajectory_*.csv`, never blended; the gap between them is itself part of the finding.

### 2. Base Grid Exhaustion

Average annual output (Ember) has stayed far below the stated peak demand for the whole series; the 2024 collapse is a peak-hour event (UNE bulletins, not yet verified) that annual averages do not show. `data/electricity_generation_*.csv` compares average output with that peak: it is a gap to peak, not a measure of unmet energy.

### 3. Currency Demonetization

The 2021 unification fixed an official rate that the informal market abandoned, and hard-currency retail split the economy in two. These figures come from the decree text and from named secondary sources; their verification status is listed row by row in `sources.csv`.

### 4. Capital Misallocation under GAESA

ONEI's investment tables for 2023 and 2024 put hotels and restaurants plus business services and real estate at about a third of all investment, agriculture near 3% and health near 2% (as quoted from ONEI; see the check on `investment_by_activity` in `sources.csv`). The video's 2020-2024 average is not yet confirmed, and the GAESA attribution is the channel's reading, not an ONEI category. `data/capital_investment_allocation_onei.csv` lists the named shares and an explicit remainder.

## What is here

| File | What |
|---|---|
| `sources.csv` | every on-screen figure and every fetched dataset: beats, claim, figures, source, tier, retrieval date, status and notes |
| `sources.json` | the same rows with every field (exact on-screen badge, URL, raw file, sha256) |
| `data/*.csv` | clean series and tables used by the charts |
| `data/raw/<publisher>/` | the raw extracts as downloaded (Cuba rows only) with `.meta.json`: URL, retrieval time, sha256 of the full download |
| `checksums.sha256` | sha256 of every file in this folder |

| Data file | Source |
|---|---|
| `data/population_trajectory_2015_2025.csv` | World Bank, World Development Indicators (SP.POP.TOTL), based on UN World Population Prospects |
| `data/electricity_generation_2000_2024.csv` | Ember, Yearly Electricity Data (CC BY 4.0) |
| `data/sugar_harvest_collapse_1961_2023.csv` | FAO, FAOSTAT Crops and livestock products (QCL), item 'Raw cane or beet sugar (centrifugal only)' |
| `data/capital_investment_allocation_onei.csv` | ONEI, Anuario Estadístico de Cuba |

## Verification status

Not every figure in the video has been verified to the same standard, and this dossier says which is which.

| Status | Rows in `sources.csv` | Meaning |
|---|---|---|
| `fetched` | 3 | Fetched by the pipeline from the publisher's API or bulk file; raw extract and sha256 included here. |
| `checked_secondary` | 1 | Checked against reporting that quotes the primary source (the primary itself could not be retrieved); see the check notes. |
| `checked_mixed` | 6 | Checked: some figures confirmed, others not found or different; the check notes say which. |
| `outdated` | 1 | Was right for an earlier date; the current value differs materially (check notes give the current one). |
| `contradicted` | 2 | Checked: the source found disagrees with the figure shown on screen (check notes give what it says). |
| `not_found` | 4 | Searched; no source found for the figure. |
| `document` | 1 | The figure is the cited legal document itself (decree text); not yet re-checked against the published edition. |
| `brief_sourced` | 5 | Source named in a later production brief; figure not yet matched against the primary document. No raw snapshot. |
| `synthesis` | 2 | Tier 3 analytical framing; no figure to verify. |

Only `fetched` rows have been checked against the primary data itself: they are the downloaded data. Rows with a
`check` (any `checked_*`, `outdated`, `contradicted` or `not_found` status) record what the channel's search found,
when, and where, including where it disagrees with the video. Figures with a `brief_*` status have not been checked
yet; treat them as such. Threshold and reference columns in the data files carry their own status column.

## Source tiers

| Tier | Meaning | On-screen figures |
|---|---|---|
| 1 | Official sovereign / multilateral statistics and documents (World Bank, IMF, UN FAOSTAT, US EIA, Federal Reserve, national statistics offices) | 5 |
| 2 | Independent demographic, academic and energy-data audits (e.g. Juan Carlos Albizu-Campos, Ember) | 13 |
| 3 | Structured macro synthesis by the channel (reconstructed balance sheets, scenarios); no figure of its own | 4 |

## Method

* **Observed vs estimated.** Charts draw published annual values only; nothing is interpolated or projected. Where an
  official series and an estimate disagree (population), both are published, separately.
* **Units.** Electricity: annual TWh converted to average MW (TWh × 10⁶ ÷ 8,760). The gap to peak demand compares
  average output with a stated peak; it is not a measure of unmet energy.
* **Crossings.** `below_threshold` in the sugar table compares each year with the stated domestic-consumption
  threshold; the chart's crossing point is interpolated between the two years either side of it.
* **Reproduce.** Download from the URL in `sources.json`, filter to Cuba, and compare with `data/raw/`; the sha256 of
  the full download is in each `.meta.json`.

## Citation and reuse

Cite as: *Capital Selection, "Cuba 2030: The Anatomy of Systemic Exhaustion", Research Data Room, retrieved <date>*, at the address where you found this
folder. Credit the original publishers: World Bank (CC BY 4.0), Ember (CC BY 4.0), FAO FAOSTAT (see FAO's terms of use).
Check each provider's current terms before reuse.

*Not investment advice. Educational analysis of public data.*
