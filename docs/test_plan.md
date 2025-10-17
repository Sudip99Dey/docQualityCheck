# Test Plan — MyApp Documentation — v1.0

## 1. Scope & Objectives

Define the quality checks for MyApp documentation. Out of scope: product code.

## 2. Test Items

- docs/user_manual.md

## 3. Approach

- Review-based testing via GitHub PR (two peers)
- Automated checks: markdownlint, codespell, Vale (CI)

## 4. Environment

- Repo: docQualityCheck
- Branching: feature/* for changes; main protected
- CI workflow: .github/workflows/doc-quality.yml
- Collaboration tool: HackMD / Google Docs (versioning enabled)

## 5. Test Cases / Checklist

- TC-01: Headings surrounded by one blank line (markdownlint clean)
- TC-02: Lists separated by blank lines (markdownlint clean)
- TC-03: No typos (codespell clean)
- TC-04: Style OK; terminology consistent (Vale alerts at warning or below)
- TC-05: Single H1; hierarchical headings
- TC-06: Links and examples, if any, are valid

## 6. Roles & Responsibilities

- Author (You): create/update docs, open PR, fix feedback
- Reviewer A/B: review clarity/completeness, formatting/terminology
- Collaborator: co-edit test plan, help resolve conflicts

## 7. Schedule

- Collaboration window: <date/time>
- PR window: <date>
- Merge target: <date>

## 8. Risks & Mitigations

- Conflicting edits → use suggestions/comments, agree on sections
- Noisy rules → tune `.vale.ini` or `.markdownlint.json` minimally

## 9. Version Control Notes

- Link PR(s) and latest passing CI run

## 10. Results & Sign-off

- Summary of issues found/resolved
- Final approval note
