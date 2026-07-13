# Grid Connection Feasibility Study — 50MW Solar Farm

## Overview
A power systems feasibility study assessing the grid connection of a 
proposed 50MW solar PV farm to a regional 132kV transmission network 
in Victoria, Australia.

## Tools Used
- Python (pandapower)
- Jupyter Notebook
- Microsoft Word

## Studies Conducted
- Steady-state load flow analysis (base case and full output)
- Voltage sensitivity analysis (0 to 50MW in 10MW steps)
- Three-phase fault level analysis (IEC 60909)

## Key Findings
- All bus voltages within NER compliance limits (0.90–1.10 pu)
- Maximum voltage at solar farm bus: 1.012 pu at full output
- All equipment within thermal limits (max loading: 86.44%)
- Fault levels within assumed switchgear ratings at all buses
- Connection assessed as technically feasible

## Network Description
| Element | Details |
|---|---|
| External Grid | 132 kV, Zsc = 2500 MVA |
| 132kV Line | 25 km, ACSR overhead |
| Transformer | 60 MVA, 132/33 kV |
| 33kV Feeder | 2 km, dedicated collector |
| Solar Farm | 50 MW, inverter-based PV |

## Repository Structure
- `Solar Project.ipynb` — pandapower model and analysis
- `Grid Connection Study Report.pdf` — full technical report
- `voltage_profile.png` — voltage sensitivity chart

## References
- AEMO, National Electricity Rules, S5.1.4
- IEC 60909-0:2016
- Glover, Sarma & Overbye, Power Systems Analysis and Design
