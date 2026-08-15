# Data notes

## Source and construction

`overall.csv` is a historical combined dataset produced from SMU BOSS Overall Results spreadsheets. The original aggregation script expects term files named using patterns such as `2015-16_T1.xls` and appends the available academic years and terms.

The tracked CSV is retained so that the saved notebook can be inspected as a portfolio artifact. Before reusing or refreshing it, confirm the university source's current access conditions, permitted uses, definitions, and coverage.

## Variable dictionary

| Variable | Description |
| --- | --- |
| `term` | Academic term, such as Term 1, Term 2, Term 3A, or Term 3B. |
| `session` | Academic-year session. |
| `bidding_window` | Bidding round and window. |
| `course_code` | Course code. |
| `description` | Course title. |
| `section` | Class section. |
| `vacancy` | Total class vacancies. |
| `opening_vacancy` | Vacancies at the opening of the first bidding window. |
| `before_process_vacancy` | Vacancies before a bidding window was processed. |
| `dice` | Recorded D.I.C.E. value from the source export. |
| `after_process_vacancy` | Vacancies after a bidding window was processed. |
| `enrolled_students` | Number of enrolled students. |
| `median_bid` | Median successful bid for the class and window. |
| `min_bid` | Minimum successful bid for the class and window. |
| `instructor` | Instructor listed for the section. |
| `school` | School or department offering the course. |
| `year` | Academic year used in the analysis. |

## Interpretation limits

The data is observational and tied to historical bidding rules and course offerings. Model predictions may reflect omitted factors and changes in policy, demand, curriculum, or data definitions. They should not be treated as guarantees of future bidding outcomes.
