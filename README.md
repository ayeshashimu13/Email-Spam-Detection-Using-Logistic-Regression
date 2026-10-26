# Email Spam Detection Using Logistic Regression

Fits logistic regression to email metadata, diagnoses separation, and compares classification thresholds.

Original results: final-model AIC 1851.74 versus 2376.02 for the simple model. Spam recall increases from about 10% at threshold 0.50 to 39% at 0.30. These are training-data results, not held-out performance.

## Run

Requires Python 3 and the original dataset.

```sh
python -m venv .venv
source .venv/bin/activate
python -m pip install -r requirements.txt
python -m jupyter lab
```

Place `email.csv` in `data/`, then open `email_spam_analysis.ipynb` and run cells in order from the repository root. Dependencies are unpinned; saved results reflect the original environment, and numerical details may vary by version.

## Scope and provenance

Adapted from the author’s original email-spam analysis notebook. Original modelling steps, statistical summaries, figures, and interpretations are preserved; added headings explain the workflow and limitations. Machine paths, installation logs, raw-row saved previews, empty cells, and a duplicate AIC-print cell were removed.

Intermediate convergence failures and undefined standard errors are preserved as part of the separation investigation. All classification metrics use the fitting data. Further validation is required before deployment.

## Data and rights

Datasets are not included: no redistribution license was found alongside the local data files. Obtain data from an authorized source. Saved derived statistical outputs are retained; source CSVs and raw-row previews are excluded. No license is granted for third-party materials.
