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

## The phrasebook

`references/requirement-wordings.md` is a companion reference, loaded on demand. Where `SKILL.md` gives the questions to put to a guideline, the phrasebook catalogues what the answers look like on the page — the recurring clause types, the wordings each one takes, and what each variant actually obligates.

It exists because most of the work of reading a funding guideline is pattern-matching against a genre you have seen before. Knowing that "incorporated under" and "registered under" are different tests, that an expenditure bar and a concurrent-submission bar are different bars, or that a benefit criterion, a geographic work requirement, an asset lock-in and a public-benefit test are four separate obligations, is the difference between a clean application and one that fails on something nobody scored.

Eighteen sections: the shared criterion vocabulary, scoring instruments and hurdle clauses, eligibility, benefit-to-the-jurisdiction, matching and in-kind, IP, deliverables language, double-funding, duration and disallowables, related parties and procurement, declarations, audit, format and language, process and finality, lay-accessibility requirements, what published oversight reviews find, how to read the absences, and currency.

Same discipline as the skill: no scheme names, no bodies, no jurisdiction, no dates, no live figures. Quoted phrasings are anonymised examples of *forms of words*, with jurisdiction-specific nouns replaced by bracketed generics. Where something is inferred rather than published — most of what can be said about writing for lay reviewers — it carries an explicit status note. Nothing in it should ever be quoted into an application; the current guideline is the only authority.

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

Claude picks it up automatically from the `description` field. You can also invoke it directly with `/public-funding-applications`. Either clone brings `references/` with it, which is what the skill reads for the phrasebook.

In the Claude apps, upload the repo as a zip rather than `SKILL.md` alone, so `references/` comes too. `SKILL.md` on its own still works — it is self-contained — but the phrasebook pointers will go nowhere.

## Scope

The skill will not inflate technical complexity to deter scrutiny, and will not let the plain layer claim more than the specification supports. Both are in there as craft guidance rather than as rules imposed on it: manufactured density doesn't produce deference, it produces a low "insufficiently justified" score or a referral to an external expert, and a gap between the layers surfaces during the presentation, the panel-comment round, or the audit — whichever comes first.

## Contributing

The parts most likely to need work from real use are the intermediary section, which is written from how these bodies are structurally accountable rather than from experience of dealing with them, and the compliance interrogation, which will grow as new disclosure regimes appear. Issues and PRs welcome.

## License

MIT — see [LICENSE](LICENSE).
