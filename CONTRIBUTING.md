# Contributing

Thanks for taking an interest in NirbhayaLens. This is a portfolio analytics repository, but corrections and improvements are welcome.

## Reporting an issue

Open an issue with:

- what you expected and what happened,
- the file or notebook involved,
- for data issues, the district/state/year and the value you believe is wrong,
- for dashboard issues, the page and visual name.

Please do **not** open issues containing personal data or scraped records about identifiable individuals.

## Proposing a change

1. Fork the repository and create a branch: `git checkout -b fix/justice-gap-nulls`.
2. Keep the change scoped — one topic per pull request.
3. Preserve the analytical trail: if you change a metric, document the reason in the notebook markdown and update the affected section of `README.md`.
4. Re-run the affected notebook end to end so the committed CSV marts match the code.
5. If you regenerate a dashboard screenshot, replace the file in `screenshots/` and keep the same filename.
6. Update `CHANGELOG.md` under `## [Unreleased]`.

## Data and provenance

- Do not add datasets that are not published by an official source, and do not commit personal or scraped individual-level data.
- Keep `data/raw/` immutable: cleaning logic belongs in `notebooks/01_data_cleaning.ipynb`, never in edits to the source files.
- New metrics must be reproducible from committed files and must not be described as validated results without a stated method.

## Style

- Python: PEP 8, pandas idioms, no hard-coded absolute paths in committed code (the notebooks use a single `BASE_DIR` constant — keep it that way).
- SQL: uppercase keywords, one clause per line, comments explaining the business question.
- Documentation: Markdown, one `#` heading per file, no fabricated statistics.

## Attribution

Contributions are accepted under the repository's [MIT licence](LICENSE). The original analysis is credited to Diyashi Roy; keep that attribution intact in derived documentation.
