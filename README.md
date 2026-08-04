# Bioinformatics MSc Study Repository

My organised workspace for learning bioinformatics during my master's degree. It combines course notes with reproducible analysis projects and references.

## Current course

[Intro to Bioinformatics — Mike Saint-Antoine](https://www.youtube.com/playlist?list=PLWVKUEZ25V95IKyBrxHtRTK_6Ig8Xi9-f) (26 videos)

| Area | Location |
| --- | --- |
| Course notes | `01_study_notes/` |
| Differential-expression project | `02_course_projects/01_differential_expression/` |
| GWAS project | `02_course_projects/02_gwas/` |
| References and glossary | `03_reference/` |

## Study workflow

1. Create one note per lesson in `01_study_notes/`.
2. Record commands, data sources, results, and interpretation in the relevant project folder.
3. Keep raw datasets out of Git; document how to download them in that project's README.
4. Keep a project's notebooks, scripts, data, and results inside that project so it can be reproduced independently.

## Local setup

```powershell
conda env create -f environment.yml
conda activate bioinformatics-study
```

The environment is deliberately small. Add specialist packages only when a course project requires them.

## Repository layout

```text
01_study_notes/                  # Notes for the current course
02_course_projects/
  01_differential_expression/    # Course project 1
  02_gwas/                       # Course project 2
03_reference/                    # Glossary and source-linked reference notes
```

## Data policy

Each project ignores its own `data/raw/` and `data/processed/` folders. Its README should state the source, download date, licence or access conditions, and transformations needed to recreate the analysis. Do not put personal, identifiable, controlled-access, or large datasets in this public repository.
