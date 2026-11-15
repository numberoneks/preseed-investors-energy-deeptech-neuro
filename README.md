---
license: cc-by-4.0
pretty_name: US Pre-Seed Investors in Energy, Deeptech, Hardware and Neuroscience (2026)
language:
- en
tags:
- venture-capital
- pre-seed
- investors
- deeptech
- climate
- energy
- neuroscience
- biotech
- new-york
size_categories:
- n<1K
task_categories:
- tabular-classification
---

# NYC and US pre-seed investors in energy, deeptech, hardware and neuroscience (2026)

This is an open list of **152 venture funds** that write pre-seed checks in energy, deeptech, hardware, climate, materials, biotech, medtech and neuroscience. 52 of them are based in New York City. Every row has a public source URL.

**Publish targets (not created yet; each needs Kunal's yes and his own sign-in):**
- **GitHub repo:** `numberoneks/preseed-investors-energy-deeptech-neuro`
  Description: `Open CSV of 150+ US pre-seed investors in energy, deeptech, hardware and neuroscience. Stage, check size, HQ, sectors and a source URL on every row. NYC-heavy. CC BY 4.0.`
  Topics: `venture-capital, pre-seed, investors, deeptech, climate-tech, energy, neuroscience, biotech, nyc, open-data`
- **Hugging Face dataset:** `numberoneks/preseed-investors-us-2026`
  Description: `152 US pre-seed venture funds in energy, deeptech, hardware, climate, biotech and neuroscience, with stage, check range, HQ, sectors and a source URL per row (Nov 2026).`
- The GitHub account `numberoneks` matches Kunal's X handle (P2002 on Wikidata Q141795945). Whether that GitHub account exists or belongs to him is **UNVERIFIED**, so use whichever account he actually owns.

## Files
| File | What it is |
|---|---|
| `preseed_investors_us_2026.csv` | The dataset (152 rows, UTF-8) |
| `preseed_map_2026.md` | "The 2026 Pre-Seed Map", Kunal's authored and ranked top 50 plus his two disclosed funds |
| `url_status_2026-11-14.tsv` | curl status for every URL in the CSV, checked 2026-11-14 |

## Columns
| Column | Meaning |
|---|---|
| `name` | Fund name, as the source lists it |
| `url` | Fund website (normalized to https) |
| `hq` | Headquarters city, as the source lists it |
| `stages` | The stages the source says the fund invests in (all rows include Pre-Seed) |
| `check_range` | Average or typical check, as the source lists it |
| `sectors` | Sectors the source lists, separated by semicolons |
| `source_url` | Public page the row was taken from |
| `notes` | Empty except on the two self-reported rows |

## How it was built
1. On 2026-11-14 we ran 105 founder questions, such as "pre-seed energy investors" and "who funds neuroscience startups", and counted which pages the answers cited (`../../founder/`).
2. VC Sheet was the third most-cited domain (34 of 105 queries). Its sheets for NYC-focused funds, funds that lead pre-seeds, deeptech, climate and biotech were among the most-cited single pages.
3. We pulled every fund profile on those five sheets (328 funds). We kept funds whose listed stages include Pre-Seed, whose sectors include at least one of energy, deeptech/hardware, climate, materials, chips, robotics, space, defense, biotech, medtech, health or bio, and whose HQ is in the US.
4. Two rows are **self-reported** by the funds: Prithvi Ventures and Ayuh Ventures, both managed by the dataset's author, Kunal Sethi. That is disclosed in `notes`, and their source is each fund's own site.

## Limits
- Check sizes and stages are what VC Sheet shows; funds change them. Confirm with the fund before pitching.
- No contact emails are included, by design.
- The facts (name, stage, check size, HQ, sectors) come from VC Sheet profiles; no descriptions are copied into the CSV. The Map quotes short VC Sheet summaries with attribution. Read VC Sheet's terms before publishing (https://www.vcsheet.com/terms-of-use, 200). Whether those terms allow redistribution is UNVERIFIED.
- License: CC BY 4.0. Attribution: "Kunal Sethi, 2026 Pre-Seed Map, from public VC Sheet profiles".

## Citation
```
@misc{sethi2026preseed,
  title  = {US Pre-Seed Investors in Energy, Deeptech, Hardware and Neuroscience},
  author = {Kunal Sethi},
  year   = {2026},
  note   = {Open dataset, CC BY 4.0}
}
```
