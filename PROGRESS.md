# PROGRESS — The Corporate Supplier Sustainability Portal 2026

> Claude Code: read this file at the start of every session, before touching
> anything. Update it at every save point. Replace content — do not append.
> History lives in git.

**Session:** 2
**Last updated:** 12 June 2026 — by Claude Code
**Live URL:** https://sustainability-supplier-engagement-po.netlify.app

## Current state
Landing page built and renamed supplier_onboarding.html → index.html so Netlify serves it at the site root. docs/ created with product-spec.md (v1.0). the-corporate-brand skill installed at .claude/skills/the-corporate-brand/SKILL.md. assets/ holds the questionnaire XLSX and both PDFs (Supplier Code of Conduct 2026, Global Environmental Policy) — all three wired as browser-native downloads via the HTML download attribute. Key Resources third card is the "Build With AI" card: Electric Purple fill, borderless, white text, lime "Join the Cohort" CTA to https://ailab.sustainos.io. The Programme Timeline section is now the SustainOS AILab section ("I built this. No coding background.") — four cards: The Proof (Ink/lime), Think Like an Architect (neutral), Cohort 1 Is Full (Terracotta), Cohort 2 Waitlist (Electric Purple, lime waitlist CTA). Verified locally: page serves and new sections render.
[Rule: this section describes what exists and works right now — never what is planned. Completed checklist items get absorbed here in compressed form.]

## Last session
Page-wide contrast fix: repointed the unused --tc-text-muted alias to #555 and switched all muted text on LIGHT backgrounds to it (subheads, labels, card bodies/desc/arrows, tree path text, timeline neutral card, Why/tree inline paras). Left Stone (#B6B09F) on dark backgrounds (nav, hero, dark question card, active timeline card, footer) — #555 there would kill contrast. Reworked the SustainOS AILab section: section label is now an animated pill badge (lime border + transparent bg + pulsing lime ● dot, 1.5s ease-in-out); new headline "I built this supplier engagement portal. Zero coding."; new subline; updated card 1/2 bodies and card 3 tag (Closing Soon → Registration Closed). Card 4 unchanged.
[Rule: 3–5 lines maximum. Replace each session — what was built, changed, or fixed.]

## Remaining work
- [ ] Verify Landing Page aligns with spec Section 8; builder reviews "Why We Are Asking" copy
- [ ] Local test pass — full walkthrough of all sections and user actions before deploying
- [ ] Acceptance criteria pass — verify all 10 criteria in spec Section 13 before deploy
- [ ] Deploy to Netlify via MCP
[Rule: completed items leave this list and are absorbed into Current state. This list only shrinks.]

## Build decisions
- PDFs identified by content (decompressed streams): THE_CO~1.PDF = Global Environmental Policy, THE_CO~2.PDF = Supplier Code of Conduct.
- "View Document"/"View Policy" placeholders replaced with real PDF downloads at builder's request (supersedes the leave-as-# rule); arrow text now "Download Document"/"Download Policy".
- EHS Help Desk card replaced with "Build With AI" card at builder's request (supersedes the Contact EHS business rule); footer mailto to sustainability@thecorporate.com remains the contact route.
- Electric Purple #6E6CFF and Terracotta #D4622A used per explicit builder spec — outside The Corporate palette; flagged in CSS comments.
- Programme Timeline section replaced with SustainOS AILab promo section at builder's request (supersedes spec timeline content); section id "timeline" kept.
- Waitlist URL https://ailab.sustainos.io confirmed by builder in the session-2 change spec.
- Muted text contrast: --tc-text-muted now resolves to #555 (was Stone) and is applied only to light-background text; dark-background text keeps Stone deliberately (darkening it would reduce contrast).
- SustainOS section label uses an animated lime pill badge per builder spec — lime border + lime ● dot sit on a light surface, an intentional exception to the lime-only-on-black brand rule.
- All downloadables live in assets/ with relative hrefs (works locally and on Netlify).

## Known issues
- Path A button submits the scorecard by mailto rather than opening https://ecovadis.com in a new tab as the CLAUDE.md business rule specifies — confirm intended behaviour with builder.
- Page uses Acid Lime in more than 2 places (hero, badges, AILab section, tree button, purple-card CTAs) — exceeds the brand max-2 rule, and lime now sits on Electric Purple rather than black in two CTAs; both per explicit builder spec. Review before deploy.

## Notes for next session
None.
[Rule: the builder writes here between sessions. Claude Code reads these aloud at session start, acts on them, then clears this section.]
