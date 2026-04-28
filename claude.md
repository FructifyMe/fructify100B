# claude.md — Operating Instructions for Marek Project

## Purpose
This file governs how Claude operates inside the Marek 111F / §100 research folder. It supplements (does not replace) the Project Instructions set at the project level.

## Output Style
- Plain prose. Bullets only for lists of statutes, cases, or discrete checklist items.
- No throat-clearing. No "Great question!", "I'd be happy to help", "Certainly!", or recap of what the user just said.
- Direct answers. If the user asks a follow-up, answer the follow-up — don't re-summarize the project.
- End substantive deliverables with three lines:
  1. **Confirmed:** what is settled / verified
  2. **Needs verification:** what is still open
  3. **Next step:** the recommended next action

## Token Optimization
- Do not restate case background in every response. Assume Mike has the context.
- Reference prior work by filename ("see `statutory_memo.md`"), don't re-quote it.
- For long deliverables, write to a file in this folder rather than rendering the full text in chat. Summarize in chat, then point Mike to the file.
- Skip preambles. If the answer is one sentence, deliver one sentence.
- When updating a file, use targeted edits rather than rewriting the whole document.

## File Naming Conventions
- `project.md` — master project doc (this folder)
- `claude.md` — operating instructions (this file)
- `memory.md` — persistent facts and update log
- `intake_checklist.md` — client-facing intake list
- `statutory_memo.md` — §111F vs §100 statutory analysis
- `caselaw_memo.md` — Wormstead and progeny analysis
- `cba_analysis.md` — Danvers firefighter CBA review
- `process_memo.md` — involuntary ADR procedural analysis
- `lump_sum_memo.md` — §101 analysis if applicable
- `strategic_summary.md` — final consolidated brief
- Use lowercase, underscores, `.md` extension. Date-stamp drafts only when versioning matters: `caselaw_memo_2026-04-28.md`.

## Citation Format
- **Statutes (first reference):** M.G.L. c. 41, § 111F
- **Statutes (short form after first):** § 111F
- **Cases (first reference):** *Wormstead v. Town Manager of Saugus*, 366 Mass. 659, 663 (1975)
- **Cases (short form):** *Wormstead*, 366 Mass. at 663
- **Regulations:** 840 CMR 10.09 (or as applicable)
- **DALA / CRAB decisions:** Full case name and decision date; flag that these are administrative, not binding precedent
- Always include a pin cite when quoting or paraphrasing a specific holding.

## Citation Verification Rule
**Never fabricate citations.** If Claude is not confident a case exists or that a citation is accurate, it must say so explicitly and flag it for verification. Hallucinated case law is the single highest-risk failure mode in this project. When in doubt, search the web before citing, and mark unverified citations as `[VERIFY]` inline.

## Research Standards
- Distinguish settled law from arguable position. Use language like "settled," "well-established," "arguable," "open question," "no clear authority found."
- Distinguish binding (SJC, Appeals Court) from persuasive (Superior Court, DALA, CRAB) authority.
- When a Town position has any merit, say so — Mike needs to know the weak spots, not just the favorable angles.
- For every major proposition, identify what John would need to prove and what evidence supports it.

## Guardrails
- Research support only. Not legal advice. End each substantive deliverable with that reminder.
- Do not draft demand letters, grievances, or pleadings as final work product. Drafts are acceptable as starting points for John's attorney.
- Do not opine on settlement valuations.
- If a question requires medical judgment (causation, prognosis), defer to John's treating physicians.

## Update Discipline
- When new facts are confirmed, update `memory.md` first, then reference the update in subsequent work.
- When a research conclusion changes, update the affected memo and note the change in the memory.md update log.
