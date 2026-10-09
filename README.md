# HKUST COMP5331 Materials

Study materials for **COMP5331: Knowledge Discovery in Databases** at the Hong Kong University of Science and Technology.

This archive collects homework question papers, reference solutions, lecture slides, classroom written notes, and past-exam resources for future students.

## Available materials

| Location | Contents |
| --- | --- |
| [HW/2019Fall](HW/2019Fall/) | Homework 1–3 and their reference solutions |
| [HW/2025Fall](HW/2025Fall/) | Homework 1–3 and their reference solutions |
| [HW/2026Fall](HW/2026Fall/) | Homework 1 question paper |
| [Slides](Slides/) | Overview, association rules, FP-tree, clustering, outliers, subspace clustering, and classification |
| `COMP5331-WrittenNotes-*.pdf` | Classroom written notes dated September 11 and 12, 2026 |
| [Exams](Exams/) | Links to 2019 and 2020 final-exam pages; no exam PDFs have been archived yet |

See [SOURCES.md](SOURCES.md) for source links and provenance. Semester labels refer to the material's course semester, rather than its upload date. Lecture coverage and assessment formats can change between semesters.

## Adding materials

- Put homework papers and reference solutions in `HW/<year><semester>/`, for example `HW/2026Fall/hw2.pdf` or `HW/2026Fall/hw2-sol.pdf`.
- Put original lecture files in `Slides/`.
- Put past-exam PDFs in `Exams/<year><semester>/`, for example `Exams/2020Fall/final.pdf`.
- Record the source URL, semester, and whether a solution is official or student-written in [SOURCES.md](SOURCES.md).

Materials retain their original authorship; this repository does not assign a blanket license to the course documents.

## Maintainer's local workspace

The Git working tree is the existing `Comp5331` study folder. Files are used in place, without a second working copy of the materials.

The [.gitignore](.gitignore) uses an allowlist. It includes the categories above and keeps research work, personal answer files, rendered previews, conversion outputs, temporary files, and Office lock files local. New homework PDFs named `hw<number>.pdf` or `hw<number>-sol.pdf` under a semester folder are eligible for tracking. Other filenames require an intentional update to the allowlist.

Before uploading new materials, review the selected files:

```sh
git status --short
git add HW Slides Exams README.md SOURCES.md .gitignore
git diff --cached --stat
git commit -m "Add course materials"
git push
```

Git stores version history in `.git/`; the original working files stay in their current locations.
