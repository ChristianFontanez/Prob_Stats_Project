# Instructor feedback on proposal

Source: feedback shared in the project conversation, dated October 13, 2026 at 3:08 p.m. This is a faithful summary, not a copy of the original submission or instructor's complete grading record. The original submitted proposal was not available in the repository.

1. Narrow the question and confirm the available data contain the needed variables. Define the budget, model-year range, and how price, fuel economy, and safety are weighted if ranking a “best” car. The instructor suggested comparing asking prices across NHTSA safety-rating categories for listings below $15,000 as one alternative.
2. Distinguish fuel economy in MPG from Craigslist `odometer`, which measures miles already driven. Identify an exact source and column for MPG if it remains in scope.
3. Remove “estimated mileage until breakdown” unless suitable data are found. A listing's odometer does not say when that particular vehicle will break down. The instructor stated the file examined did not provide mileage at sale or breakdown.
4. The safety file the instructor examined contains ordinal `OVERALL_STARS`; 5,484 of its 17,313 records had an overall rating. Determine the usable count after matching to listings. These figures are not the matched sample size.
5. Craigslist `price` is an asking price, not necessarily a transaction price. Explain the source and role of KBB estimates if used.
6. Define one observation and explain joins on make, model, and model year, including model versions; list exact names, sources, meanings, and classifications of all relevant variables.
7. Verify downloaded files actually open and contain needed columns. Give the NHTSA download link, distinguish model years from listing dates, and describe specific filters and usable counts.
8. Identify one named group contact. Discord and iMessage are communication channels, not a contact person.

The instructor described the topic as practical and interesting and explained that the deduction reflected the broad question, missing data for key variables, and an incomplete explanation of feasibility. Statistical method selection was not required at the proposal stage; the later draft and final guidelines have additional analysis requirements.

## Important file distinction

The NHTSA safety-rating file mentioned in the feedback has not been found in this repository. The NHTSA complaints file is a separate source. The NHTSA ODI complaint dictionary does describe `MILES` as mileage at failure; that does not establish remaining life for an individual listing, and may not be the file the instructor examined. Verify source, timing and missingness before using it.
