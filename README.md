# 🧠 Humanizer-zh — 中文AI文本去AI味优化 Skill

[![Version](https://img.shields.io/badge/version-1.1.0-blue)](https://github.com/wxie0815-arch/humanizer-zh)
[![OpenClaw](https://img.shields.io/badge/OpenClaw-Compatible-green)](https://openclaw.ai)
[![License](https://img.shields.io/badge/license-MIT-orange)](LICENSE)

> 针对中文语境，基于24条核心人性化原则，去除AI生成文本的"AI味"，使其更自然、更像人类写作。专为加密货币内容优化。

## 🎯 功能概述

`humanizer-zh` 是三阶段专业写作流程的**第三阶段**，负责将 `copywriting` 生成的文章初稿进行深度优化，去除AI生成文本的机械感，使其读起来更自然、更有个性。

```
writing-plans  →  copywriting  →  humanizer-zh
   (规划阶段)       (撰写阶段)      (优化阶段)
```

## ✨ 核心特性

- **24条人性化原则**：基于 `humanizer` skill 的核心原则，针对中文语境深度适配
- **五大问题专项处理**：过度书面语、车轱辘话、缺乏情感、翻译腔、滥用排比
- **加密内容专项规则**：保留 `$BTC`、TVL、DeFi 等专业术语，避免过度炒作词汇
- **风格一致性**：在去AI味的同时，保持用户的个人写作风格
- **智能判断**：根据文章类型（快讯/深度/KOL）调整优化力度

## 🚀 快速开始

### 安装

```bash
gh repo clone wxie0815-arch/humanizer-zh
```

### 在 binance-square-oracle 中使用

`humanizer-zh` 已内置于 [binance-square-oracle](https://github.com/wxie0815-arch/binance-square-oracle) 预言机中，通过三阶段写作流程自动调用。

### 独立使用

```python
from writing_skill import WritingSkill

skill = WritingSkill()
final_article = skill.humanize(
    draft="此外，值得注意的是，$BTC的价格走势呈现出明显的上升趋势...",
    style_fingerprint="用户历史写作风格（可选）"
)
print(final_article)
```

## 📋 优化效果对比

| 维度 | 优化前（AI味） | 优化后（人味） |
|------|--------------|--------------|
| 连接词 | "此外，值得注意的是..." | 直接陈述或自然过渡 |
| 情感 | 中立、客观 | 有观点、有态度 |
| 句式 | 长句堆砌 | 长短句交替 |
| 词汇 | 书面语、学术腔 | 口语化、接地气 |
| 结尾 | "综上所述..." | 行动引导或思考方向 |

## 🔗 相关 Skill

| Skill | 说明 | 仓库 |
|-------|------|------|
| `writing-plans` | 生成结构化写作计划 | [wxie0815-arch/writing-plans](https://github.com/wxie0815-arch/writing-plans) |
| `copywriting` | 根据写作计划撰写文案初稿 | [wxie0815-arch/copywriting](https://github.com/wxie0815-arch/copywriting) |
| `binance-square-oracle` | 集成三阶段写作的完整预言机 | [wxie0815-arch/binance-square-oracle](https://github.com/wxie0815-arch/binance-square-oracle) |

## 📄 许可证

MIT License — 自由使用、修改和分发。

---

## 💰 赞助支持

如果这个项目对您有帮助，欢迎赞助支持！

**BSC（BEP-20）钱包地址：**
 

支持 USDT / BNB / 任意 BEP-20 代币。感谢每一位支持者 🙏

**作者：** 无邪Infinity | 币安广场 [@wuxie](https://www.binance.com/en/square/profile/wuxie) | X [@wuxie149](https://x.com/wuxie149)
