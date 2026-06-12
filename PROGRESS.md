# PROGRESS — The Corporate Supplier Sustainability Portal 2026

> Claude Code: read this file at the start of every session, before touching
> anything. Update it at every save point. Replace content — do not append.
> History lives in git.

**Session:** 1
**Last updated:** 12 June 2026 — by Claude Code
**Live URL:** none yet [Rule: fill in after the first successful deploy]

## Current state
supplier_onboarding.html built. docs/ created with product-spec.md (v1.0). the-corporate-brand skill installed at .claude/skills/the-corporate-brand/SKILL.md. assets/ holds the questionnaire XLSX and both PDFs (Supplier Code of Conduct 2026, Global Environmental Policy) — all three wired as browser-native downloads via the HTML download attribute. Key Resources third card is now a "Build With AI" card linking to https://ailab.sustainos.io (replaced EHS Help Desk at builder's request). Verified locally: page serves and all three download paths return 200.
[Rule: this section describes what exists and works right now — never what is planned. Completed checklist items get absorbed here in compressed form.]

## Last session
First Session Setup: created docs/ and moved product-spec.md. Renamed the two truncated-name PDFs (THE_CO~1/~2.PDF) to their proper names and moved them plus the questionnaire XLSX into assets/. Wired "Supplier Code of Conduct" and "Global Environmental Policy" cards as PDF downloads. Replaced the EHS Help Desk card with the "Build With AI" card (lime label on Ink chip, links to SustainOS AILab waitlist).
[Rule: 3–5 lines maximum. Replace each session — what was built, changed, or fixed.]

## Remaining work
- [ ] Builder: confirm the waitlist URL — https://ailab.sustainos.io was used (prompt said "ailab.susatinos.io", assumed typo)
- [ ] Verify Landing Page aligns with spec Section 8; builder reviews "Why We Are Asking" copy
- [ ] Local test pass — full walkthrough of all sections and user actions before deploying
- [ ] Acceptance criteria pass — verify all 10 criteria in spec Section 13 before deploy
- [ ] Deploy to Netlify via MCP
[Rule: completed items leave this list and are absorbed into Current state. This list only shrinks.]

## Build decisions
- PDFs identified by content (decompressed streams): THE_CO~1.PDF = Global Environmental Policy, THE_CO~2.PDF = Supplier Code of Conduct.
- "View Document"/"View Policy" placeholders replaced with real PDF downloads at builder's request (supersedes the leave-as-# rule); arrow text now "Download Document"/"Download Policy".
- EHS Help Desk card replaced with "Build With AI" card at builder's request (supersedes the Contact EHS business rule); footer mailto to sustainability@thecorporate.com remains the contact route.
- Lime "Build With AI" label rendered as lime text on an Ink chip to honour the lime-only-on-black brand rule.
- All downloadables live in assets/ with relative hrefs (works locally and on Netlify).

## Known issues
- Path A button submits the scorecard by mailto rather than opening https://ecovadis.com in a new tab as the CLAUDE.md business rule specifies — confirm intended behaviour with builder.
- Page uses Acid Lime in more than 2 places (hero, badges, timeline, tree button) — exceeds the brand max-2 rule; review before deploy.

## Notes for next session
None.
[Rule: the builder writes here between sessions. Claude Code reads these aloud at session start, acts on them, then clears this section.]
