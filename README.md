# 🏛️ Finance LLM Zoo · 开源金融大模型动物园

> **公益策展 · 来自顶尖高校与研究机构的开源金融大模型 · 免费、开放、无需注册**

[![Curation](https://img.shields.io/badge/Curated%20by-AgentPit-orange)](https://github.com/agentpit-io)
[![Open Source First](https://img.shields.io/badge/Open%20Source-First-blue)](#-策展原则)
[![Free API](https://img.shields.io/badge/API-Free%20Forever-green)](https://develop.agentpit.io/help)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

**🌐 项目主页 (完整对比 + 交互):** [www.agentpit.io/finance-llm-zoo](https://www.agentpit.io/finance-llm-zoo)  
**🔬 上游研究仓库 (原始 changelog / issue 讨论):** [hangeaiagent/kronos-free-api](https://github.com/hangeaiagent/kronos-free-api)  
**📖 免费 API 完整文档:** [develop.agentpit.io/help](https://develop.agentpit.io/help)

---

## 🎯 项目定位

**Finance LLM Zoo** 是 [AgentPit](https://github.com/agentpit-io) 团队公益维护的开源金融大模型策展项目 —— 收录来自**清华、上海财经、复旦、同济、哥伦比亚、武汉大学、度小满、北京中关村学院**等顶尖机构的开源金融基础模型,并为其中已支持的模型提供**永久免费的 API 接入**,方便研究者、学生、独立开发者零成本调用。

**已收录 8 个模型 · 已提供免费 API 5 个 · 策展中待接入 3 个**

## 📜 策展原则

1. **开源优先** · 只收录采用 OSI 认可开源许可证(MIT / Apache 2.0 / CC BY-NC 等)的模型 · 拒绝闭源与"开源展示但不能用"的伪开源
2. **如实公示** · 每个模型的局限、许可证限制、部署成本、缺陷都直接列出 · 不美化不遮掩
3. **免费共享** · 对已提供 API 的模型 · 承诺永久免费供个人研究 / 学习 / 独立开发使用 · 不设注册墙
4. **上游致敬** · 所有 API 均标注原始论文、作者、GitHub 仓库 · 鼓励用户去原仓库 Star、引用、贡献

---

## 📚 收录模型清单

### ✅ 已提供免费 API (5)

#### 1. [Fin-R1](https://github.com/SUFE-AIFLM-Lab/Fin-R1) · 上海财经大学

[![GitHub Stars](https://img.shields.io/github/stars/SUFE-AIFLM-Lab/Fin-R1?style=flat)](https://github.com/SUFE-AIFLM-Lab/Fin-R1) [![License](https://img.shields.io/badge/License-Apache%202.0-blue)](https://github.com/SUFE-AIFLM-Lab/Fin-R1/blob/main/LICENSE)

- **机构** · 上海财经大学 AI-FLM Lab
- **发布** · 2024 年 · 底座:自研(DeepSeek-R1 微调)
- **定位** · A 股专项金融推理模型 · AgentPit 首个上线的金融大模型 API
- **核心能力** · 研报解读 / 财报问答 / 投资逻辑分析 · 思维链推理 · OpenAI messages 兼容格式
- **性能** · 中文金融 NLP 评测超越同规模通用模型 · 财报问答准确率 78%+
- **局限** · 主要覆盖 A 股 · 港股/美股任务性能有限
- **免费 API** · `POST /api/v1/open-api/llm` → [详情](https://www.agentpit.io/finance-models/fin-r1)

#### 2. [Kronos](https://github.com/shiyu-coder/Kronos) · 清华大学(IIIS 交叉信息研究院 + 自动化系)

[![GitHub Stars](https://img.shields.io/github/stars/shiyu-coder/Kronos?style=flat)](https://github.com/shiyu-coder/Kronos) [![License](https://img.shields.io/badge/License-MIT-yellow)](https://github.com/shiyu-coder/Kronos/blob/main/LICENSE) [![Paper](https://img.shields.io/badge/Paper-arXiv%3A2508.02739-red)](https://arxiv.org/abs/2508.02739)

- **机构** · 清华大学 IIIS 交叉信息研究院 + 自动化系
- **发布** · 2025 年 8 月(AAAI 2026 录用)· 底座:自研自回归 Transformer(4.1M ~ 499M 参数)
- **定位** · 全球首个专为金融 K 线数据预训练的开源基础大模型 · "把 K 线当语言来学"
- **核心能力** · 价格序列预测 / 波动率预测 / 合成 K 线生成 / 零样本跨资产泛化(股/期/汇/加密) · 45+ 交易所 · 120 亿条 K 线预训练
- **性能** · 零样本 RankIC 超 TimesFM +93% · 波动率 MAE 优于所有基线 9% · 回测保真度提升 22%
- **局限** · 只处理 K 线价量数据 · 无文本能力 · 499M 大版本未开源 · 需 Qlib 接入 A 股回测
- **在线 Demo** · [shiyu-coder.github.io/Kronos-demo](https://shiyu-coder.github.io/Kronos-demo/)
- **免费 API** · `POST /api/v1/open-api/kronos` → [详情](https://www.agentpit.io/finance-models/kronos)

#### 3. [FinGPT](https://github.com/AI4Finance-Foundation/FinGPT) · AI4Finance · 哥伦比亚大学

[![GitHub Stars](https://img.shields.io/github/stars/AI4Finance-Foundation/FinGPT?style=flat)](https://github.com/AI4Finance-Foundation/FinGPT) [![License](https://img.shields.io/badge/License-MIT-yellow)](https://github.com/AI4Finance-Foundation/FinGPT/blob/main/LICENSE)

- **机构** · AI4Finance Foundation · 哥伦比亚大学
- **发布** · 2023 年(持续更新)· 底座:多选 LLaMA-2 / ChatGLM2 / Qwen / InternLM
- **定位** · 开源金融 LLM 框架(非单一固定模型)· 四大模组灵活组合
- **核心能力** · 金融咨询 · 文本情感分析 · 内嵌财务公式(ROE/DCF)· RAG 检索问答
- **性能** · 金融 NLP / 试题 / 资料 / 时事 四维度全能 · 中文咨询超越同期多数开源模型
- **局限** · 底座 Baichuan-13B 偏老 · 推理深度弱于轩辕 FinX1 · 2024 年后无重大更新
- **免费 API** · `POST /api/v1/open-api/fingpt` → [详情](https://www.agentpit.io/finance-models/fingpt)

#### 4. [CFGPT](https://github.com/TongjiFinLab/CFGPT) · 同济大学 FinLab · 上海人工智能实验室

[![GitHub Stars](https://img.shields.io/github/stars/TongjiFinLab/CFGPT?style=flat)](https://github.com/TongjiFinLab/CFGPT) [![License](https://img.shields.io/badge/License-Apache%202.0-blue)](https://github.com/TongjiFinLab/CFGPT/blob/main/LICENSE)

- **机构** · 同济大学 FinLab · 上海人工智能实验室
- **发布** · 2023 年 · 底座:InternLM / GLM-4 (6B / 9B)
- **定位** · 中文金融 GPT · 聚焦 A 股市场研究
- **核心能力** · 年报深度解析 · 研究报告生成 · 财务指标计算(ROE/PE/DCF)· A 股监管适配
- **性能** · 年报结构化提取 F1 值超同期所有开源模型 · 中文金融 NLP 综合超 GPT-3.5(2023 测试)
- **局限** · 高度垂直年报场景 · 实时行情/消息面弱 · 无完整思维链输出
- **免费 API** · `POST /api/v1/open-api/cfgpt` → [详情](https://www.agentpit.io/finance-models/cfgpt)

#### 5. [M3](https://github.com/ArthurZhang02/m3-market-microstructure) · 北京中关村学院

[![License](https://img.shields.io/badge/License-CC%20BY--NC%204.0-red)](https://github.com/ArthurZhang02/m3-market-microstructure) [![Paper](https://img.shields.io/badge/Paper-arXiv%3A2608.19227-red)](https://arxiv.org/abs/2608.19227)

- **机构** · 北京中关村学院(Zhang et al. · AAAI 系列)
- **发布** · 2026 年 8 月 · 底座:自研 VQ Tokenizer + 因果 Transformer
- **定位** · **市场微观结构生成式基础模型** · 不预测涨跌 · 生成未来订单流轨迹
- **核心能力** · 生成挂单/撤单序列(价格由撮合规则还原)· 冲击成本估计 · 反事实分析 · 采样式而非确定式
- **训练数据** · 沪深300 + 中证500 共 800 只标的 · 约 319 亿条逐笔委托事件
- **性能** · 开源三档 Tiny 10M / Small 25M / Base 75M · CPU 即可推理(单次模拟约 30 秒)· 复现市场典型事实
- **局限** · **非文本模型**,不能问答 · 原生输入需付费 Level-2 数据(API 只提供内置样本模拟)· 366M / 1.27B 未开源 · **CC BY-NC 4.0 商用需授权** · 约 1/3 时间间隔为负(已反馈上游)
- **免费 API** · `POST /api/v1/open-api/microstructure` → [详情](https://www.agentpit.io/finance-models/m3)

---

### ⏳ 策展中·待接入 API (3)

#### 6. [轩辕 XuanYuan FinX1](https://github.com/Duxiaoman-DI/XuanYuan) · 度小满 AI-Lab

[![GitHub Stars](https://img.shields.io/github/stars/Duxiaoman-DI/XuanYuan?style=flat)](https://github.com/Duxiaoman-DI/XuanYuan) [![License](https://img.shields.io/badge/License-Apache%202.0-blue)](https://github.com/Duxiaoman-DI/XuanYuan/blob/main/LICENSE)

- **机构** · 度小满 AI-Lab · **发布** · 2024 年 12 月 · **底座** · 自研(Qwen 系架构)
- **定位** · 国内首个金融推理大模型 · 类 GPT-O1 · 思维链 + 过程奖励 + 强化学习
- **核心能力** · 决策与风控 / 宏观-市场-政策多维分析 / 结构化财务数据提取
- **性能** · FinanceIQ 金融评测 10 类(CPA / 银行 / 证券从业等)全面超 GPT-4o 和 Qwen2.5-72B
- **接入难点** · 需 4× A100/H100 并行 · 本地部署成本极高 · Preview 版本

#### 7. [DISC-FinLLM](https://github.com/FudanDISC/DISC-FinLLM) · 复旦大学 DISC Lab

[![GitHub Stars](https://img.shields.io/github/stars/FudanDISC/DISC-FinLLM?style=flat)](https://github.com/FudanDISC/DISC-FinLLM) [![License](https://img.shields.io/badge/License-Apache%202.0-blue)](https://github.com/FudanDISC/DISC-FinLLM/blob/main/LICENSE)

- **机构** · 复旦大学 DISC Lab · **发布** · 2023 年 · **底座** · Baichuan-13B(指令微调)
- **定位** · 中文金融大模型 · 面向国内金融从业者和研究场景
- **核心能力** · 金融咨询(投资/保险/理财)· NLP 情感/NER/分类 · 内嵌财务公式 · RAG 增强
- **性能** · 年报分析 F1 超同期开源模型 · 中文金融知识问答 72%+
- **接入难点** · 底座 Baichuan-13B 版本较老 · 无 O1 式思维链 · 实时行情分析弱

#### 8. [PIXIU / FinMA](https://github.com/The-FinAI/PIXIU) · 武汉大学 & The-FinAI

[![GitHub Stars](https://img.shields.io/github/stars/The-FinAI/PIXIU?style=flat)](https://github.com/The-FinAI/PIXIU) [![License](https://img.shields.io/badge/License-Apache%202.0-blue)](https://github.com/The-FinAI/PIXIU/blob/main/LICENSE)

- **机构** · 武汉大学 & The-FinAI 联合团队 · **发布** · 2023 年 · **底座** · LLaMA(7B/13B/30B)
- **定位** · 综合框架:模型(FinMA)+ 数据(FIT 136K 指令)+ 评测(FLARE)
- **核心能力** · FLARE 9 种金融 NLP 任务学术权威评测 · 情感/NER/股票趋势预测 · 完整微调教程
- **性能** · 金融情感/NER/股票预测 超 BloombergGPT 和 GPT-4(2023 测试)
- **接入难点** · 主要英文 · 中文 A 股场景性能有限 · LLaMA 底座中文弱于 Qwen/GLM

---

## 📊 横向对比总表

| 模型 | 机构 | 发布 | 底座 | 许可证 | 部署成本 | 中文A股 | 推理深度 | API 状态 |
|---|---|---|---|---|---|---|---|---|
| [Fin-R1](https://github.com/SUFE-AIFLM-Lab/Fin-R1) | 上海财经大学 | 2024 | DeepSeek-R1 微调 | Apache 2.0 | 中 (单卡 A100) | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐ | ✅ 已上线 |
| [Kronos](https://github.com/shiyu-coder/Kronos) | 清华大学 | 2025.08 | 自研 4.1M-499M | MIT | 低 (CPU 可跑) | ⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ | ✅ 已上线 |
| [FinGPT](https://github.com/AI4Finance-Foundation/FinGPT) | AI4Finance / 哥大 | 2023 | 多选 LLaMA/GLM/Qwen | MIT | 极低 (单卡 A100 80G) | ⭐⭐⭐ | ⭐⭐ | ✅ 已上线 |
| [CFGPT](https://github.com/TongjiFinLab/CFGPT) | 同济 + 上海AI实验室 | 2023 | InternLM / GLM-4 | Apache 2.0 | 低 (6B 单卡 3090) | ⭐⭐⭐⭐ | ⭐⭐⭐ | ✅ 已上线 |
| [M3](https://github.com/ArthurZhang02/m3-market-microstructure) | 北京中关村学院 | 2026.08 | VQ Tokenizer + Trans | **CC BY-NC 4.0** | 极低 (CPU) | ⭐⭐⭐⭐⭐ | ⭐⭐⭐ | ✅ 已上线 |
| [轩辕 FinX1](https://github.com/Duxiaoman-DI/XuanYuan) | 度小满 | 2024.12 | 自研 Qwen 系 | Apache 2.0 | 高 (4× A100/H100) | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ | ⏳ 策展中 |
| [DISC-FinLLM](https://github.com/FudanDISC/DISC-FinLLM) | 复旦大学 | 2023 | Baichuan-13B | Apache 2.0 | 中 (单卡 A100) | ⭐⭐⭐⭐ | ⭐⭐ | ⏳ 策展中 |
| [PIXIU/FinMA](https://github.com/The-FinAI/PIXIU) | 武汉大学 | 2023 | LLaMA 7B/13B/30B | Apache 2.0 | 低 (7B 单卡 3090) | ⭐⭐⭐ | ⭐⭐⭐ | ⏳ 策展中 |

> 💡 **更完整的对比 + 详细性能/局限说明**,请访问项目主页 [www.agentpit.io/finance-llm-zoo](https://www.agentpit.io/finance-llm-zoo)

---

## 🚀 免费 API 简要接入(可选)

上述 **5 个已上线模型**可通过 AgentPit 免费 API 直接调用,零本地部署成本,适合快速原型验证。

### 3 步接入

```bash
# 1. 注册账号
open https://www.agentpit.io/register

# 2. 申请 API Key
open https://develop.agentpit.io/apply

# 3. 调用示例(以 Fin-R1 为例)
curl -X POST https://develop.agentpit.io/api/v1/open-api/llm \
  -H "Authorization: Bearer YOUR_API_KEY" \
  -H "Content-Type: application/json" \
  -d '{
    "model": "fin-r1",
    "messages": [{"role":"user","content":"分析茅台 2024 年报"}]
  }'
```

### 全部 API 端点

| 模型 | 端点 | 完整文档 |
|---|---|---|
| Fin-R1 | `POST /api/v1/open-api/llm` | [docs](https://develop.agentpit.io/help#llm) |
| Kronos | `POST /api/v1/open-api/kronos` | [docs](https://develop.agentpit.io/help#kpred) |
| FinGPT | `POST /api/v1/open-api/fingpt` | [docs](https://develop.agentpit.io/help#fingpt) |
| CFGPT | `POST /api/v1/open-api/cfgpt` | [docs](https://develop.agentpit.io/help#cfgpt) |
| M3 | `POST /api/v1/open-api/microstructure` | [docs](https://develop.agentpit.io/help#microstructure) |
| Google Search Grounding | `POST /api/v1/open-api/google` | [docs](https://develop.agentpit.io/help#google-search) |

> 📖 **完整的请求/响应参数、curl / Python / Node 示例、错误码 · 见** [develop.agentpit.io/help](https://develop.agentpit.io/help)

### ⚠️ 常见错误码

| HTTP | 含义 | 处理 |
|---|---|---|
| 401 | API Key 无效或已撤销 | 检查 Key 或重新申请 |
| 429 | 超出月度 Token 额度 | 联系管理员提升额度 |
| 502 | 上游模型服务异常 | 稍后重试 |

---

## 🗺️ 路线图

- [x] Google Search Grounding API
- [x] Kronos K 线预测 API(清华 · 支持自定义因子权重)
- [x] Fin-R1 金融大模型 API(上海财经大学 · A 股中文优化 · 链式推理)
- [x] FinGPT 情感分析 API(哥大 AI4Finance · 中英双语)
- [x] CFGPT 中文金融大模型 API(同济 · A 股年报/研报专项)
- [x] M3 市场微观结构模型 API(北京中关村学院 · 订单流生成)
- [ ] 轩辕 XuanYuan FinX1 API(度小满 · GPT-O1 级金融推理)
- [ ] DISC-FinLLM API(复旦 · 金融 RAG 场景)
- [ ] PIXIU / FinMA API(武大 · FLARE 评测框架)
- [ ] BloombergGPT 开源等价物评测对比
- [ ] 中文金融大模型 Benchmark 公开榜单

> ⭐ Star 本仓库,第一时间获取新模型上线通知

---

## 🤝 贡献

**发现好的开源金融模型漏收了?** 欢迎 [开 Issue](https://github.com/agentpit-io/finance-llm-zoo/issues/new) 提名新模型 · 请附:
- GitHub 仓库地址
- 原始论文/技术报告
- 使用的开源许可证
- 你为什么觉得值得收录

我们会评估其开源属性(许可证)、技术定位、上游活跃度后决定是否加入策展。

---

## 📄 License

策展仓库本身采用 **MIT License** · 但**每个收录的模型遵循其原始许可证**(见对比表许可证列)· 使用前请查阅上游仓库。

---

<p align="center">
  由 <a href="https://github.com/agentpit-io">AgentPit</a> 公益维护 ·
  <a href="https://www.agentpit.io/finance-llm-zoo">项目主页</a> ·
  <a href="https://develop.agentpit.io/help">API 完整文档</a> ·
  <a href="https://github.com/hangeaiagent/kronos-free-api">上游研究仓</a>
</p>
