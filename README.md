# When the Leaderboard Flips: Perturbation-Dependent Ranking in LLM Evaluation

## M20 Initial Capstone Report
Controlled Block-A experiment: **50 questions × 5 conditions × 4 LLMs = 1,000 audited observations**.

### Main findings
- Gemini 3.5 Flash Lite: **250/250 (100.0%)**
- Qwen 3.8-27B: **249/250 (99.6%)**
- GPT-OSS-20B: **248/250 (99.2%)**
- GPT-OSS-120B: **243/250 (97.2%)**
- all 10 errors are concentrated in three source questions
- perturbations can both degrade and repair responses
- relative model ranking/ties change across evaluation conditions

### Baseline ML
A class-weighted logistic regression uses pre-response features only and a deterministic question-group split to prevent leakage.
Test accuracy: **86.5%**; balanced accuracy: **43.8%**.
Because only 10/1,000 observations are errors, the classifier is a transparent M20 baseline rather than a strong failure-prediction claim.

### Structure
`notebooks/` final M20 notebook  
`data/processed/` audited analysis data and derived tables  
`figures/` high-resolution PNG + vector PDF figures  
`docs/` executive summary  
`provenance/` audit hash and methodology note

Pilot and qualification observations are excluded. No API keys are stored.
