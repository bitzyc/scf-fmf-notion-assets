# Single-LP11 Near-Full-Parameter Optimized Co-Design

This report adds a fourth single-LP11 two-lobe experiment mode. Each `N` is independently optimized over SCF side, FMF radius, SMF core radius, SCF length, relaxed pitch, free ring rotation, target direction, and complex controls.

These rows are deterministic proxy evidence plus Lumerical handoff. They are not a pure N-only causal experiment and are not real Lumerical validation unless the handoff cases are solved and replayed.

## Best Rows

| N | eta single | eta group | SCF side um | FMF radius um | SMF radius um | L mm | pitch um | rotation deg | target | gate |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 2 | 0.847000 | 0.904915 | 90 | 16 | 4.5 | 3.675 | 91 | 135.000 | LP11y-polX | True |
| 4 | 0.881759 | 0.907159 | 100 | 16 | 4.5 | 5.775 | 67 | 45.000 | LP11x-polY | True |
| 6 | 0.882718 | 0.882719 | 130 | 16 | 4.5 | 3.550 | 48 | 45.000 | LP11x-polY | True |
| 8 | 0.904225 | 0.904226 | 110 | 14 | 4.5 | 3.575 | 34 | 28.125 | LP11x-polY | True |
| 10 | 0.902515 | 0.902516 | 130 | 16 | 4.5 | 5.825 | 31 | 34.875 | LP11x-polY | True |

## Variable Definition

- Fixed: wavelength, single-LP11 two-lobe objective family, two Jones-like channels per SMF, uniform-ring layout family, edge margin, length gate, normalization, eta/energy definitions, and no robustness.
- Independent variable: `SMF count N`.
- Optimized per `N`: SCF side, FMF radius, SMF core radius, length, relaxed pitch, free rotation, canonical target direction, and complex controls.

## Solver Status

- Solver status: `proxy_plus_handoff_pending_real_solver`.
- Lumerical handoff scripts are generated for the top three candidates per count.
- No new real sidecar is claimed by this runner.
