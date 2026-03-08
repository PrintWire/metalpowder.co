---
title: "DMLS Powder Recycling: How Many Cycles Before You're Changing Properties?"
date: 2026-03-08
summary: "Recycled DMLS powder changes with every cycle — oxygen content increases, particle size distribution shifts, and flowability degrades. This guide quantifies the limits."
tags: ["powder recycling", "Ti6Al4V", "316L", "DMLS", "feedstock qualification"]
---

Every unsintered powder in a DMLS build job is potential feedstock for the next run.
But it has been exposed to heat, laser radiation, and oxidation during the build.
Recycling indefinitely degrades the powder incrementally until properties fall out of spec.

## What Changes in Recycled Powder

**Oxygen content (titanium):** The most critical parameter. Ti6Al4V picks up oxygen from
ambient atmosphere during the build — even in inert-gas-purged chambers with < 100 ppm O₂.
Each cycle typically adds 200–500 ppm O. ASTM F3001 (DMLS Ti6Al4V) allows maximum 0.20%
oxygen. Starting powder at 0.10% gives headroom for approximately 5–10 recycles before
mandatory blending with virgin powder or rejection.

**Particle size distribution:** Partially melted "satellite" particles attach to unsintered
powder and shift D90 upward. After 10–15 cycles, sieve analysis (ASTM B214) reveals 5–15%
increase in particles > 63 µm, which increases layer roughness.

**Flowability:** Satellite accumulation and electrostatic charge buildup both reduce Hall
flow rate. A decrease > 20% from virgin spec triggers mandatory sieving.

## Recommended Recycling Protocols by Alloy

| Alloy | Max Recycles Before Blending | Key Indicator |
|-------|------------------------------|---------------|
| Ti6Al4V ELI | 5–8 | Oxygen content |
| 316L stainless | 15–20 | Particle size D90 |
| AlSi10Mg | 10–15 | Flowability |
| Inconel 718 | 20–30 | Chemistry |
| 17-4 PH | 10–15 | Carbon content |

## Best Practice: Blend Ratio Protocol

Rather than running to failure and scrapping a full lot, implement a blend ratio protocol:
mix recycled powder with 20–40% virgin powder after every 5 cycles. This maintains
chemistry within specification while maximizing powder utilization. Document blend
ratios in lot traceability records for AS9100D compliance.
