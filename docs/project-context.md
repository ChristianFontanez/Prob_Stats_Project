# Current project context

Snapshot based on the group discussion and repository review through October 31, 2026. Treat working assumptions as provisional and verify the repository and issues for later changes.

## Group, question, and work

- Group members: Ava, Thomas, Christian. A named instructor contact still needs confirmation.
- The final research question has **not** been confirmed; track [issue #1](https://github.com/ChristianFontanez/Prob_Stats_Project/issues/1). A previously suggested candidate compares asking price and odometer mileage by model year for listings below $15,000. It is an option, not an approved group decision.
- Ava leads the universal clean dataset. Christian and Thomas independently perform exploratory analyses of the same frozen dataset, then compare overlap and differences. See [roadmap](../ROADMAP.md) for dependencies and proposed remaining responsibilities.
- Draft: November 16, 2026; presentation: December 1, 2026; final written group report and separate individual reflections: December 14, 2026 at noon Eastern, with no late submissions. Confirm draft/presentation submission times and presentation requirements on Canvas.

## Available files and sources

| Repository file | Intended contents |
|---|---|
| `craigslist_clean_2000_2020.csv.zip` | Cleaned individual Craigslist listings, with `price`, `year`, `manufacturer`, `model`, `odometer`, `posting_date`, and other fields. |
| `listings_with_complaints.csv.zip` | Listings joined to complaint summaries by make, model and model year. |
| `complaint_reasons_by_model_year.csv` | Complaint record counts and category benchmarks by make, model, model year and reason. |
| `reason_benchmarks.csv` | Category-level benchmarks. |
| `carsfull.py`, `complain_clean.py`, `Breakdownreasons.py` | Earlier Python cleaning, matching and aggregation scripts. Read before interpreting derived columns. |

Original sources: [Kaggle Craigslist listings](https://www.kaggle.com/datasets/austinreese/craigslist-carstrucks-data), [NHTSA ODI complaints catalog](https://catalog.data.gov/dataset/nhtsas-office-of-defects-investigation-odi-complaints), and [ODI complaint field dictionary](https://static.nhtsa.gov/odi/ffdd/cmpl/CMPL.txt). `CMPL.txt` is a data dictionary, not the complaint data itself. The repository's earlier scripts refer to `FLAT_CMPL.zip` as an input; obtain its actual download URL and version when documenting or rebuilding the analysis.

Earlier inspection found 186,685 cleaned listings, model years 2000–2020, with posting dates April 4–May 4, 2021; 113,232 had asking prices below $15,000. These are historical checks of the earlier files, not the final analysis sample or proof of a valid match. Rerun counts on Ava's released version and document filters and version.

## Interpretation and quality checks

- A listing price is an asking price. `odometer` is miles driven, not fuel economy. The listed CSVs do not provide KBB valuations, MPG or NHTSA `OVERALL_STARS`.
- Complaint records describe reported safety issues, not crash-test star ratings or the probability of breakdown. Counts lack a denominator for vehicle exposure and can reflect vehicle popularity, age, reporting and repeat component records. A z-score or complaints per listing does not fix those limitations.
- `median_fail_miles` summarizes positive reported failure mileages for complaints matching a make/model/year. It cannot estimate a particular listed vehicle's remaining life.
- The existing join code fills missing complaint counts with zero. `matched_to_nhtsa` identifies a model-name match, not necessarily a successful make-model-year complaint match. Preserve unresolved matches distinctly from verified zero values, and assess ambiguous model prefixes and vehicle versions.
- The complaint script counts rows; the ODI dictionary warns the `ODINO` reference can repeat for components. Define the counting unit. Check complaint date relative to listing date before any historical interpretation.
- The reason benchmark code calculates `ratio_to_avg_count = n_complaints / avg_count_per_model_year`. Its comparison population is make/model/year combinations represented in the complaint data; it is not a vehicle failure rate.
- The Craigslist sample and repeated listings/model-years raise selection and independence concerns. State limits on generalization and avoid causal claims.

## Research and sources not yet integrated

The group discussed KBB values and safety-star ratings, but neither is supplied in the existing listing file. A historical KBB value needs a contemporaneous source and appropriate vehicle matching; no such source has been joined. The safety data mentioned by the instructor needs identification, matching, and a usable-sample check. Do not fabricate availability, outputs, statistical conclusions, or a confirmed final question.
