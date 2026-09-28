# 你好，我是 Jiaqi Yang

[English](README.md) | **简体中文**

我是香港理工大学和萨里大学的经济学研究者，在做用大语言模型（能理解和生成文字的 AI 模型）辅助投资研究的工具，以及机器学习预测模型。我关心两件事：一是自动化流程每天不用我管也能自己跑；二是衡量模型到底有没有做对。

## 项目

| 项目 | 简介 |
|---|---|
| **[finfluencer-digest](https://github.com/jackieyangjq/finfluencer-digest)** | 每天早上，Gemini 看 16 个 YouTube 财经频道和一批 X（原推特）账号，提取结构化的个股观点，汇总共识和分歧，再发一封摘要邮件。一个模型出错就自动换备用模型；用 GitHub Actions（GitHub 自带的自动化服务）定时运行，并加了一道检查，防止定时触发被漏掉；新闻都核对过来源，防止编造引用。用 Python 写成；有 27 个离线测试（不联网也能跑）、CI（每次提交代码都自动跑测试），以及不填密钥也能运行的演示模式。 |
| **[ml-inflation-forecasting](https://github.com/jackieyangjq/ml-inflation-forecasting)**（机器学习通胀预测） | 复现并扩展 Medeiros 等（2021，*JBES*）的美国 CPI 通胀预测研究：8 个模型，从 AR 基准（只用通胀自身历史）到 LASSO、随机森林和 XGBoost，用 FRED-MD 的 121 个宏观指标，在 2000–2026 年的 308 个滚动窗口里逐月重新训练；用 Diebold-Mariano 检验（判断两个模型的误差差距是否显著）和模型置信集比较准确度，用 SHAP 拆解每一次预测靠的是哪些指标。在论文原来的 2001–2015 年检验期，树模型的 12 个月预测误差比 AR 低 15–20%；2020 年以后没有模型胜过 AR。Python；有测试、CI，结果随仓库提供。 |
| **[applied-stats-econometrics-toolkit](https://github.com/jackieyangjq/applied-stats-econometrics-toolkit)**（统计与计量方法工具箱） | 我在研究中用到的统计与计量方法，用 Python 实现，每个方法都在真实答案已知的模拟数据上检验过：分批实施政策的双重差分（双向固定效应与 Callaway-Sant'Anna、Sun-Abraham 等新方法对比，Goodman-Bacon 分解，随机化推断，空间相关标准误），组内相关系数与 Shapley-Owen 方差分解，带固定效应的分位数回归（MMQR），VAR 与格兰杰因果检验、脉冲响应，有界结果的 Tobit 模型与 Oster 敏感性分析，PELT 变点检测与 Bass 扩散模型。24 个测试、CI。 |
| **[llm-text-measurement](https://github.com/jackieyangjq/llm-text-measurement)**（用大模型做文本测量） | 用大模型把文本变成研究数据，并检验测量是否可靠：gpt-5.5 为 998 条公开酒店评论标注提到的方面、褒贬，并逐字引用原文作证据。标签与住客本人"喜欢 / 不喜欢"分栏的一致率为 94.6%（κ = 0.89），同一模型重跑的一致性 α = 0.96，换 claude-sonnet-5 为 0.93，60 条阴性对照零误报。可断点续跑的批处理、附检索示例的第二轮复核、token 用量记录；另以 Word2Vec 词典和蒸馏分类器作为廉价基线对比。 |
| **[热量记录](https://github.com/jackieyangjq/caltrk)** · [在线使用](https://jackieyangjq.github.io/caltrk/) | 单文件、离线优先（不联网也能用）的网页应用：用视觉模型（能看懂图片的 AI 模型）识别食物，对模型输出做算术交叉验证（用算术把几个数互相核对），每周用真实体重数据校准热量收支模型。六周发布了 24 个版本。 |
| **[filings-qa-agent](https://github.com/jackieyangjq/filings-qa-agent)**（财报问答研究助手） | 在 SEC 披露文件（美国上市公司交给美国证监会的年报、季报）里检索并回答，每句话都带可核对的出处（引用了没给模型看过的段落的句子整句删掉）；一个会调用工具、每步留轨迹的研究智能体（能自己决定下一步做什么的 AI 程序）；一套 50 题的评测，比较关键词检索、向量检索（按语义相近程度查找）和混合检索：关键词答对 95%，混合 90%，向量 70%，30 组不可答题全部正确弃答。用 SQLite 的全文索引加 numpy 代替向量数据库；168 个离线测试、CI、离线演示。 |
| **[catfolio fork](https://github.com/jackieyangjq/catfolio)**（投资面板） | 一个本地优先的投资组合面板（上游 irrwood/catfolio，MIT 许可），我加了长桥券商账户同步和一个“观点记分牌”工作区：导入任何来源的个股看多看空观点，按之后的价格走势评分，给每个来源画“每次都跟”的净值曲线和逐月命中率。四个 PR 已提交到上游。 |

## 开源贡献

- [ClaudeCodeUsage](https://github.com/ClaudeCodeUsage/ClaudeCodeUsage)（VS Code 编辑器的扩展，TypeScript 编写）：[#115](https://github.com/ClaudeCodeUsage/ClaudeCodeUsage/pull/115) 给仪表盘的日期标签格式化函数加了缓存（同样的输入只算一次），修复了 #99，2026 年 9 月合并。
- [catfolio](https://github.com/irrwood/catfolio)（FastAPI 写的投资组合面板，Python）：[#4](https://github.com/irrwood/catfolio/pull/4) 港股代码补零与港币汇率、[#5](https://github.com/irrwood/catfolio/pull/5) 清理失效链接、[#6](https://github.com/irrwood/catfolio/pull/6) 长桥账户同步、[#7](https://github.com/irrwood/catfolio/pull/7) 观点记分牌工作区；2026 年 9 月提交。

## 最近在做

- 在扩展 catfolio：长桥同步和观点记分牌已在 fork 里上线，四个 PR 等上游审阅（2026 年 9 月）。
- 财经博主的个股观点正在记分牌里逐步到期：最早的 5 日结果 2026 年 9 月底出来，63 日结果 12 月出来。

## 联系方式

jiaqi.yang@surrey.ac.uk
