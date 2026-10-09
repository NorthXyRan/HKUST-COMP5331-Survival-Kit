# HKUST COMP5331 Materials

Study materials for **COMP5331: Knowledge Discovery in Databases** at the Hong Kong University of Science and Technology.

This archive collects homework question papers, reference solutions, and lecture slides for future students.

## Available materials

| Location | Contents |
| --- | --- |
| [HW/2019Fall](HW/2019Fall/) | Homework 1–3 and their reference solutions |
| [HW/2025Fall](HW/2025Fall/) | Homework 1–3 and their reference solutions |
| [HW/2026Fall](HW/2026Fall/) | Homework 1 question paper |
| [Slides](Slides/) | Overview, association rules, FP-tree, clustering, outliers, subspace clustering, and classification |
Semester labels refer to the material's course semester, rather than its upload date.

## Adding materials

- Put homework papers and reference solutions in `HW/<year><semester>/`, for example `HW/2026Fall/hw2.pdf` or `HW/2026Fall/hw2-sol.pdf`.
- Put original lecture files in `Slides/`.

Materials retain their original authorship; this repository does not assign a blanket license to the course documents.

## Maintainer's local workspace

The Git working tree is the existing `Comp5331` study folder. Files are used in place, without a second working copy of the materials.

The [.gitignore](.gitignore) uses an allowlist. It includes the categories above and keeps research work, personal answer files, rendered previews, conversion outputs, temporary files, and Office lock files local. New homework PDFs named `hw<number>.pdf` or `hw<number>-sol.pdf` under a semester folder are eligible for tracking. Other filenames require an intentional update to the allowlist.

Before uploading new materials, review the selected files:

```sh
git status --short
git add HW Slides README.md .gitignore
git diff --cached --stat
git commit -m "Add course materials"
git push
```

Git stores version history in `.git/`; the original working files stay in their current locations.
