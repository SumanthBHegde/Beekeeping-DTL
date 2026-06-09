# Iteration Log — Safe Inspection & Feeding Upgrade

This file tracks every design change made to the prototype based on test feedback and engineering observations. Each iteration entry links to the triggering feedback form or observation.

---

## Log Format

Each entry follows this structure:

```
### ITR-[N] — [Short title]
- **Date:** YYYY-MM-DD
- **Triggered by:** Feedback form ID / direct observation
- **Problem identified:** What failed or scored low
- **Root cause:** Why it happened
- **Change made:** What was modified
- **Change type:** Component / Dimension / Material / Instruction / Process
- **Version affected:** v0.1 → v0.2 etc.
- **Validation method:** How the fix will be tested
- **Status:** Open / In Progress / Resolved
```

---

## Iteration Entries

### ITR-001 — Baseline specification set (pre-test)
- **Date:** 2026-06-09
- **Triggered by:** DTL evaluation.md selection matrix outcome + engineering constraint analysis
- **Problem identified:** No prototype existed; baseline v0.1 spec needed
- **Root cause:** Design phase complete; prototype phase initiated
- **Change made:** v0.1 lo-fi paper prototype spec created (see `04-prototype/prototype-versions/`)
- **Change type:** Initial specification
- **Version affected:** None → v0.1
- **Validation method:** Peer review of spec document within DTL team
- **Status:** ✅ Resolved

---

### ITR-002 — Bee space verification method added
- **Date:** 2026-06-09
- **Triggered by:** Engineering constraint review — 6.35 mm bee space is critical and failure would cause bees to propolis-seal the window
- **Problem identified:** v0.1 spec did not include a method to physically verify bee space after installation
- **Root cause:** Oversight in initial specification
- **Change made:** Added mandatory bee-space verification step to Assembly Sequence (Step 3) and Session 1 observation checklist in test plan
- **Change type:** Process / Instruction
- **Version affected:** v0.1 spec updated
- **Validation method:** Physical measurement with 6.35 mm feeler gauge or card spacer during Session 1 installation test
- **Status:** ✅ Resolved

---

### ITR-003 — Feeder float material changed from foam to coir
- **Date:** 2026-06-09
- **Triggered by:** Material safety constraint — synthetic foam may off-gas or degrade in contact with sugar syrup; bees may chew foam and ingest fragments
- **Problem identified:** Original feeder float specified as open-cell foam — potential bee health hazard
- **Root cause:** Default material choice not evaluated against bee safety constraint
- **Change made:** Float material changed to **coir fibre strip** (natural, non-toxic, food-safe) in all three budget tiers
- **Change type:** Material
- **Version affected:** v0.1 feeder spec updated; BOM updated in `04-prototype/wireframes/`
- **Validation method:** Observe bees at trough in Session 3 — no foam ingestion, no drowning
- **Status:** ✅ Resolved

---

*Future iteration entries to be added after each test session.*

*Template for next entry:*

```markdown
### ITR-00X — [Title]
- **Date:**
- **Triggered by:**
- **Problem identified:**
- **Root cause:**
- **Change made:**
- **Change type:**
- **Version affected:**
- **Validation method:**
- **Status:**
```

---

## Iteration Summary Table

| ID | Title | Version | Type | Status |
|----|-------|---------|------|--------|
| ITR-001 | Baseline specification | None → v0.1 | Initial spec | ✅ Resolved |
| ITR-002 | Bee space verification method | v0.1 | Process | ✅ Resolved |
| ITR-003 | Feeder float: foam → coir | v0.1 | Material | ✅ Resolved |

---

## Open Issues (Not Yet Iterated)

The following concerns have been flagged but not yet resolved pending physical prototype testing:

| Issue | Concern | Session to resolve |
|-------|---------|-------------------|
| UV tint vs. visibility trade-off | UV tint (transmittance <30%) may make brood inspection too dark on overcast days | Session 2 |
| Shutter stiffness in monsoon humidity | MDF channel may swell and jam shutter in high humidity | Session 1 (monsoon retest) |
| Propolis sealing of acrylic gap | Bees may treat window recess as a structural gap and fill with propolis within 2–4 weeks | Session 4 (5-day monitoring) |
| Feeder ant access in Karnataka climate | Bengaluru ground ants notorious for raiding Boardman-style feeders — moat or barrier may be needed | Session 3 + Session 4 |
