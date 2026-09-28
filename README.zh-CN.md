<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/banner-dark.svg">
  <img alt="杨嘉琦（Jiaqi Yang），香港理工大学与萨里大学双博士候选人" src="assets/banner-light.svg" width="100%">
</picture>

<p align="center">
  <a href="https://jackyyangjq.github.io"><b>个人网站</b></a> &nbsp;·&nbsp;
  <a href="https://jackyyangjq.github.io/files/Jiaqi_Yang_CV_Academic.pdf">学术版简历</a> &nbsp;·&nbsp;
  <a href="https://jackyyangjq.github.io/files/Jiaqi_Yang_CV_Industry.pdf">业界版简历</a> &nbsp;·&nbsp;
  <a href="https://www.linkedin.com/in/jiaqi-yang-7b8813326">LinkedIn</a> &nbsp;·&nbsp;
  <a href="mailto:jiaqi.yang@surrey.ac.uk">邮箱</a>
  <br>
  <a href="README.md">English</a> · <b>简体中文</b>
</p>

我研究数字技术和公共政策如何改变旅游与酒店市场，方法上结合因果推断、时间序列模型，以及把大语言模型当作文本测量工具。我正在求职（2026–27 年），方向包括高校教职，以及业界的研究、数据科学和量化岗位。

- 2026 年获 IATE 与 CHME 两个国际会议的最佳论文奖
- 论文在 *Annals of Tourism Research* 和 *Journal of Travel Research* 修改后再审
- 公开研究方法代码，每个方法都在答案已知的数据上检验过

## 研究方法代码

<table>
  <tr>
    <td width="33%" valign="top">
      <a href="https://github.com/jackyyangjq/applied-stats-econometrics-toolkit"><img src="https://raw.githubusercontent.com/jackyyangjq/applied-stats-econometrics-toolkit/main/figures/did_event_study.png" alt="模拟的分批实施政策事件研究：三种估计方法与真实效应对比"></a>
      <p><b><a href="https://github.com/jackyyangjq/applied-stats-econometrics-toolkit">applied-stats-econometrics-toolkit</a></b>（统计与计量方法工具箱）<br>我在研究中用的统计与计量方法，每个都在模拟数据上检验过：分批实施的 DID、带固定效应的分位数回归、VAR、有界结果模型、变点检测。</p>
    </td>
    <td width="33%" valign="top">
      <a href="https://github.com/jackyyangjq/llm-text-measurement"><img src="https://raw.githubusercontent.com/jackyyangjq/llm-text-measurement/main/figures/validation.png" alt="大模型标签与重跑、换模型和廉价基线的一致性"></a>
      <p><b><a href="https://github.com/jackyyangjq/llm-text-measurement">llm-text-measurement</a></b>（用大模型做文本测量）<br>用大模型标注 998 条酒店评论，并从六个角度检验：与住客本人好评 / 差评分栏的一致率 94.6%，换一个模型的一致性 α = 0.93，阴性对照零误报。</p>
    </td>
    <td width="33%" valign="top">
      <a href="https://github.com/jackyyangjq/ml-inflation-forecasting"><img src="https://raw.githubusercontent.com/jackyyangjq/ml-inflation-forecasting/main/figures/forecasts_h12.png" alt="美国未来 12 个月通胀：实际值与随机森林、AR 模型预测值"></a>
      <p><b><a href="https://github.com/jackyyangjq/ml-inflation-forecasting">ml-inflation-forecasting</a></b>（机器学习通胀预测）<br>用 FRED-MD 的 121 个宏观指标和机器学习预测美国通胀，复现 Medeiros 等（2021）。2001–2015 年树模型的预测误差比 AR 基准低 15–20%，2020 年后优势消失。</p>
    </td>
  </tr>
</table>

## 工具与应用

| 项目 | 简介 |
|---|---|
| **[filings-qa-agent](https://github.com/jackyyangjq/filings-qa-agent)**（财报问答研究助手） | 美国上市公司年报季报问答：每句话都有可核对的出处，带会调用工具的研究智能体，50 题检索评测（关键词检索答对 95%）。 |
| **[finfluencer-digest](https://github.com/jackyyangjq/finfluencer-digest)** | 每日个股观点摘要：Gemini 看 16 个 YouTube 财经频道和一批 X 账号，提取观点、汇总共识，每天发邮件。多模型备用、定时运行、新闻来源核对。 |
| **[catfolio fork](https://github.com/jackyyangjq/catfolio)**（投资面板） | 投资面板的 fork：加了券商同步和观点记分牌，按之后的股价给个股观点打分。已向上游提交 4 个 PR。 |
| **[热量记录](https://github.com/jackyyangjq/caltrk)** · [在线使用](https://jackyyangjq.github.io/caltrk/) | 离线网页应用：用视觉模型识别食物照片，用真实体重数据校准热量估计。七周发布 20 个版本。 |

## 开源贡献

- [ClaudeCodeUsage](https://github.com/ClaudeCodeUsage/ClaudeCodeUsage)（VS Code 扩展，TypeScript）：[#115](https://github.com/ClaudeCodeUsage/ClaudeCodeUsage/pull/115) 给仪表盘的日期标签格式化加了缓存（修复 #99），2026 年 9 月合并。
- [catfolio](https://github.com/irrwood/catfolio)（FastAPI 投资面板，Python）：[#4](https://github.com/irrwood/catfolio/pull/4) 港股代码补零与港币汇率、[#5](https://github.com/irrwood/catfolio/pull/5) 清理失效链接、[#6](https://github.com/irrwood/catfolio/pull/6) 券商账户同步、[#7](https://github.com/irrwood/catfolio/pull/7) 观点记分牌工作区；2026 年 9 月提交。

## 个人网站的访客来自哪里

<p align="center">
  <a href="https://jackyyangjq.github.io/visitors/"><img src="https://jackyyangjq-visits.jackyyangjq.workers.dev/map.svg" width="100%" alt="个人网站访问的世界地图，每小时更新"></a>
  <br><sub>由网站自己的计数程序统计，不用 cookie，每小时更新。<a href="https://jackyyangjq.github.io/visitors/">城市、来源和每日访问</a></sub>
</p>
