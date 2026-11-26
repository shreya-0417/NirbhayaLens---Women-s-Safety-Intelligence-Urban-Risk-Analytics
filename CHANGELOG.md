# Changelog

All notable changes to this repository are documented here. The format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/) and the project uses [Semantic Versioning](https://semver.org/).

## [Unreleased]

## [1.0.0] — 2026-11-26

First public release of the migrated and rebranded repository.

### Added

- `README.md` rewritten as a full project document: overview, problem statement, objectives, features, stack, architecture, screenshots, dataset attribution, methodology, EDA, SQL and Python notes, statistical methods, dashboard guide, verified key findings, installation, execution, structure, dependencies, limitations, roadmap, credits and licence.
- `docs/architecture.mmd` — editable Mermaid source for the pipeline diagram.
- `docs/architecture.png` — exported architecture diagram.
- `screenshots/` — genuine dashboard captures (`dashboard-overview`, `dashboard-kpis`, `dashboard-analysis`, `dashboard-details`, `dashboard-trends`).
- `CONTRIBUTING.md`, `CHANGELOG.md`, an MIT `LICENSE` and a `NOTICE` file recording authorship attribution and the datasets' provenance and terms.
- `.gitignore` entries for virtual environments, local env files and notebook checkpoints.

### Changed

- Project rebranded to **NirbhayaLens — Women's Safety Intelligence & Urban Risk Analytics** throughout the documentation.
- Dashboard workbook renamed `powerbi/womens_safety_dashboard.pbix` → `powerbi/nirbhyalens_risk_dashboard.pbix`.
- PDF export renamed `outputs/womens_safety_dashboard.pdf` → `outputs/nirbhyalens_dashboard.pdf`.
- Dashboard screenshots moved out of `outputs/screenshots/` into the top-level `screenshots/` directory with descriptive filenames.
- Repository metadata, install and execution instructions updated for the new repository URL and a Python 3.11 environment.

### Fixed

- Documentation corrected against the committed data: the previous claim of "45+ districts classified as Critical Red Zones" is not supported by the results. No district reaches the 75-point threshold; the documented findings now reflect the actual tier counts (99 HIGH / 629 MODERATE / 251 LOWER in 2024) and the observed index behaviour.
- Removed the stale clone URL pointing at the previous repository.
- Corrected the documented screenshot filenames so every image reference resolves.

### Preserved

- Both analytical notebooks, unchanged in logic.
- All raw datasets, cleaned master CSV, SQLite database and analytical marts.
- The Power BI report and its PDF export.
- Original authorship credit to Diyashi Roy.

## Provenance

The analytical implementation, datasets and dashboard in this repository originate from Diyashi Roy's women's safety analysis project. Version 1.0.0 is a migration, rebranding and documentation rebuild of that work; it does not claim the analysis was independently developed here.
