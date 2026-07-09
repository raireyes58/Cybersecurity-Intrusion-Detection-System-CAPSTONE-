## src/

This project's core logic lives inside the main Jupyter notebook
(`notebooks/`), organized as documented, reusable functions per step
(e.g. `clean_data()`, `treat_outliers()`, `evaluate_model()`).

No standalone .py scripts are included in this folder, since the
notebook format was chosen to keep code, results, and narrative
justification together for review — but every function is written
to be copy-paste reusable outside the notebook if needed.
