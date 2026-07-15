# 67 Character — leg & arm variants

Live viewer: https://oscarbrendonn.github.io/sixseven-final-uclu/

Four variants of the same locked 67 character, plus an **all-four side-by-side** view.
**A is the untouched original** — nothing was done to it, it is the reference for comparison.
Identical texture and colour everywhere (4K source, no decimation).
Head, hair, hands and shoes are untouched in every variant.

![measurements](measurements.png)

| variant | height | vs A | arm span | vs A | arm/height |
|---|---|---|---|---|---|
| **A · original (untouched)** | 3.0233 | — | 2.4994 | — | 0.8267 |
| **B** | 3.1510 | +4.2% | 2.6585 | +6.4% | 0.8437 |
| **C** | 3.2296 | +6.8% | 2.7248 | +9.0% | 0.8437 |
| **D** | 3.2689 | +8.1% | 2.4994 | 0.0% | 0.7646 |

| what was done | A | B | C | D |
|---|---|---|---|---|
| leg stretch (hip→ankle, shoes rigid) | — | ×1.13 | ×1.21 | ×1.25 |
| arm stretch (shoulder→wrist, hands rigid) | — | +6.4% | +9.0% | — |
| hoodie hem widened (lattice, by hand) | — | yes | yes | yes |
| oversize cut (lattice, by hand) | — | yes | yes | — |
| leg width (lattice, by hand) | — | — | — | yes |

## Method

- **Leg stretch** — everything above the hip (40% of height) stays fixed; hip→ankle is stretched
  vertically; the shoe moves down rigidly, so its shape is never deformed.
- **Arm stretch** — shoulder stays fixed, arm stretches outward, the hand shifts rigidly (hands never grow).
  B and C are tuned so **arm/height = 0.8437** — the proportion of the visual reference.
- **Hoodie hem / oversize cut / leg width** — shaped by hand with lattices, then baked.
- Texture stretches vertically where the mesh was stretched, but the garment is flat black,
  so it is invisible.

Files: `original.glb` · `f113.glb` · `f121.glb` · `uzunbacak.glb` (~4.6 MB each) · `all4.glb` (12.8 MB, all four in one scene)
