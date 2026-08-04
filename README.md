# Bioinformatics MSc Study Repository

My organised workspace for learning bioinformatics during my master's degree. It combines course notes with reproducible analysis projects and references.

## Current course

[Intro to Bioinformatics — Mike Saint-Antoine](https://www.youtube.com/playlist?list=PLWVKUEZ25V95IKyBrxHtRTK_6Ig8Xi9-f) (26 videos)

| Area | Location |
| --- | --- |
| Course notes | `Study_Notes/` |
| Differential-expression project | `02_projects/differential_expression/` |
| GWAS project | `02_projects/gwas/` |
| Reusable notebooks | `notebooks/` |
| Reusable scripts | `scripts/` |
| References and glossary | `03_reference/` |

## Study workflow

1. Create one note per lesson in `Study_Notes/`.
2. Record commands, data sources, results, and interpretation in the relevant project folder.
3. Keep raw datasets out of Git; document how to download them instead.
4. Save final figures and short reports in `reports/`.

## Local setup

```powershell
conda env create -f environment.yml
conda activate bioinformatics-study
```

The environment is deliberately small. Add specialist packages only when a course project requires them.

## Data policy

`data/raw/`, `data/interim/`, and `data/processed/` are ignored by Git. Each analysis should include a small README that states the source, download date, and any transformations needed to recreate its data.
