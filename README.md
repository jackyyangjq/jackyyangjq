# Hi, I'm Jiaqi Yang

**English** | [简体中文](README.zh-CN.md)

Economics researcher at The Hong Kong Polytechnic University and the University of Surrey, building LLM-powered tools for investment research and machine-learning forecasting models. I care about pipelines that run every day without me, and about measuring whether the model actually got it right.

## Projects

| Project | What it is |
|---|---|
| **[finfluencer-digest](https://github.com/jackieyangjq/finfluencer-digest)** | Daily digest of stock calls: Gemini watches 16 YouTube finance channels and X accounts, extracts each call and sums up the consensus. Multi-model fallback, scheduled runs, source-checked news. |
| **[ml-inflation-forecasting](https://github.com/jackieyangjq/ml-inflation-forecasting)** | Machine-learning forecasts of US inflation from 121 FRED-MD series, replicating Medeiros et al. (2021). Tree models cut forecast error by 15-20% against an AR benchmark in 2001-2015, but not since 2020. |
| **[applied-stats-econometrics-toolkit](https://github.com/jackieyangjq/applied-stats-econometrics-toolkit)** | Statistics and econometrics I use in research, each checked on simulated data: staggered DiD, quantile regression with fixed effects, VAR, bounded-outcome models, change points. |
| **[llm-text-measurement](https://github.com/jackieyangjq/llm-text-measurement)** | LLM labelling of 998 hotel reviews, validated six ways: 94.6% agreement with the guests' own liked/disliked split, alpha 0.93 against a second model, no false labels on controls. |
| **[Calorie tracker](https://github.com/jackieyangjq/caltrk)** · [live](https://jackieyangjq.github.io/caltrk/) | Offline web app that recognises food from photos with a vision model and calibrates calorie estimates against real weight data. 20 versions in seven weeks. |
| **[filings-qa-agent](https://github.com/jackieyangjq/filings-qa-agent)** | Question answering over SEC filings with a checkable source for every sentence, a tool-using research agent, and a 50-question retrieval evaluation (keyword search 95% correct). |
| **[catfolio fork](https://github.com/jackieyangjq/catfolio)** | Portfolio dashboard fork with broker sync and a tracker that scores stock calls against later prices. Four pull requests upstream. |

## Open source

- [ClaudeCodeUsage](https://github.com/ClaudeCodeUsage/ClaudeCodeUsage) (VS Code extension, TypeScript): [#115](https://github.com/ClaudeCodeUsage/ClaudeCodeUsage/pull/115) memoised the dashboard date-label formatter (fixes #99), merged September 2026.
- [catfolio](https://github.com/irrwood/catfolio) (FastAPI portfolio dashboard, Python): [#4](https://github.com/irrwood/catfolio/pull/4) HK symbol zero-padding and HKD FX, [#5](https://github.com/irrwood/catfolio/pull/5) dead links, [#6](https://github.com/irrwood/catfolio/pull/6) Longbridge account sync, [#7](https://github.com/irrwood/catfolio/pull/7) call-tracker workspace; opened September 2026.

## Now

- Extending catfolio: Longbridge sync and the call tracker are in the fork, with pull requests open upstream (September 2026).
- Scoring influencer stock calls in the call tracker as they mature: the first 5-day results land at the end of September 2026, the 63-day ones in December.

## Contact

jiaqi.yang@surrey.ac.uk
