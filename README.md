# DRL-LP
Hybrid DRL &amp; LP optimization framework

## Notebook Description
| File | Description |
|---|---|
| `Make MMH dataset.ipynb` | Constructs training, validation, and test datasets for the ReCovNet model using pre-processed demand points and candidate MMH supply sites in Seoul. Each training sample consists of demand point information, randomly sampled candidate sites, service radius, and the target number of selected facilities. |
| `LP evaluation.ipynb` | Evaluates the performance of the MCLP-based Linear Programming model using Gurobi Optimizer. The notebook compares objective value and runtime across different settings of candidate sites and selected facility sites. |
| `DRL evaluation.ipynb` | Evaluates the location selection performance of the ReCovNet-based Deep Reinforcement Learning model. The notebook calculates objective value and runtime from DRL inference results and compares them with LP-based results. |
| `DRL-LP for MMH.ipynb` | Applies the proposed DRL–LP hybrid framework. ReCovNet first selects an intermediate candidate set, and Gurobi-based LP then determines the final MMH locations from the reduced candidate set. |

## Training environment
| Category | Item | Setting |
|---|---|---|
| Computing environment | CPU | 13th Gen Intel® Core™ i7-13700KF |
| Computing environment | GPU | NVIDIA GeForce RTX 3080 12GB |
| Computing environment | RAM | 32 GB |
| Computing environment | OS | Windows 11 |
| Software | Python | 3.8.20 |
| Software | NumPy | 1.23.5 |
| Software | PyTorch | 1.8.0 |
