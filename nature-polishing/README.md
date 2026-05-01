# `nature-polishing` skill

An academic-writing skill for polishing, restructuring, and translating manuscript prose into concise `Nature`-leaning English.

This version was expanded using:

- close reading of sampled `Nature` papers
- a scientific English writing course
- the 2023 `Academic Phrasebank` PDF supplied locally by the user

## What changed

- The skill is now `move-based`, not just rule-based.
- Section-specific rhetoric is separated from style guardrails.
- Phrasebank-style support for gaps, literature positioning, results phrasing, cautious interpretation, conclusions, and abstracts has been added.
- The main `SKILL.md` is shorter and more executable.
- Reusable reference files now hold the larger phrase inventories.

## File structure

```text
nature-polishing/
├── SKILL.md
├── README.md
└── references/
    ├── phrasebank-playbook.md
    ├── section-moves.md
    └── style-guardrails.md
```

## When to use

- polishing an abstract, introduction, results, discussion, conclusion, or title
- translating Chinese academic text into publishable English
- tightening section logic before submission
- softening overclaims and fixing evidence-weighted language
- making prose read more like strong journal English without inventing content

## Design intent

The skill should:

- preserve facts and citation intent
- improve rhetorical sequencing at paragraph level
- keep sentences short and readable
- use stronger phrase families for section-specific writing tasks
- avoid generic AI prose and unsupported claims

## Reference map

- `section-moves.md`: section order and move patterns
- `phrasebank-playbook.md`: hedging, transitions, evidence, limitations, future work
- `style-guardrails.md`: British style, articles, abbreviations, units, register, overclaim control

## Notes

- The skill is designed for polishing and restructuring, not for fabricating scientific content.
- The reference files are intentionally selective. They are meant to guide choices, not to encourage boilerplate copying.
