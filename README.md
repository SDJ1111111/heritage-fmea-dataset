# Dataset: Expert Assessment Data for Risk Prioritisation of Heritage Timber Components

This repository contains the English-language research data accompanying the manuscript
*Ontology-enabled risk prioritisation in heritage building information modelling using
stability-corrected FMEA*. The data support a cloud-model-based FMEA assessment of
damage in historic timber components.

All Chinese-language labels in the original worksheets have been translated into
academic English using the terminology defined in the manuscript (Table 1 for HBIM
component codes, Table 4 for damage-node codes, and the ontology section for the
eight parent damage classes). All numerical values, formulas and worksheet structures
are identical to the original data collection forms.

## Files

| File | Description |
|---|---|
| `data/Data Collection Information Form1_English.xlsx` – `Form6_English.xlsx` | Six raw expert assessment forms. Each workbook contains 88 data rows evaluating the 29 damage nodes (U11–U81) against seven component types (H11–H74), rated by three experts on occurrence (O), severity (S) and detectability (D) on a 1–7 scale. |
| `data/Book1_English.xlsx` | Consolidated analysis workbook (31 worksheets). Contains the aggregated cloud parameters (Ex, En, He), the stability-corrected entropy and hyper-entropy, grey relational coefficients, and the final risk-priority ranking (worksheets `gj` and `Newgj`). |

## Terminology

### HBIM component codes (manuscript Table 1)

| Code | Component | Code | Component |
|---|---|---|---|
| H11 | Painted finish | H71 | Beam |
| H12 | Paint layer | H72 | Bracket |
| H13 | Sculpture | H73 | Column |
| H74 | Tie beam | | |

### Damage classes and nodes

| Parent class | Child nodes |
|---|---|
| U1 Decay | U11 Surface decay; U12 Internal decay; U13 Surface and internal decay; U14 Ageing |
| U2 Deformation | U21 Erosion/denudation; U22 Movement; U23 Dislocation; U24 Concavity; U25 Subsidence; U26 Material loss; U27 Falling off; U28 Rolling; U29 Droop; U210 Warping |
| U3 Insect damage | U31 Surface insect damage; U32 Internal insect damage; U33 Surface and internal insect damage |
| U4 Material defect | U41 Air shrinkage; U42 Knot; U43 Leaking joint; U44 Oblique shrinkage |
| U5 Cracking | U51 Splitting; U52 Rupture; U53 Dry shrinkage and cracking; U54 Fracture; U55 Embrittlement and carbonisation |
| U6 Fire hazard | U61 Fire hazard |
| U7 Water seepage | U71 Water seepage |
| U8 Weed growth | U81 Weed growth |

### Column codes

- **O** = Occurrence, **S** = Severity, **D** = Detectability (FMEA risk factors).
- **Ex** = Expectation, **En** = Entropy, **He** = Hyper-entropy of the normal cloud model.
- **NewEn / NewHe** = stability-corrected entropy and hyper-entropy.
- **gj** = grey relational grade; **Newgj** = improved grey relational grade used for final ranking.

## Notes

- Source worksheet A53 in the original data reads `4材料缺陷` (a missing "U" prefix); it is
  rendered as `U4 Material defect` here, consistent with the manuscript terminology.
- All formulas and cached values in `Book1_English.xlsx` are preserved byte-for-byte;
  the workbook can be recalculated directly in Excel or WPS.

## Suggested citation

Please cite the accompanying manuscript and this dataset repository (insert DOI once
the repository is archived, e.g. via Zenodo).
