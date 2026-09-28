# 你好，我是 Jiaqi Yang

[English](README.md) | **简体中文**

我是香港理工大学和萨里大学的经济学研究者，在做用大语言模型（能理解和生成文字的 AI 模型）辅助投资研究的工具，以及机器学习预测模型。我关心两件事：一是自动化流程每天不用我管也能自己跑；二是衡量模型到底有没有做对。

## 项目

| 项目 | 简介 |
|---|---|
| **[finfluencer-digest](https://github.com/jackieyangjq/finfluencer-digest)** | 每日个股观点摘要：Gemini 看 16 个 YouTube 财经频道和一批 X 账号，提取观点、汇总共识，每天发邮件。多模型备用、定时运行、新闻来源核对。 |
| **[ml-inflation-forecasting](https://github.com/jackieyangjq/ml-inflation-forecasting)**（机器学习通胀预测） | 用 FRED-MD 的 121 个宏观指标和机器学习预测美国通胀，复现 Medeiros 等（2021）。2001–2015 年树模型的预测误差比 AR 基准低 15–20%，2020 年后优势消失。 |
| **[applied-stats-econometrics-toolkit](https://github.com/jackieyangjq/applied-stats-econometrics-toolkit)**（统计与计量方法工具箱） | 我在研究中用的统计与计量方法，每个都在模拟数据上检验过：分批实施的 DID、带固定效应的分位数回归、VAR、有界结果模型、变点检测。 |
| **[llm-text-measurement](https://github.com/jackieyangjq/llm-text-measurement)**（用大模型做文本测量） | 用大模型标注 998 条酒店评论，并从六个角度检验：与住客本人好评 / 差评分栏的一致率 94.6%，换一个模型的一致性 α = 0.93，阴性对照零误报。 |
| **[热量记录](https://github.com/jackieyangjq/caltrk)** · [在线使用](https://jackieyangjq.github.io/caltrk/) | 离线网页应用：用视觉模型识别食物照片，用真实体重数据校准热量估计。七周发布 20 个版本。 |
| **[filings-qa-agent](https://github.com/jackieyangjq/filings-qa-agent)**（财报问答研究助手） | 美国上市公司年报季报问答：每句话都有可核对的出处，带会调用工具的研究智能体，50 题检索评测（关键词检索答对 95%）。 |
| **[catfolio fork](https://github.com/jackieyangjq/catfolio)**（投资面板） | 投资面板的 fork：加了券商同步和观点记分牌，按之后的股价给个股观点打分。已向上游提交 4 个 PR。 |

## 开源贡献

- [ClaudeCodeUsage](https://github.com/ClaudeCodeUsage/ClaudeCodeUsage)（VS Code 编辑器的扩展，TypeScript 编写）：[#115](https://github.com/ClaudeCodeUsage/ClaudeCodeUsage/pull/115) 给仪表盘的日期标签格式化函数加了缓存（同样的输入只算一次），修复了 #99，2026 年 9 月合并。
- [catfolio](https://github.com/irrwood/catfolio)（FastAPI 写的投资组合面板，Python）：[#4](https://github.com/irrwood/catfolio/pull/4) 港股代码补零与港币汇率、[#5](https://github.com/irrwood/catfolio/pull/5) 清理失效链接、[#6](https://github.com/irrwood/catfolio/pull/6) 长桥账户同步、[#7](https://github.com/irrwood/catfolio/pull/7) 观点记分牌工作区；2026 年 9 月提交。

## 最近在做

- 在扩展 catfolio：长桥同步和观点记分牌已在 fork 里上线，四个 PR 等上游审阅（2026 年 9 月）。
- 财经博主的个股观点正在记分牌里逐步到期：最早的 5 日结果 2026 年 9 月底出来，63 日结果 12 月出来。

## 联系方式

jiaqi.yang@surrey.ac.uk
