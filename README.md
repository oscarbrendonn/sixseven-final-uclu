# 67 Character — leg & arm variants

Live viewer: https://oscarbrendonn.github.io/sixseven-final-uclu/

Five variants of the same locked 67 character, plus an **all-five side-by-side** view.
**A is the untouched original** — nothing was done to it; it is the reference.
Texture and colour are identical everywhere (4K source, no decimation).
Head, hair, hands and shoes are untouched in every variant.

![measurements](measurements.png)

| variant | height | vs A | arm span | vs A | arm/height |
|---|---|---|---|---|---|
| **A · original (untouched)** | 3.0233 | — | 2.4994 | — | 0.8267 |
| **B · legs +4.2%** | 3.1510 | +4.2% | 2.6585 | +6.4% | 0.8437 |
| **C · legs +6.8%** | 3.2296 | +6.8% | 2.7248 | +9.0% | 0.8437 |
| **D · legs +8.1%** | 3.2689 | +8.1% | 2.7580 | +10.3% | 0.8437 |
| **E · D + wider legs** | 3.2689 | +8.1% | 2.7580 | +10.3% | 0.8437 |

### widths

| variant | chest | hoodie hem | hip | thigh | knee | ankle |
|---|---|---|---|---|---|---|
| **A · original** | 0.589 | 0.545 | 0.560 | 0.308 | 0.282 | 0.283 |
| **B** | 0.623 | 0.619 | 0.656 | 0.344 | 0.291 | 0.274 |
| **C** | 0.634 | 0.620 | 0.687 | 0.340 | 0.288 | 0.275 |
| **D** | 0.614 | 0.599 | 0.645 | 0.304 | 0.278 | 0.267 |
| **E** | 0.614 | 0.603 | 0.657 | **0.314** | **0.286** | **0.273** |

### what was done

| | A | B | C | D | E |
|---|---|---|---|---|---|
| leg stretch (hip→ankle, shoes rigid) | — | ×1.13 | ×1.21 | ×1.25 | ×1.25 |
| arm stretch (shoulder→wrist, hands rigid) | — | +6.4% | +9.0% | +10.3% | +10.3% |
| hoodie hem widened (lattice, by hand) | — | yes | yes | yes | yes |
| oversize cut (lattice, by hand) | — | yes | yes | — | — |
| leg width (lattice, by hand) | — | — | — | — | **yes** |

## Method

- **Leg stretch** — everything above the hip (40% of height) stays fixed; hip→ankle is stretched
  vertically; the shoe moves down rigidly, so its shape is never deformed.
- **Arm stretch** — shoulder stays fixed, arm stretches outward, the hand shifts rigidly (hands never grow).
  B, C, D and E are tuned so **arm/height = 0.8437** — the proportion of the visual reference.
- **Hoodie hem / oversize cut / leg width** — shaped by hand with lattices, then baked.
- Texture stretches vertically where the mesh was stretched, but the garment is flat black,
  so it is invisible.

## Notes on the numbers

- Units are Blender units; every model is at the same scale, so only ratios matter.
- **Shoulder width** and **leg-length percentage** are deliberately omitted: the baggy trouser legs
  merge, so the crotch line cannot be detected automatically and the numbers came out unreliable.
  They are left out rather than guessed.
- **E vs D** — the only difference is trouser leg width, shaped by hand: thigh +3.3%, knee +2.9%, ankle +2.2%.
- Topology is identical across all five: 787,741 verts · 1,445,601 polys.

Files: `original.glb` · `f113.glb` · `f121.glb` · `uzunbacak.glb` · `e_wider.glb` (~4.6 MB each) · `all5.glb` (17 MB, all five in one scene)
