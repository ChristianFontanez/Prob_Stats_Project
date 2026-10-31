# Probability and Statistics Project Roadmap

Group: Ava, Thomas, and Christian. Add full submission names before exporting reports.

This roadmap records the agreed division of data and exploratory work and proposes the remaining assignments. Intermediate dates and reviewers are planning targets for group review. The research question is not yet confirmed: resolve issue #1 before freezing the analysis dataset.

## Deadlines

| Milestone | Course deadline | Internal target |
|---|---|---|
| Draft | November 16, 2026; check Canvas for time | Complete group review November 15 |
| Presentation | December 1, 2026; time to confirm | Slides ready November 30 |
| Final group report and individual reflections | December 14, 2026, **12:00 p.m. Eastern; no late submissions** | Submit December 13 |

[Kanban board](https://github.com/users/ChristianFontanez/projects/4) · [Issues](https://github.com/ChristianFontanez/Prob_Stats_Project/issues)

## Working agreement

- Ava leads preparation of one universal clean dataset. Original inputs remain unchanged. Record filters, exclusions, missingness, duplicate rules and any joins in reproducible R code.
- Christian and Thomas each analyze the same version independently. Save observations before reading the other person's interpretations, then compare overlaps and differences.
- Analysts report data problems to Ava rather than silently applying different filters. Approved changes create a new version and both analyses rerun.
- Each issue has one lead, a reviewer, dependencies and a completion checklist. The lead records output links and verification evidence before closing it.
- Suggested board columns: Backlog, Ready, In progress, Review, Done. Record blocking issue links in each issue. Start only when dependencies are complete.
- All members review and understand the methods, code and conclusions. Assignments do not divide statistical understanding between people.

## Active issues: draft preparation and independent exploration

| Issue | Lead | Proposed target | Dependencies |
|---|---|---|---|
| [#1 Lock question and population](https://github.com/ChristianFontanez/Prob_Stats_Project/issues/1) | Christian; all approve | Nov 1 | None |
| [#2 Document sources and variables](https://github.com/ChristianFontanez/Prob_Stats_Project/issues/2) | Ava | Nov 2 | #1 |
| [#3 Prepare shared dataset in R](https://github.com/ChristianFontanez/Prob_Stats_Project/issues/3) | Ava | Nov 4 | #2 |
| [#4 Check exclusions and joins](https://github.com/ChristianFontanez/Prob_Stats_Project/issues/4) | Ava; Thomas reviews | Nov 5 | #3 |
| [#5 Freeze dataset v1 and verify loading](https://github.com/ChristianFontanez/Prob_Stats_Project/issues/5) | Ava; Christian reviews | Nov 6 | #4 |
| [#6 Christian's independent summaries](https://github.com/ChristianFontanez/Prob_Stats_Project/issues/6) | Christian | Nov 7 | #5 |
| [#7 Thomas's independent summaries](https://github.com/ChristianFontanez/Prob_Stats_Project/issues/7) | Thomas | Nov 7 | #5 |
| [#8 Christian's two exploratory graphs](https://github.com/ChristianFontanez/Prob_Stats_Project/issues/8) | Christian | Nov 8 | #6 |
| [#9 Thomas's two exploratory graphs](https://github.com/ChristianFontanez/Prob_Stats_Project/issues/9) | Thomas | Nov 8 | #7 |
| [#10 Compare findings and resolve differences](https://github.com/ChristianFontanez/Prob_Stats_Project/issues/10) | Christian and Thomas; Ava handles data fixes | Nov 9 | #8, #9 |

Ava’s confirmed GitHub account is @kava117. Thomas (@Thomasbtt25) and Ava have read/write invitations; formal issue assignments await their acceptance in this repository.

## Remaining draft work

These are roadmap tasks, not yet separate GitHub issues. Expand them after the question is confirmed and the initial work is underway.

| ID | Task and completion criterion | Lead / review | Target | Depends on |
|---|---|---|---|---|
| D11 | Select at least two labeled, explained graphs and a relevant summary table | Thomas / Christian | Nov 10 | #10 |
| D12 | Define population quantity; justify method; state hypotheses if testing; identify whether method is covered in class | Christian / Thomas | Nov 10 | #10 |
| D13 | Check conditions and attempt analysis; interpret results and identify unfinished work | Thomas / Christian | Nov 11 | D12 |
| D14 | Write data description with actual sample size, variables, preparation and sources | Ava | Nov 11 | #5; update after changes |
| D15 | Write motivation, revised question and EDA interpretation | Christian | Nov 12 | D11 |
| D16 | Write methods and preliminary findings | Thomas | Nov 12 | D13 |
| D17 | Write limitations, next steps, feedback questions and role table | Ava / all | Nov 13 | D13 |
| D18 | Assemble one commented .Rmd covering loading, preparation, graphs and analysis | Thomas | Nov 13 | D11, D13 |
| D19 | Assemble self-contained 800–1,200-word PDF with all members and six required sections | Christian | Nov 14 | D14–D18 |
| D20 | Reproduce report outputs from a fresh R session using supplied data/instructions | Ava | Nov 14 | D18, D19 |
| D21 | Group walkthrough; reconcile numbers and ensure everyone can explain the analysis | Christian coordinates; all | Nov 15 | D20 |
| D22 | Upload and verify PDF, .Rmd and data or direct download/loading instructions | Christian, provisional | Nov 16 | D21 |

Draft sections: title/group members; question and motivation; data description; exploratory analysis; statistical methods and preliminary results; preliminary conclusions and limitations; next steps, roles and feedback questions. Role table columns must be remaining task, responsible member(s), and target completion date. Word count excludes graphs, tables, code and references. Data preparation and EDA must be complete in R. Attempt taught methods; clearly explain planned untaught methods and unfinished work. Ask the professor before the deadline if method choice is uncertain.

## Presentation plan

Presentation-specific guidelines still need checking. These tasks are preparation targets, not additional course requirements.

| ID | Task and completion criterion | Lead | Target | Depends on |
|---|---|---|---|---|
| P01 | Record draft feedback with action, owner and affected section | Christian | Nov 19, or within one day of feedback | Draft feedback |
| P02 | Address data feedback; version any revised dataset | Ava | Nov 21 | P01 |
| P03 | Rerun analysis and verify conditions/results | Thomas; Christian reviews | Nov 23 | P02 |
| P04 | Agree on two or three supported findings, figures and limitations | Christian; all approve | Nov 24 | P03 |
| P05 | Draft data and limitations slides | Ava | Nov 25 | P04 |
| P06 | Draft methods and results slides | Thomas | Nov 25 | P04 |
| P07 | Assemble slides, introduction/conclusion and speaking assignments | Christian | Nov 27 | P05, P06 |
| P08 | Timed rehearsal; everyone practices answering analysis questions | Ava coordinates; all | Nov 29 | P07 |
| P09 | Finish rehearsal corrections; verify slides and backup | Christian | Nov 30 | P08 |
| P10 | Present and record questions/comments immediately afterward | All; Ava maintains notes | Dec 1 | P09 |

## Final report plan

| ID | Task and completion criterion | Lead / review | Target | Depends on |
|---|---|---|---|---|
| F01 | Combine draft/presentation feedback into an action checklist; record reasons for declining suggestions | Christian | Dec 2 | P10 |
| F02 | Freeze final data and complete preparation/loading documentation | Ava | Dec 4 | F01 |
| F03 | Complete statistical methods, condition checks and numerical results | Thomas | Dec 6 | F02 |
| F04 | Independently reproduce headline results and check interpretations | Christian | Dec 7 | F03 |
| F05 | Revise introduction and conclusions; explain practical importance | Christian | Dec 8 | F04 |
| F06 | Revise data, selected EDA and limitations sections | Ava | Dec 8 | F04 |
| F07 | Revise methods/results; explain estimates, uncertainty and hypotheses where applicable | Thomas | Dec 8 | F04 |
| F08 | Write revision note addressing important feedback and declined suggestions | Christian / all | Dec 9 | F05–F07 |
| F09 | Assemble report and audit data/source/R-package citations and figure references | Christian / Ava | Dec 10 | F08 |
| F10 | Run final .Rmd from a fresh session; verify all tables, figures and numbers | Ava; Thomas fixes code | Dec 11 | F09 |
| F11 | Group accuracy and understanding review; resolve all corrections | Thomas coordinates; all | Dec 12 | F10 |
| F12 | Submit and verify group PDF, .Rmd and data/loading instructions | Christian, provisional | Dec 13 | F11 |

Final report: 1,200–1,800 words excluding tables, figure captions, code, references and revision note. Include title and all names; introduction; data description and EDA; methods and results; discussion/conclusion; references; revision note. Number and label figures/tables and explain them in the text. There is no minimum final graph count. Report practical meaning as well as statistical uncertainty, limitations, bias, independence, generalizability and whether causal claims are justified. Significant results are not required.

The final .Rmd must load and prepare data, create summaries/graphs and run statistical analysis with comments, required packages and portable paths. Supply data or a direct download link and clear instructions. Final changes after the fresh-session check require rerunning affected checks.

## Individual submissions

| Task | Owner | Internal target |
|---|---|---|
| I01 Independently write and separately submit reflection | Ava | Dec 13 |
| I02 Independently write and separately submit reflection | Thomas | Dec 13 |
| I03 Independently write and separately submit reflection | Christian | Dec 13 |

Each reflection is 150–200 words and includes the student's name and project title. Address specific contributions/changes from planned role, one statistical decision or numerical result in context, and personal AI use and verification (or explicitly no AI use). Write independently in the student's own words, **without AI-generated text**. Do not bundle reflections into the group report. All are due December 14 at noon Eastern.

## Decisions and known limitations

- Research question: pending #1. The earlier price–odometer question is a candidate, not an agreed final scope.
- Shared-data ownership and independent exploratory work are agreed; subsequent leads, reviewers and intermediate dates are proposals.
- Existing repository files contain asking prices and complaint summaries. Do not assume KBB values, MPG or NHTSA overall safety ratings are available. Verify required variables before expanding scope.
- Model years and listing dates differ. Complaint counts are not failure probabilities, and reported failure mileage does not estimate remaining vehicle life.
- If complaint data are used, check duplicate complaint/component records, match failures, exposure denominators and complaint timing relative to listings.
- Confirm full names, exact draft/presentation times and presentation format.

## Requirement sources

- [Project Draft Guidelines (Canvas)](https://rollins.instructure.com/courses/25193/files/3582214?wrap=1)
- [Final Project Report Guidelines (Canvas)](https://rollins.instructure.com/courses/25193/files/3582223?wrap=1)
- Presentation date supplied by the group: December 1, 2026.

Planning date: October 31, 2026. Update this roadmap as the group confirms decisions and receives feedback.
