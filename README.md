# LangChain Corporate Contribution Analysis — Data

Supporting datasets for a term paper on corporate motivations for contributing
to free and open-source software (FOSS), using the LangChain ecosystem as a
case study.

**Research question:** What are the business cases and rational motivations for
organisations to invest in contributing to FOSS projects?

## Datasets (`data/`)

| File | Description |
|------|-------------|
| `contributors.csv` | Per-contributor records across all LangChain repos: repo, GitHub username, commit count, self-reported company field, email domain, and classified affiliation. |
| `repo_contribution_provenance.csv` | Per-repo split of commits into **host** (LangChain Inc.), **external** (other corporations), and **independent** contributors, with counts and percentages. |
| `repo_contribution_concentration.csv` | Per-repo concentration and dominance metrics, including host share, number of external companies, and bus-factor style measures (developers/companies accounting for 80% and 50% of commits). |
| `repo_top_companies.csv` | Per-repo ranking of contributing companies by commit count and commit share. |

## Notes on classification

Affiliations are classified in three tiers: **Confirmed**, **Inferred**, and
**Unaffiliated**. Some affiliations are inferred from context (e.g. commit
email domains, profile signals) rather than explicit profile data and should be
read as best-effort estimates.
