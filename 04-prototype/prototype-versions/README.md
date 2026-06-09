# Prototype Versions — Safe Inspection & Feeding Upgrade

This directory contains versioned iterations of the beehive prototype and related notes. This includes both physical prototype tracking and the digital interactive visualiser.

## Digital Prototype
* **v1.0 (Interactive Visualiser)**
  * The active version is located in the parent directory: `../beehive-prototype.html`.
  * Fully procedural 3D model using Three.js (r165).
  * Features implemented: ISI Standard dimensions, internal thin XPS insulation, dual inspection windows (left & back), external top feeder system, flow hive modifications, and interactive UI controls.
* Any major revisions, experimental branches, or snapshots of the digital prototype should be saved here (e.g., `beehive-prototype-v2.html`) to maintain a clean history.

## Physical Prototypes Overview

This folder tracks every iteration of the **Safe Inspection & Feeding Upgrade** — a retrofit module that combines a UV-tinted acrylic inspection window (C1) with an external top-feeder (C2) onto any standard Indian wooden bee box, without structural modification.

The prototype is developed across three fidelity levels:

| Version | Fidelity | Status | Goal |
|---------|----------|--------|------|
| v0.1 | Paper / cardboard mock-up | ✅ Complete (Lo-Fi) | Validate spatial layout and dimensions |
| v0.2 | Foam-board + acrylic sample | 🔄 In Progress (Mid-Fi) | Check bee space, light leak, thermal behaviour |
| v0.3 | Full working unit — Budget tier | ⏳ Planned | End-to-end usability test with beekeeper |
| v1.0 | Standard tier (₹4,000) | ⏳ Planned | Final field validation |

---

## v0.1 — Low-Fidelity Paper Prototype Specification

### Concept
A cardboard scale model (1:1) of the hive's front face, with a cut-out window covered by a flap shutter and a small tray representing the feeder trough, used to test ergonomics and spatial decisions without any cost.

### Target Standard Box Dimensions
Indian standard wooden bee box (Langstroth-style 10-frame brood body):
- External width: **505 mm**
- External depth: **415 mm**
- External height (brood body): **240 mm**

### Window Module Specification (v0.1)

| Parameter | Value | Rationale |
|-----------|-------|----------|
| Window cutout size | 180 mm × 100 mm | Enough to see brood frames without weakening hive wall |
| Position | Front face, centred horizontally, 80 mm from bottom | Below top bars, avoids hive entrance below |
| Acrylic proxy material | Transparent OHP sheet (80 micron) | Simulates transparency; zero cost |
| Shutter proxy | Cardboard flap with tape hinge | Simulates sliding opaque cover |
| Bee space maintained | ≥ 6.35 mm clearance from inner surface to nearest comb | Non-negotiable; marked on mock-up with spacer strip |

### Feeder Module Specification (v0.1)

| Parameter | Value | Rationale |
|-----------|-------|----------|
| Feeder type | Boardman entrance-style trough | No hive opening required; bees access from entrance |
| Reservoir proxy | 500 mL plastic bottle inverted over cardboard tray | Simulates sugar syrup reservoir |
| Trough width | 30 mm | Fits standard hive entrance slot |
| Trough depth | 20 mm | Prevents bee drowning risk |
| Float / landing strip | Cardboard strip inside trough | Prevents bees from submerging |

### Critical Constraints Checklist (v0.1)

- [ ] Bee space (6.35 mm) verified with ruler on all internal surfaces
- [ ] Window cutout does not penetrate inner hive wall beyond 12 mm depth
- [ ] Shutter fully covers window — zero light leak when closed
- [ ] No sharp card edges facing the hive interior
- [ ] Feeder tray positioned below hive entrance — no hive opening required
- [ ] Feeder removable without disturbing bees

---

## v0.2 — Mid-Fidelity Foam-Board Prototype (Planned)

### Changes from v0.1
- Replace OHP sheet with a real **5 mm UV-tinted cast acrylic** sample (200 mm × 120 mm)
- Replace cardboard shutter with a **3 mm PVC slider** running in 4 mm MDF grooves
- Replace cardboard walls with **10 mm XPS foam-board** to test thermal performance
- Replace tray with a **1-litre PET bottle + inverted feeder lid** assembly

### Thermal Validation Target
- Ambient temperature during test: 28–35°C (Bengaluru outdoor, daytime)
- Brood-side acrylic surface must not exceed **36°C** when in direct sunlight
- UV tint (transmittance < 30% for UV-A 315–400 nm) must be confirmed with UV torch test

---

## v0.3 & v1.0 — Full Working Prototype (Planned)

See `sketches/` and `wireframes/` folders for dimensional drawings and exploded BOM.
Field testing protocols are in `05-test/test-plan/`.

---

## Change Log

| Date | Version | Change | Author |
|------|---------|--------|---------|
| 2026-06-09 | v0.1 | Initial lo-fi specification drafted | pavannaik2004 |
