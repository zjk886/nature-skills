---
name: nature-polishing
description: Polish, restructure, or translate academic prose into Nature-leaning English using section-specific rhetorical moves, writing-strategy constraints, calibrated hedging, and strict sentence-level clarity. Use whenever the user asks to polish a manuscript paragraph, abstract, introduction, results, discussion, conclusion, title, or Chinese academic draft for publication-quality English, especially when they mention Nature style, scientific English, academic polishing, or journal-ready prose.
version: 4.0.0
author: Yuan1z skill refined with Nature-paper analysis and Academic Phrasebank (2023)
---

# Nature-Style Academic Polishing

Use this skill to improve language, structure, and rhetorical control in academic writing. The target style is `Nature`-leaning English: concise, evidence-weighted, and section-aware. The goal is not to imitate a journal mechanically. The goal is to make the prose read like strong publishable science.

## Default stance

- Preserve the author's factual meaning, quantitative values, and citation intent.
- Do not invent data, references, mechanisms, or novelty claims.
- Diagnose the writing task before rewriting: section, intervention depth, and whether the draft is translation-heavy.
- Prefer short declarative sentences with one main proposition each.
- Use phrase families as scaffolds, not as copy-paste boilerplate.
- If the science is ambiguous, keep the language accurate and restrained rather than guessing.

## When to open extra files

| File | Open when |
|---|---|
| [references/writing-strategy.md](references/writing-strategy.md) | You are polishing a full paragraph, section, abstract, or Chinese draft and need the high-level writing logic: hourglass structure, section responsibilities, claim-evidence-boundary control, or citation positioning |
| [references/section-moves.md](references/section-moves.md) | You need section-specific move order or phrase patterns for Introduction, Literature Review, Methods, Results, Discussion, Conclusion, Abstract, or Title |
| [references/phrasebank-playbook.md](references/phrasebank-playbook.md) | You need help with hedging, evidence strength, transitions, paragraph linking, limitations, or future-work phrasing |
| [references/style-guardrails.md](references/style-guardrails.md) | You need Nature/British style checks, article usage, abbreviations, units, register, or overclaim control |

## Core writing strategy

These rules stay in the core skill. Do not reduce the task to surface polishing if the writing logic is wrong.

### 1. Fix thinking before wording

- First identify what the paragraph or section is trying to do.
- If the rhetorical job is unclear, repair that before polishing sentences.
- Cosmetic polishing of a structurally wrong paragraph is failure.
- Prioritize in this order: `section logic -> paragraph logic -> claim/evidence/boundary -> sentence polish`.

### 2. Use the hourglass structure

- Scientific papers usually move `broad -> narrow -> broad`.
- Introduction sections zoom in: field -> gap -> question -> approach.
- Discussion and conclusion sections zoom out: result -> interpretation -> implication -> boundary.
- If a paragraph opens narrowly and drifts broadly without control, rebuild it.

### 3. Remember that writing order is not reading order

- Strong papers are often built from `Results -> Introduction/Conclusion -> Title -> Discussion -> Methods -> Abstract`.
- When a user gives notes, data, or rough Chinese draft material, organize around evidence first rather than around the source sentence order.
- The reader should see a clean argument, not the chronology of the author's drafting process.

### 4. Force every key claim to carry evidence and a boundary

- Each important statement should answer three questions:
  - `What is the claim?`
  - `What evidence supports it?`
  - `What is the scope or limitation?`
- If the draft has claim plus enthusiasm but no boundary, add restraint.
- If the draft has data but no claim, state the point explicitly.
- If the draft has a claim but no supporting basis, soften it or mark the evidential gap.

### 5. Treat each section as a distinct intellectual task

- `Introduction`: what is known, what is unknown, what question is being asked, and how it will be addressed
- `Results`: what was observed, under which condition, and with which quantitative support
- `Discussion`: what the result means, how it relates to prior work, and when the interpretation may fail
- `Methods`: what another group would need to reproduce the work
- `Conclusion`: what the central contribution is, which evidence matters most, and what boundary or implication follows
- `Abstract`: a mini-paper, not a teaser and not a full discussion section

### 6. Handle citation as intellectual positioning, not formatting

- Distinguish support, borrowing, contrast, and reuse.
- Cite the source actually read and verified.
- Do not build novelty by turning earlier work into a straw man.
- If the paragraph depends on prior work for its logic, make that dependence explicit.

## Hard requirements

1. Keep every sentence at `<= 30` words. Prefer `12-24` words where possible.
2. If any sentence exceeds `20` words, check whether it carries more than one proposition. Split if needed.
3. Give each paragraph one controlling idea followed by support.
4. Avoid filler openings such as `It is well known that`, `It is worth noting that`, and `As a matter of fact`.
5. Use no more than one demonstrative-led sentence (`This`, `These`, `Such`) per paragraph.
6. Define abbreviations on first use unless they are standard (`DNA`, `RNA`, `ATP`, `pH`).
7. Avoid contractions, rhetorical questions, and unsupported superlatives.
8. Match claim strength to evidence. Correlation does not become causation during polishing.
9. Keep Results mainly in past tense. Keep Discussion interpretive and hedged.
10. Use British English spelling unless the user explicitly asks for another house style.

## Workflow

### 1. Diagnose the task first

Identify three things before editing:

- `Task type`: light polish, structural rewrite, Chinese-to-English translation plus polishing, abstract/title rewrite, or section-level rewriting
- `Manuscript section`: introduction, literature review, methods, results, discussion, conclusion, abstract, title, or mixed
- `Intervention level`
  - `Light`: grammar, diction, and flow only
  - `Moderate`: sentence splitting, paragraph reordering, stronger topic sentences
  - `Heavy`: rebuild the move structure while preserving all defensible content
- `Rhetorical failure`: wrong section logic, missing gap, missing evidence, overclaim, mixed Results/Discussion writing, or only sentence-level noise

If the user only says `polish this`, infer the section from tense, content, and function.

### 2. Repair section thinking before editing sentences

Check the draft against the core writing strategy:

- Does the section perform the correct intellectual job?
- Does the argument follow hourglass logic where appropriate?
- Does each important claim have evidence and a boundary?
- Are Results and Discussion improperly mixed?
- Is the contribution stated too early, too late, or without a gap statement?

If any of these fail, fix them before line-editing.

### 3. Rebuild paragraph logic before polishing sentences

Use the `controlling idea -> support` pattern:

- Start with a topic sentence that states the paragraph's function.
- Follow with support: data, mechanism, literature, comparison, limitation, or implication.
- Move new ideas into a new paragraph instead of stacking them into one.
- Use explicit thematic linking between adjacent sentences by restating the noun, using a definite noun phrase, or using a restrained connective.

Do not preserve the original sentence count if the source paragraph is overloaded.

### 4. Apply section-specific rhetoric

#### Introduction

- Move from field importance -> known background -> gap or controversy -> aim -> value.
- Make sure the Introduction answers four questions:
  - what is already known?
  - what remains unresolved?
  - what specific question is posed here?
  - how will the study address it?
- Do not dump results into the Introduction.
- Use `Here, we ...` only when it introduces the actual study aim or contribution.

#### Literature Review

- Synthesize the field rather than listing citations one by one.
- Distinguish `what is established`, `what remains debated`, and `what is missing`.
- Use fair positioning language. Never caricature prior work to make the current work look stronger.

#### Methods

- Write for reproducibility, not atmosphere.
- Another group should be able to reproduce the work from the section alone, or from the section plus a clearly cited prior protocol.
- Replace vague phrases like `under standard conditions` or `using routine methods` with actual parameters, instruments, versions, controls, and statistics.
- Keep Methods concrete and specific. Precision matters more than elegance here.

#### Results

- Report what was observed, in what system, under what condition, and with what quantitative detail.
- Refer to figures and tables directly when useful.
- Do not explain mechanism at length here unless the sentence is still reporting an observed pattern.
- Negative findings should stay precise rather than apologetic.
- Results answer `what happened`, not `what it ultimately means`.

#### Discussion

- Interpret findings, compare them with earlier work, explain plausible reasons, state limits, and note implications.
- Use hedges when moving from observation to explanation.
- Distinguish clearly between `explanation`, `speculation`, `limitation`, and `implication`.
- Make sure the Discussion addresses:
  - how the work fits the broader field
  - what it adds to understanding
  - which earlier work must be acknowledged
  - whether the findings revise, support, or complicate prior interpretations

#### Conclusion

- Use a three-part close: central contribution -> key evidence -> implication with boundary.
- Do not introduce brand-new data in the final paragraph.

#### Abstract

- Treat the abstract as a mini-paper: context -> gap -> approach -> main result -> implication.
- Keep it dense, readable, and selective. Only the most decision-relevant details belong here.
- The abstract is a summary paragraph, not a collection of disconnected highlights.

#### Title

- Prefer searchable nouns and restrained verbs.
- Avoid vague hooks, unsupported `first` claims, and technical clutter.
- If aiming for Nature style, target `<= 75` characters including spaces.
- Aim for `curiosity with credibility`: enough interest to invite reading, but every word must still be defensible by the data.

### 5. Control sentence architecture

- Prefer one main clause per sentence.
- If a sentence contains a main claim plus a participial phrase plus an `including` list, it is probably overloaded.
- Front-load the point. Move conditions and qualifiers later.
- Prefer active voice with a concrete subject when it improves clarity.
- Use passive voice when the actor is irrelevant and the result matters more.

Useful high-value patterns:

- `Here, we show that ...`
- `Using X, we found that ...`
- `These results suggest that ...`
- `A possible explanation is that ...`
- `Taken together, these findings indicate that ...`

### 6. Calibrate claims and evidence

Use three evidence levels:

- `Strong evidence`: demonstrate, show, establish, reveal, identify
- `Moderate evidence`: suggest, indicate, support the view that, are consistent with
- `Speculative extension`: may reflect, could arise from, appears to, seems likely

Before finalizing, check for:

- absolute claims such as `prove`, `conclusively`, `unprecedented`
- correlation presented as causation
- unjustified scope expansion from one model or cohort to all settings
- unsupported `first`, `best`, `superior`, or `novel` claims

### 7. Translation mode for Chinese drafts

When the source is Chinese or strongly Chinese-influenced English:

- Extract the core propositions first. Do not translate clause-by-clause mechanically.
- Supply omitted English subjects only when the reference is unambiguous.
- Convert parataxis into explicit logical relations: contrast, cause, limitation, implication.
- Break long comma-linked Chinese sentences into multiple English sentences.
- Replace repetition used for emphasis with more precise progression.
- Keep technical terms stable. Do not alternate synonyms for key scientific entities.
- When the Chinese source hides the logical relation between sentences, reconstruct that relation explicitly instead of preserving ambiguity.

### 8. Register and style guardrails

- Use British English by default.
- Avoid spoken fillers, contractions, and conversational evaluation.
- Keep nominalisation under control. A compact noun phrase is useful; a chain of five abstract nouns is not.
- Be impersonal when needed, but allow `we` in team-based science writing where it reads naturally.
- Preserve symbols, units, gene names, and statistical notation exactly unless they are clearly wrong.

### 9. Integrity checks before output

Always verify:

- every sentence length
- section-appropriate tense
- abbreviation definitions
- article usage around singular count nouns
- figure and table references
- citation placeholders or missing attribution
- whether any polished sentence overstates what the data can support
- whether the section now performs the right intellectual task

If the original text is scientifically incoherent, do not silently repair the science. Polish the language and note the unresolved issue briefly.

## Output format

Default output:

1. The polished text as plain prose, not in a code block.
2. `Revision notes:` with `3-5` short bullets on the main changes.
3. If the rewrite required major restructuring, add one short note explaining the structural change.

If the user explicitly asks for a side-by-side revision, provide:

- `Original`
- `Polished`
- `Why changed`

## What this skill now adds from Academic Phrasebank

- move-based paragraph design rather than sentence-level polishing only
- safer phrase families for gap statements, results reporting, cautious interpretation, and conclusions
- stronger handling of transitions, evidence collocations, and limitation language
- clearer separation between reporting, interpreting, and speculating
- a restored emphasis on writing strategy, not just sentence polish

Use the reference files to retrieve those patterns only when needed.
