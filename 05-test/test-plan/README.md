# Usability Test Plan — Safe Inspection & Feeding Upgrade

## Test Objective

Validate that the integrated prototype achieves its three core outcomes without violating any engineering constraints:
1. Beekeeper can visually inspect colony status **without opening the hive**
2. Beekeeper can feed the colony **without opening the hive**
3. Brood nest temperature remains within **33–36°C** throughout
4. Bee stress behaviour does not increase after installation

---

## Participants

| Role | Profile | Recruitment |
|------|---------|-------------|
| Primary tester | Small-scale beekeeper, 40–80 hives, 3+ years experience | Karnataka Beekeepers' Co-operative, Bengaluru |
| Secondary tester | Novice beekeeper, < 1 year, 1–5 hives | DTL network / local apiculture NGO |
| Observer | DTL team member (non-participant) | Project team |

**Minimum sample:** 3 beekeepers across 2 test sites (minimum 2 active hives per site).

---

## Test Conditions

| Condition | Detail |
|-----------|--------|
| Location | Outdoor apiary, Bengaluru region (or peri-urban farm) |
| Season | Post-monsoon flow period (October–November) or pre-monsoon build-up (Feb–March) |
| Time of day | 07:00–09:00 (cool, low bee flight) for installation; 10:00–12:00 for live observation test |
| Ambient temperature | 24–34°C (record at each observation) |
| Hive type | Standard Indian wooden Langstroth-style 10-frame box |
| Prototype version | v0.2 minimum (foam-board + real acrylic); v0.3 preferred |

---

## Test Sessions

### Session 1 — Installation Usability
**Duration:** 60 minutes  
**Task:** Beekeeper installs the prototype module (window + shutter + feeder) onto their own hive, following a 1-page visual instruction sheet.

**Metrics:**
- Time to complete installation (target: < 45 min with hand tools only)
- Number of times hive body opened during installation (target: **zero**)
- Number of errors / deviations from instruction sheet
- Beekeeper confidence rating (1–5 Likert scale post-task)

**Observation checklist:**
- [ ] Bee space ≥ 6.35 mm confirmed after installation
- [ ] Shutter fully seals window (light leak test: torch behind shutter)
- [ ] Feeder trough level, no spillage
- [ ] No sharp edges / exposed metal on hive exterior
- [ ] XPS wrap does not cover ventilation strip

---

### Session 2 — Inspection Window Test
**Duration:** 30 minutes (at peak forager return, ~16:00–17:00)  
**Task:** Beekeeper uses the inspection window to answer 5 standardised colony-status questions (see below) without opening the hive.

**5 Colony-Status Questions:**
1. Is the queen present? (look for brood pattern)
2. Is the colony queenright? (capped brood visible?)
3. Is there visible honey/nectar storage in visible frames?
4. Are there signs of pest/disease (unusual cell appearance, debris)?
5. Is the colony population adequate? (frame coverage visible)

**Metrics:**
- Answer accuracy vs. subsequent full hive inspection (ground truth)
- Time to answer all 5 questions through window
- Shutter operation ease rating (1–5)
- Window clarity rating (1–5) — UV tint vs. visibility trade-off

---

### Session 3 — Feeder Usability Test
**Duration:** 20 minutes  
**Task:** Beekeeper refills feeder reservoir (1L bottle) and verifies bees are actively feeding — without opening hive.

**Metrics:**
- Time to refill reservoir
- Spillage incidents (target: zero)
- Beekeeper-rated ease of refill (1–5)
- Bee access confirmation: bees observed at trough within 15 minutes
- Drowning incidents observed at trough (target: zero)

---

### Session 4 — Thermal & Structural Monitoring
**Duration:** 5 days continuous (passive monitoring)  
**Tool:** Cheap digital thermometer (DHT22 sensor or equivalent) placed on inner wall near brood area, data logged manually twice daily (08:00 and 14:00).

**Metrics:**
- Brood-area temperature range over 5 days (target: 33–36°C)
- Acrylic inner-surface temperature at solar noon (target: < 36°C)
- Any visible condensation on acrylic inner face (target: none)
- Colony population change (frame count before vs. after 5 days)

---

### Session 5 — Bee Behaviour Observation
**Duration:** 3 × 30-minute observation windows over 5 days  
**Method:** Standardised observation: count guard bee activity at entrance, fanning behaviour, and propolis-sealing of window recess.

**Behavioural indicators (stress signs to watch for):**
- Excessive propolis application on acrylic (> 3 mm bead) — indicates bees treating window as intrusion
- Increased guarding / defensive behaviour at entrance
- Reduced forager return rate
- Abnormal clustering near window (cold stress indicator)

---

## Success Criteria

| Criterion | Threshold | Critical? |
|-----------|-----------|----------|
| Zero hive openings during feeding | 100% sessions | ✅ Critical |
| Zero hive openings during inspection | 100% sessions | ✅ Critical |
| Brood temperature 33–36°C | All 5 monitoring days | ✅ Critical |
| Installation time < 45 min | ≥ 75% of testers | High |
| Window inspection accuracy ≥ 3/5 questions correct | ≥ 75% of testers | High |
| Beekeeper satisfaction ≥ 4/5 (overall) | ≥ 75% of testers | Medium |
| Zero bee drowning incidents in feeder | 100% sessions | ✅ Critical |
| Zero toxic material concerns flagged | All testers | ✅ Critical |

---

## Materials Required

- Prototype v0.2 or v0.3 unit (×3 minimum)
- 1-page visual installation instruction sheet (A4 laminated)
- Feedback form (see `05-test/feedback/`)
- Digital thermometer (DHT22 × 2 per hive)
- Stopwatch
- Observation logbook
- PPE: veiled suit, gloves (for full-inspection ground truth session)
- Camera / phone for photo documentation

---

## Timeline

| Phase | Activity | Week |
|-------|----------|------|
| Prep | Finalise v0.2 prototype | Week 1 |
| Prep | Recruit testers, confirm sites | Week 1–2 |
| Test | Sessions 1–3 (usability) | Week 3 |
| Test | Sessions 4–5 (thermal + behaviour, 5 days) | Week 3–4 |
| Analysis | Collate feedback, score against success criteria | Week 5 |
| Iteration | v0.3 revisions based on findings | Week 5–6 |
