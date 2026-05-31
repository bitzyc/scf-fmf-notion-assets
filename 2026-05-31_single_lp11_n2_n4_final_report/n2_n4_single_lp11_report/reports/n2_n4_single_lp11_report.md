# N=2 and N=4 Single-LP11 Final Report

This report summarizes the current best real mode-basis replay evidence for the N=2 and N=4 single canonical LP11 two-lobe target search. It is not a full-count conclusion; N=6/8/10 are not included here.

Field panels are retained-basis reconstructions from saved real SMF FDE modes, EME SCF/FMF port bases, and solved EME S-matrix sidecars. They are not new Lumerical monitor exports.

## Selected Results

| N | eta_single_LP11 | eta_LP11_group | single/group | target | SCF side (um) | FMF R (um) | SMF R (um) | L (mm) | layout | positions (um) |
|---:|---:|---:|---:|---|---:|---:|---:|---:|---|---|
| 2 | 0.775000 | 0.775000 | 1.000000 | LP11y-polY | 55 | 15 | 4.5 | 3.425 | best_local_axis_pair | `-21,0;21,0` |
| 4 | 0.742182 | 0.742182 | 1.000000 | LP11x-polY | 82 | 18 | 4.5 | 7.400 | line_four | `-34,0;-16,0;16,0;34,0` |

## Key Figures

![Final structures](../figures/optimized_structures_n2_n4.png)

![Eta comparison](../figures/eta_single_lp11_n2_vs_n4.png)

![Energy accounting](../figures/energy_accounting_n2_vs_n4.png)

![Geometry comparison](../figures/geometry_parameters_n2_vs_n4.png)

## Key-Position Mode/Field Panels

Each row shows `SMF input | SCF z=0 | SCF z=L | FMF output` for the selected single-LP11 optimum.

![N2 N4 field contact sheet](../figures/field_panels_N2_N4_contact_sheet.png)

![N=2 field panels](../figures/field_panels_N2.png)

![N=4 field panels](../figures/field_panels_N4.png)

## Field Reconstruction Diagnostics

| N | source eta | reconstructed eta | abs error | target | two-lobe gate | convention |
|---:|---:|---:|---:|---|---|---|
| 2 | 0.775000 | 0.775000 | 0.000e+00 | LP11y-polY | True | retained-basis reconstruction; SCF z=L is phase propagation for visualization; eta uses S21 @ normalized SCF z=0 coefficients |
| 4 | 0.742182 | 0.742182 | 0.000e+00 | LP11x-polY | True | retained-basis reconstruction; SCF z=L is phase propagation for visualization; eta uses S21 @ normalized SCF z=0 coefficients |

## Interpretation Boundary

- The N=2 best checked row is slightly higher than the current N=4 best checked row.
- This does not prove that fewer cores are universally better; it only summarizes the currently completed N=2/N=4 real replay branches.
- The field panels are explanatory. The quantitative evidence remains the eta, target dominance, and energy ledger tables.

## Machine-Readable Summary

```json
{
  "ok": true,
  "status": "n2_n4_single_lp11_report_generated",
  "smf_counts": [
    2,
    4
  ],
  "best_eta_by_count": {
    "2": 0.7750002096014241,
    "4": 0.7421820139163451
  },
  "field_reconstruction_status": "retained_basis_reconstruction_completed",
  "claim_boundary": "Current N=2/N=4 single-LP11 real mode-basis replay summary only; not a full N-trend or fabricated-device conclusion.",
  "files": {
    "selected_rows": "Demo for user/2026-05-31_single_lp11_n2_n4_final_report/results/n2_n4_single_lp11_report/sweeps/n2_n4_selected_rows.csv",
    "energy": "Demo for user/2026-05-31_single_lp11_n2_n4_final_report/results/n2_n4_single_lp11_report/sweeps/n2_n4_energy.csv",
    "field_diagnostics": "Demo for user/2026-05-31_single_lp11_n2_n4_final_report/results/n2_n4_single_lp11_report/sweeps/n2_n4_field_reconstruction_diagnostics.csv",
    "controls": "Demo for user/2026-05-31_single_lp11_n2_n4_final_report/results/n2_n4_single_lp11_report/sweeps/n2_n4_controls_reconstructed.csv",
    "report": "Demo for user/2026-05-31_single_lp11_n2_n4_final_report/results/n2_n4_single_lp11_report/reports/n2_n4_single_lp11_report.md",
    "figures": {
      "structures": "Demo for user/2026-05-31_single_lp11_n2_n4_final_report/results/n2_n4_single_lp11_report/figures/optimized_structures_n2_n4.png",
      "eta": "Demo for user/2026-05-31_single_lp11_n2_n4_final_report/results/n2_n4_single_lp11_report/figures/eta_single_lp11_n2_vs_n4.png",
      "energy": "Demo for user/2026-05-31_single_lp11_n2_n4_final_report/results/n2_n4_single_lp11_report/figures/energy_accounting_n2_vs_n4.png",
      "geometry": "Demo for user/2026-05-31_single_lp11_n2_n4_final_report/results/n2_n4_single_lp11_report/figures/geometry_parameters_n2_vs_n4.png",
      "field_N2": "Demo for user/2026-05-31_single_lp11_n2_n4_final_report/results/n2_n4_single_lp11_report/figures/field_panels_N2.png",
      "field_N4": "Demo for user/2026-05-31_single_lp11_n2_n4_final_report/results/n2_n4_single_lp11_report/figures/field_panels_N4.png",
      "field_contact": "Demo for user/2026-05-31_single_lp11_n2_n4_final_report/results/n2_n4_single_lp11_report/figures/field_panels_N2_N4_contact_sheet.png"
    },
    "summary_json": "Demo for user/2026-05-31_single_lp11_n2_n4_final_report/results/n2_n4_single_lp11_report/data/n2_n4_single_lp11_report_summary.json"
  }
}
```
