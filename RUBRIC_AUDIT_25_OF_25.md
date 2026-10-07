# M20 Final 25/25 Rubric Audit

## Verdict
**Submission-ready: 25/25 target supported by the package.**

The canonical notebook was executed from a clean extracted repository layout and completed with **zero execution errors**. The executive-summary DOCX was rendered and visually inspected page by page.

## 1. Organization — 5/5
Clear research/business question; logical report flow; interpretation accompanies results; README, notebook, figures, and executive summary are numerically consistent.

## 2. Syntax and code quality — 5/5
The canonical notebook executes end-to-end without errors. Assertions verify the 1,000-row grid. The question-level split is deterministic and reproducible. No API calls or credentials are required for analysis.

## 3. Visualizations — 5/5
Seven focused figures are supplied as high-resolution PNG and vector PDF. They include categorical model/condition/benchmark comparisons and a continuous prompt-length visualization, plus ranking, transition, error-pattern, and model-evaluation graphics.

## 4. Cleaning, EDA, and feature engineering — 5/5
Analysis starts from the jointly audited 1,000-observation production freeze. Integrity assertions cover row count, IDs, experimental dimensions, target validity, QA validity, and grid completeness. Pre-response engineered features are documented. Pilot and qualification rows are excluded.

## 5. Modeling — 5/5
Logistic regression supplies the learned baseline. Predictors are pre-response only. Train/test assignment is grouped by original question_id. Ordinary accuracy, balanced accuracy, and confusion matrix are reported, with severe class imbalance interpreted transparently.

## Scientific consistency
- 1,000 observations = 50 questions × 5 conditions × 4 models.
- Gemini 3.5 Flash Lite: 250/250 = 100.0%.
- Qwen 3.8-27B: 249/250 = 99.6%.
- GPT-OSS-20B: 248/250 = 99.2%.
- GPT-OSS-120B: 243/250 = 97.2%.
- 10 errors concentrated in 3 source questions.
- Logistic-regression test accuracy: 86.5%; balanced accuracy: 43.8%.
- Grouped test split: 13 questions / 260 observations / 3 errors.
- No unsupported population-level claim is made from Block A.

## Submission gate
**PASS.** Remaining operational step: upload this exact repository content to GitHub, verify rendering, then submit the repository URL.
