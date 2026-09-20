# public-funding-applications-writing-style

A Claude Agent Skill for writing, rewriting and compliance-checking applications for public or publicly-accountable funding.

It covers government departments, statutory bodies, and — importantly — the quasi-government intermediaries that actually administer most public money: science parks, productivity councils, incubators, R&D centres, trade and development bodies, industry associations, arts and film councils, public trusts and corporate foundations.

The skill is scheme-agnostic and jurisdiction-agnostic. It contains no scheme names, no weighting tables and no funding amounts, because those go stale and a wrong one in a submitted application is expensive. What it contains is the method those specifics were evidence for.

## The premise

Every body in this genre is spending money it must account for to someone else — a legislature, an auditor, a board, a donor, a parent ministry.

That single fact produces the behaviour you are writing into, and it is the same whether the letterhead says Commission or Corporation:

- The reviewer needs a **defensible** reason to score you high, not a correct one. They are writing a file note someone may read later.
- They score against a rubric and stay inside it. Brilliance outside the rubric does not help.
- They will not do work you left undone. A requirement you made them infer may be marked unmet.
- They mostly cannot be appealed and rarely explain a rejection usefully.
- Panels are mixed-expertise by design, so that no single specialist decides. Whoever scores your technical merit may not share your field.

From which the governing principle: **never ask a non-specialist to judge the science.** Give them something else to judge that is verifiable, external to you, and points the same way — a measured result against a named baseline, an accredited test report, a customer letter, a granted patent, a named individual's publication record in the exact sub-field.

## What's in it

| Section | What it does |
|---|---|
| Reconstruct the rubric | How to derive the scoring criteria when they aren't published — the form *is* the rubric; then stated objectives, then the list of previously funded projects |
| The requirements register | One row per requirement in the guideline's own wording, with the section that satisfies it and the evidence annex |
| Two registers, stacked | Claim → mechanism → specification → evidence, in one passage, so lay and specialist readers are both served |
| Writing the plain layer | The so-what ladder, analogy discipline, sentence mechanics |
| Writing the specification layer | Match the complexity of the subject — precision as the authority signal rather than density |
| Clearing stated requirements | Mirror the guideline's vocabulary; the highlight test |
| Scope discipline | Don't open threads you'll have to defend — and where that stops, which is disclosure |
| Winning the subjective criteria | The evidence stack that lets a lay reviewer score merit high without evaluating any science |
| Writing for an intermediary | The body's own mandate is usually the hidden top criterion |
| The compliance interrogation | Questions to put to any guideline; the answers vary, the questions don't |
| Failure modes | Deemed withdrawal, no appeal, thin feedback, resubmission as a designed process |
| Operating modes | Draft / rewrite / check |

## Install

**Personal (all your projects):**

```bash
git clone https://github.com/aknopla/public-funding-applications-writing-style \
  ~/.claude/skills/public-funding-applications
```

**Project-scoped (shared with a repo's collaborators):**

```bash
git clone https://github.com/aknopla/public-funding-applications-writing-style \
  .claude/skills/public-funding-applications
```

Claude picks it up automatically from the `description` field. You can also invoke it directly with `/public-funding-applications`.

In the Claude apps, upload `SKILL.md` as a skill instead.

## Scope

The skill will not inflate technical complexity to deter scrutiny, and will not let the plain layer claim more than the specification supports. Both are in there as craft guidance rather than as rules imposed on it: manufactured density doesn't produce deference, it produces a low "insufficiently justified" score or a referral to an external expert, and a gap between the layers surfaces during the presentation, the panel-comment round, or the audit — whichever comes first.

## Contributing

The parts most likely to need work from real use are the intermediary section, which is written from how these bodies are structurally accountable rather than from experience of dealing with them, and the compliance interrogation, which will grow as new disclosure regimes appear. Issues and PRs welcome.
