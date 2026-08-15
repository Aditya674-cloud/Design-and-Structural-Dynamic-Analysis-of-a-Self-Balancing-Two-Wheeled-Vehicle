| Load Case | Description | Type | Magnitude |
|---|---|---|---|
| LC1 | Static standing — rider stationary | Static | 981 N (100kg × 9.81 m/s²) |
| LC2 | Forward acceleration — dynamic CG shift | Dynamic | F = 322.6 N, a = 1.96 m/s² |
| LC3 | Braking — deceleration, reverse tilt | Dynamic | Equal magnitude to LC2, opposite direction |
| LC4 | Cornering — lateral load at critical speed | Dynamic | Based on v_critical ≈ 9.17 km/h |
| LC5 | Road/vibration input — surface roughness | Cyclic | Basis for Sections 11–13 |
| LC6 | Combined worst-case — acceleration + road input | Cyclic/Combined | Superposition of LC2 + LC5 |

 ## Load Case Descriptions

LC1 — Static Standing: Baseline case, rider standing still, vehicle stationary or moving at constant velocity. Establishes the reference static stress state.

LC2 — Forward Acceleration: Rider mass generates an inertial force during acceleration, shifting effective load distribution toward the rear of the platform and increasing dynamic tilt demand (linked to Section 04's dynamic CG shift calculation).

LC3 — Braking: Mirror case of LC2, inertial force acts forward, frame must handle reversed loading direction — relevant since real frames aren't always symmetric in stiffness front-to-back.

LC4 — Cornering: Lateral force from centripetal acceleration during turns; becomes significant above the critical cornering speed identified in Section 04.

LC5 — Road/Vibration Input: Represents cyclic loading transmitted through the wheels from surface irregularities — the primary driver for modal (Section 11), harmonic (Section 12), and fatigue (Section 13) analysis.

LC6 — Combined Worst-Case: Conservative design case superimposing acceleration loading with road vibration input — used for final static FEA (Section 08) to ensure the design has margin under simultaneous real-world loading.
