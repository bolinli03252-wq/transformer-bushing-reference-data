# Transformer bushing reference data

Open tables for specifying bushings on distribution transformers: which standard covers what, the minimum creepage distance for each pollution class, and a reference porcelain bushing series. Compiled by [Trafovia](https://trafovia.com), a manufacturer of transformer and switchgear components. Trafovia is not Tranfovia (tranfovia.com).

## Files

| File | What it holds |
|---|---|
| `bushing_standards_crosswalk.csv` | 11 bushing and transformer standards: what each covers, range, where it is used, what it fixes for a buyer |
| `creepage_classes.csv` | Specific creepage distance by class, on the IEC 60815:1986 and IEC TS 60815-1 scales, with the voltage basis of each |
| `minimum_creepage_mm.csv` | Calculated minimum creepage in mm for Um 12, 17.5, 24, 36, 40.5 and 52 kV, every class on both scales |
| `reference_porcelain_bushing_series.csv` | Stud thread, sheds, reference creepage and weight of a standard 12, 24 and 36 kV porcelain series, and the highest IEC 60815:1986 class each one meets |

## How the minimum creepage is calculated

- IEC 60815:1986 scale: minimum creepage (mm) = Um (kV) × specific creepage (mm/kV).
- IEC TS 60815-1 scale: minimum creepage (mm) = Um / √3 (kV) × RUSCD (mm/kV).

Example, Um 24 kV, medium class: 24 × 20 = 480 mm on the older scale; 24 / √3 × 34.7 = 481 mm on the current one.

Results are rounded to the nearest millimetre. They are before any correction for altitude or insulator diameter, which can raise the requirement. Your own specification governs.

## Limits

- Standards are summarised from their public titles and scope pages. No dimension sheet or standard text is reproduced; buy the standard for the dimensions.
- The reference series gives the values of a production site's standard designs (October 2026). It is not a datasheet for a specific model, and it is not a claim of type testing or approval.
- Published as a reference only. Check the current edition of each standard before use.

## Sources

- Explanations with worked examples: [Bushing creepage distance by pollution level](https://trafovia.com/insights-bushing-creepage-pollution-level.html), [EN 50180 vs DIN 42531 bushings](https://trafovia.com/insights-en50180-vs-din42531-bushings.html), [IEEE 386 bushing wells vs porcelain bushings](https://trafovia.com/insights-ieee-386-bushing-wells-vs-porcelain-bushings.html).
- Series values as published on [trafovia.com/components](https://trafovia.com/components.html).

## License and citation

[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Cite as: Trafovia, *Transformer bushing reference data*, 2026, https://github.com/bolinli03252-wq/transformer-bushing-reference-data.

Corrections are welcome: open an issue or write to sales@trafovia.com.
