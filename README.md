# Homer

[![skills.sh](https://skills.sh/b/tanvishdesai/Homer)](https://skills.sh/tanvishdesai/Homer)

Homer is an installable agent skill for turning a rough research idea, code, and
experiment results into a structured, submission-ready academic paper draft.

The included skill is `research-paper-writing`. It guides an agent through a
five-phase workflow:

1. Orient around the contribution in plain English.
2. Analyze the target venue using five accepted papers.
3. Build a structured literature review.
4. Extract all technical details from code and results.
5. Draft and revise the paper through dedicated audit passes.

## Install

Install the skill from this repository:

```bash
npx skills add tanvishdesai/Homer --skill research-paper-writing
```

Or install from the direct GitHub path:

```bash
npx skills add https://github.com/tanvishdesai/Homer/tree/main/skills/research-paper-writing
```

## Repository Layout

```text
Homer/
├── README.md
└── skills/
    └── research-paper-writing/
        ├── SKILL.md
        ├── WRITING_RULES.md
        ├── VENUE_NOTES_TEMPLATE.md
        ├── LITERATURE_LIST_TEMPLATE.md
        ├── literature_review_template.csv
        ├── TECHNICAL_DUMP_TEMPLATE.md
        ├── README.md
        └── agents/
            └── openai.yaml
```

## Use

After installation, ask your agent something like:

```text
Use $research-paper-writing. I have idea.md and /code. Target venue: ICCV 2026.
Execute Phase 0 first and do not start Phase 1 until Phase 0 is complete.
```

The skill is designed for research paper drafting, related work synthesis,
technical extraction from experiments, and final revision passes that catch
common AI-assisted writing failures.
