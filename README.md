# ORACLE · 八字认知系统

> 不是改变你，是还原你。

**Live Demo → [gabriellewoo.github.io/oracle-bazi](https://gabriellewoo.github.io/oracle-bazi/)**

---

## 这是什么

ORACLE 是一个基于八字的**认知图谱生成工具**。

它不算命，不预测，不给你贴标签。它做一件事：用你的出生时间（四柱八字）作为输入，通过大语言模型，生成你天生的认知操作系统分析——你怎么处理信息、在哪里做错决定、什么东西在消耗你、你在什么状态下最像自己。

---

## 五维分析框架

| # | 模块 | 说明 |
|---|------|------|
| 01 | **天然优势** | 不需要培养就已拥有的能力 |
| 02 | **决策盲区** | 容易失去判断力的结构性偏差 |
| 03 | **能量泄露** | 持续消耗你的人、环境、行为 |
| 04 | **最优形态** | 产出最高、最像自己的状态 |
| 05 | **对自己的禁令** | 根据命盘结构，绝对不要对自己做的事 |

---

## 如何使用

**1. 准备 API Key**

支持 DeepSeek（推荐，便宜）或 OpenAI：
- DeepSeek：[platform.deepseek.com](https://platform.deepseek.com) → API Keys → 创建
- OpenAI：[platform.openai.com](https://platform.openai.com) → API Keys → 创建

**2. 查询自己的八字**

搜索「生辰八字在线排盘」，输入出生年月日和时辰，得到四柱八字（8个汉字）。

时辰对照：子(23-1点) 丑(1-3) 寅(3-5) 卯(5-7) 辰(7-9) 巳(9-11) 午(11-13) 未(13-15) 申(15-17) 酉(17-19) 戌(19-21) 亥(21-23)

**3. 打开页面，配置，分析**

填入 API Key → 选择四柱八字 → 填性别和关注方向 → 启动分析

分析结果可导出为 `.md` 文件，或继续追问 ORACLE。

---

## 技术说明

- **纯前端单文件**，无后端，无数据库，无服务器
- API Key 仅保存在浏览器 `localStorage`，不经过任何第三方
- 所有 AI 调用直接从浏览器发往 DeepSeek / OpenAI
- 支持流式输出（Streaming）
- 支持对话追问（带完整上下文）

---

## 本地运行

直接下载 `index.html`，双击在浏览器打开即可。无需安装任何依赖。

```bash
git clone https://github.com/GabrielleWoo/oracle-bazi.git
# 然后双击 index.html
```

---

## License

MIT — 可自由 fork、部署、修改。
