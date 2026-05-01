# 09 — GitHub Setup

## Repository
- Name: healsound
- URL: https://github.com/(yourusername)/healsound
- Visibility: Public

## Folder Structure
healsound/
├── README.md
├── docs/          ← all pre-production documents
├── src/           ← all Python source code
├── data/          ← dataset notes (not raw data)
├── models/        ← saved .pt model files
├── notebooks/     ← Jupyter exploration notebooks
├── demo/          ← Gradio app files
└── reports/       ← final report PDF and slides

## Commit Convention
- docs: → documentation changes
- feat: → new feature added
- fix:  → bug fix
- train: → model training runs
- data: → dataset changes

## Branch Strategy
- main → stable, working code only
- dev  → active development
- Always merge dev into main after testing
