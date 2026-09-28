# Hi, I'm Jiaqi Yang

**English** | [简体中文](README.zh-CN.md)

Economics researcher at The Hong Kong Polytechnic University and the University of Surrey, building LLM-powered tools for investment research and machine-learning forecasting models. I care about pipelines that run every day without me, and about measuring whether the model actually got it right.

## Projects

| Project | What it is |
|---|---|
| **[finfluencer-digest](https://github.com/jackieyangjq/finfluencer-digest)** | Every morning, Gemini watches 16 YouTube finance channels and a set of X accounts, extracts structured stock calls, aggregates consensus and disagreement, and emails a digest. Multi-model fallback, GitHub Actions scheduling with a gate against dropped cron triggers, and source-verified news to prevent fabricated citations. Python; 27 offline tests, CI, demo mode that runs without keys. |
| **[ml-inflation-forecasting](https://github.com/jackieyangjq/ml-inflation-forecasting)** | Replication and extension of Medeiros et al. (2021, *JBES*) on US CPI inflation: 8 models from a BIC-lag AR to LASSO, random forest and XGBoost, refitted monthly on 121 FRED-MD series over 308 rolling windows (2000-2026), with Diebold-Mariano tests, a model confidence set and SHAP explanations of every forecast. On the paper's 2001-2015 period the tree models cut 12-month RMSE by 15-20% against AR; from 2020 on no model beats it. Python; tests, CI, results committed. |
| **[applied-stats-econometrics-toolkit](https://github.com/jackieyangjq/applied-stats-econometrics-toolkit)** | Statistical and econometric methods I use in research, in Python, each checked on simulated data where the true answer is known: staggered difference-in-differences (TWFE against Callaway-Sant'Anna and Sun-Abraham, Goodman-Bacon decomposition, randomization inference, Conley standard errors), ICC and Shapley-Owen decompositions, fixed-effects quantile regression (MMQR), VAR with Granger tests and impulse responses, Tobit and Oster bounds for bounded outcomes, PELT change points and Bass diffusion. 24 tests, CI. |
| **[llm-text-measurement](https://github.com/jackieyangjq/llm-text-measurement)** | Turning text into research data with an LLM, and checking the measurement: gpt-5.5 labels the aspects, polarity and a verbatim quote for 998 public hotel reviews. The labels agree with the guests' own liked/disliked split 94.6% of the time (kappa 0.89), with a repeat run at alpha 0.96 and with claude-sonnet-5 at 0.93, and invent nothing on 60 negative controls. Resumable batches, a second pass with retrieved examples, a token ledger; a Word2Vec dictionary and a distilled classifier as cheaper baselines. |
| **[Calorie tracker](https://github.com/jackieyangjq/caltrk)** · [live](https://jackieyangjq.github.io/caltrk/) | Single-file offline-first web app with vision-model food recognition, arithmetic cross-checks on model output, and weekly calibration of the energy model against real weight data. 24 releases in six weeks. |
| **[filings-qa-agent](https://github.com/jackieyangjq/filings-qa-agent)** | Question answering over SEC 10-K/10-Q filings with a checkable source on every sentence (sentences citing unseen passages are dropped), a traced tool-using research agent, and an evaluation of 50 questions comparing keyword, vector and hybrid retrieval (BM25 95% correct, hybrid 90%, vector 70%; all 30 unanswerable pairs declined). SQLite FTS5 and numpy instead of a vector database; 168 offline tests, CI, offline demo. |
| **[catfolio fork](https://github.com/jackieyangjq/catfolio)** | A local-first portfolio dashboard (upstream: irrwood/catfolio, MIT) extended with Longbridge account sync and a call-tracker workspace that scores stock calls from any source against later prices, with a follow-every-call curve and monthly hit rates per source. Four pull requests open upstream. |

## Open source

- [ClaudeCodeUsage](https://github.com/ClaudeCodeUsage/ClaudeCodeUsage) (VS Code extension, TypeScript): [#115](https://github.com/ClaudeCodeUsage/ClaudeCodeUsage/pull/115) memoised the dashboard date-label formatter (fixes #99), merged September 2026.
- [catfolio](https://github.com/irrwood/catfolio) (FastAPI portfolio dashboard, Python): [#4](https://github.com/irrwood/catfolio/pull/4) HK symbol zero-padding and HKD FX, [#5](https://github.com/irrwood/catfolio/pull/5) dead links, [#6](https://github.com/irrwood/catfolio/pull/6) Longbridge account sync, [#7](https://github.com/irrwood/catfolio/pull/7) call-tracker workspace; opened September 2026.

## Now

- Extending catfolio: Longbridge sync and the call tracker are in the fork, with pull requests open upstream (September 2026).
- Scoring influencer stock calls in the call tracker as they mature: the first 5-day results land at the end of September 2026, the 63-day ones in December.

## Contact

jiaqi.yang@surrey.ac.uk
