# neat_value Methodology

The `neat_value` score is a composite, position-normalized metric designed to rank and tier fantasy football players across all positions for draft purposes. It is calculated through a multi-step process that integrates projections, value-based metrics, ADP, and career state analysis.

---

## Key Evaluation Questions

- **Expert Evaluation:** How a player is expected to perform, according to expert consensus?
- **Market Awareness:** How is the community at large valuing a player?
- **Historical Expectation:** How do players of this career state perform historically?

### All of this is:
- **League Specific:** All steps adapt to your league’s settings and scoring.
- **Cross Position:** Allows apples-to-apples comparison between all positions.

---

## 1. Fantasy Points Projection
- Each player's up-to-date projected stats are converted into fantasy points using your league’s custom scoring settings.

## 2. VORP Calculation
- **Value Over Replacement Player (VORP)** is computed for each player, representing their value above a replacement-level player at their position.
- Replacement levels are dynamically determined based on your league’s roster and scoring settings, using the prior 4 seasons of historical data.

## 3. VORP Normalization
- VORP values, across all positions, are normalized and scaled to a 1–10 range using polynomial fitting.

## 4. ADP Integration
- Up to date Average Draft Position (ADP) data is imported and scaled to the same 1–10 range, linearly.

## 5. Career State Modifiers
- Using historical data from 2000-2024, age curves, and breakout timelines are developed for the 4 fantasy relevant offensive positions.
- Based on these, as well as other factors, each player is bucketed into a "career state" (e.g., prime, rookie, developing, faded star)
- Each career state/position combination receives a modifier, derived from historical VORP and positional rank analysis.
- These modifiers are then normalized and scaled 1-10.

## 6. Composite neat_value Calculation
- The final `neat_value` is the sum of:
    - **Scaled VORP**
    - **Scaled ADP**
    - **Scaled Career State Modifier**

## 7. Sorting and Output
- The neat_value is then fitted one final time and then rounded to generate the final tiers to be used in the draft sheet.
