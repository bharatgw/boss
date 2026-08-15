# SMU module-bidding analysis

> Historical portfolio project. The data and models reflect the period in which the project was created and should not be treated as current bidding advice.

## Overview

This project explores historical SMU BOSS bidding results using descriptive statistics and regression models. It studies how variables such as vacancies, bidding windows, course offerings, and instructor information relate to historical minimum and median bids.

The strongest model reported in the original analysis was a random forest with an approximate out-of-sample R² of 0.65. That result is descriptive of the historical dataset and does not guarantee future bidding outcomes.

## Repository contents

| Path | Purpose |
| --- | --- |
| [`bidding.py`](./bidding.py) | Combines term-level BOSS Excel exports into [`overall.csv`](./overall.csv). |
| [`overall.csv`](./overall.csv) | Historical combined dataset used by the notebook. |
| [`analysis.ipynb`](./analysis.ipynb) | Data cleaning, visualisation, and modelling workflow. |
| [`DATA_NOTES.md`](./DATA_NOTES.md) | Dataset construction, variable dictionary, and interpretation limits. |

## Historical workflow

1. Download the relevant term-level BOSS Overall Results spreadsheets.
2. Place them in the working directory using the filename pattern expected by [`bidding.py`](./bidding.py), such as `2015-16_T1.xls`.
3. Run [`bidding.py`](./bidding.py) to generate [`overall.csv`](./overall.csv).
4. Open [`analysis.ipynb`](./analysis.ipynb) and run the analysis cells.

The code was developed around a Python 3.8-era environment. It uses pandas, NumPy, Matplotlib, and scikit-learn. Current compatibility has not been verified; in particular, newer pandas releases removed APIs used by the original aggregation script.

## Data provenance and responsible use

The combined data was derived from SMU BOSS Overall Results published through the university's student portal. [`overall.csv`](./overall.csv) is retained as a historical project artifact. Anyone reusing the data should independently confirm the source's current access conditions, permitted uses, definitions, and update history.

The analysis is informational. It does not account for every factor affecting module allocation and should not be used as a guarantee of admission to a course.

## License and reuse

No open-source license has been applied. The project is shared for viewing as portfolio work. The underlying university data remains subject to its source terms.