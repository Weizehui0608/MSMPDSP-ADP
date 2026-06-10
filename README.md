# MSMPDSP-ADP — Experimental Data

Experimental data for the paper:

> **How to Dynamically Schedule Multiple Knowledge-Intensive Projects Under Uncertainty? An Approximate Dynamic Programming Approach**
> Hongbo Li, Wei Chen, Zehui Wei, Qingkang Zhu, Xianchao Zhang. **Systems** .

## Contents
`Experimental_Data.xlsx` — a single workbook with the following sheets:

| Sheet | Content |
|---|---|
| `README` | Sheet-by-sheet description and metric glossary. |
| `Table7_Solution_Performance` | Table 7 — solution performance of Rollout vs. Q-Learning (scenarios A/B/C). |
| `Table8_Project_Completion` | Table 8 — project completion outcomes. |
| `Fig3_ARD` | Figure 3 — Average Relative Deviation between Rollout and Q-Learning total cost. |
| `Table9_Sensitivity_Performance` | Table 9 — sensitivity of solution performance to workers (K) and skills (S). |
| `Table10_Sensitivity_Completion` | Table 10 — sensitivity of project completion to K and S. |
| `Fig4_5_Sensitivity_Grids` | Figures 4–5 — K × S grids of total cost and completion rate. |
| `ARD_PerInstance` | Per-instance Rollout and Q-Learning total cost (raw data behind Fig. 3). |
| `Metadata` | Experimental setup and parameter ranges. |

## Metric glossary

- **C_total** — total human-resource cost
- **C_efficiency** — completed projects per unit cost
- **K_rate** — average worker utilization rate
- **TDS** — total number of delayed stages
- **C_rate** — project completion rate
- **ARD** — Average Relative Deviation, mean of (Q - R)/R; a positive value means Rollout is cheaper than Q-Learning

Each main-experiment configuration is averaged over 10 independent test instances. Project arrivals follow a Bernoulli process (probability 0.5); durations are integers in [1, 7] sampled at arrival and held fixed; skill efficiencies are integers in [1, 10].


## Contact

Corresponding authors: Zehui Wei (wzh010608@shu.edu.cn), Xianchao Zhang (zhangxianchao@zjxu.edu.cn).
