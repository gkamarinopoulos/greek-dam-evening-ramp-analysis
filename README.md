# Greek DAM Evening Ramp Analysis (January 2025)

## Research Question

Why are electricity prices often elevated around 20:00 in the Greek Day-Ahead Market (DAM)?

This project analyzes whether price spikes are driven purely by demand levels, or by residual demand ramps caused by declining renewable generation.

---

## Data

- Greek Day-Ahead Market results (HEnEx)
- System Load data (ADMIE)
- Renewable generation injections (ADMIE)
- Period: January 2025
- 744 hourly observations

---

## Methodology

1. Merge MCP, Load, and RES datasets
2. Compute Net Load = Load − RES
3. Compute hourly residual demand ramps
4. Analyze:
   - Correlations
   - Hourly averages
   - Ramp-price relationship

---

## Key Findings

- MCP correlates with Load (0.63)
- MCP correlates with Net Load (0.60)
- Peak prices occur at 17:00, before peak load (19:00)
- Strong positive relationship between price and positive residual load ramps

This suggests that Greek DAM prices are not purely demand-driven.
Evening solar decline creates ramp stress, triggering marginal fuel switching and price spikes.

---

## Conclusion

Electricity price spikes in January 2025 are partially driven by sunset ramp effects rather than absolute demand levels.

Energy markets respond to system stress — not just demand peaks.

---

## Repository Structure

- `data/` → processed dataset
- `figures/` → visualizations
- `notebooks/` → full analysis
- `requirements.txt` → dependencies

---

## Author

Ioannis Kamarinopoulos  
NTUA – Electrical & Computer Engineering  
Energy Markets & Power Systems
