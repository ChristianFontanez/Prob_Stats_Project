# Used Vehicle Analysis — MAT 219

Fall 2026 group project by **Ava, Thomas, and Christian**. We are studying used-vehicle asking prices using Craigslist listings and NHTSA complaint summaries. The final research question is being confirmed in [issue #1](https://github.com/ChristianFontanez/Prob_Stats_Project/issues/1).

## Start here

- [Kanban board](https://github.com/users/ChristianFontanez/projects/4)
- [Roadmap and responsibilities](ROADMAP.md)
- [Assignment guidelines, instructor feedback, and project context](docs/README.md)
- [Issues](https://github.com/ChristianFontanez/Prob_Stats_Project/issues) · [Milestones](https://github.com/ChristianFontanez/Prob_Stats_Project/milestones)

## Deadlines

| Deliverable | Due |
|---|---|
| Draft PDF, R Markdown and data | November 16, 2026 |
| Presentation | December 1, 2026 |
| Final report, code/data and separate individual reflections | December 14, 2026, **noon Eastern** |

## Data and workflow

- `craigslist_clean_2000_2020.csv.zip`: individual listings for model years 2000–2020, posted April–May 2021.
- `listings_with_complaints.csv.zip`: listings with make-model-year complaint summaries.
- `complaint_reasons_by_model_year.csv` and `reason_benchmarks.csv`: complaint categories and comparison summaries.
- Existing Python scripts document earlier preparation. Ava is preparing the shared dataset in R; Christian and Thomas will explore the same version independently and compare findings. Reproducible R loading instructions will accompany that release.

Prices are asking prices. Odometer means miles driven. Complaint counts are not safety ratings or failure probabilities; reported failure mileage does not predict remaining vehicle life. Do not assume KBB values or MPG are present.

## Collaboration

Choose a ready issue, follow its checklist, and request review before closing it. Route shared-data changes through Ava so both analyses use the same version. Future work and submission requirements are in the roadmap.

This repository preserves the Git history and files from [Thomas’s original project](https://github.com/Thomasbtt25/Prob_Stats_Project). The original remains intact. Collaborator invitations provide read/write access after acceptance; personal GitHub repositories do not support additional repository admins.
