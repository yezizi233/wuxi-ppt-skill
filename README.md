# WuXi BD PPT Playbook Skill

这是一个用于生成和分析 **WuXi AppTec 风格生物医药 BD / 市场理解 PPT** 的 Codex skill。

它的目标不是做通用 PPT 美化，而是把你提供的市场资料、公司资料、投资机构名单、调研笔记、截图、PDF、Excel 等素材，转化成类似 `Singapore Market Understanding Report` 的高密度咨询式 BD deck：有清晰商业问题、章节逻辑、目标筛选、Target Profile、Key Stakeholder、Enabler / VC mapping 和可落地的 BD 切入建议。

## Skill 名称

```text
wuxi-bd-ppt-playbook
```

本地安装路径：

```text
C:\Users\叶子\.codex\skills\wuxi-bd-ppt-playbook
```

GitHub 仓库：

```text
https://github.com/yezizi233/wuxi-ppt-skill
```

## 它能做什么

### 1. 根据素材生成类似风格的 PPT 方案

你给出素材后，它会按照 WuXi 风格的分析方式生成：

- deck 目标和受众判断
- consulting-style storyline
- slide-by-slide blueprint
- 每页标题、结论和页面类型
- 每页应该放什么证据
- 每页适合用什么图表、表格、地图、矩阵或人物页
- Target Profile / Key Stakeholder / Enabler / VC 页面结构
- WuXi 风格视觉规则

默认逻辑框架是：

```text
Executive Summary
-> Country / Market Overview
-> Industry Insights
-> Target Profile
-> Target Enabler / VC
-> Appendix
```

### 2. 分析已有 PPT 或截图

如果你给它一组 PPT 截图、缩略图或 `.pptx` 文件，它会逆向拆解：

- 这套 deck 在回答什么商业问题
- 面向什么受众
- 章节之间如何递进
- 每页在整体叙事中的作用
- 视觉系统如何复用
- 哪些页面模板可以沉淀
- 哪些内容是直接观察，哪些是分析推断

### 3. 生成 BD 可行动的 Target Profile

对公司、机构、VC、enabler 或 venture builder，它会强制整理：

- 机构 / 公司介绍
- 产品、平台或服务方向
- 融资、合作或里程碑时间线
- 核心能力
- 关键人和可能的关系 owner
- WuXi 潜在切入点
- 风险、不确定性和缺失来源
- 后续 BD 动作建议

### 4. 复用 WuXi 风格视觉语言

它会默认使用这一套设计语言：

- 深蓝 / 钴蓝 / 浅青 / 冷灰配色
- 白底高密度内容页
- 深蓝章节封面页
- 顶部 section tab
- 底部 WuXi 品牌条
- 蓝色模块标题栏
- 结论先行标题
- 表格、矩阵、funnel、地图、logo map、stakeholder grid

## 适合输入什么素材

你可以提供：

- 市场研究资料
- 国家或区域产业资料
- 公司列表
- 投资机构名单
- PDF / DOCX / XLSX / CSV
- PPT 截图或现有 `.pptx`
- 公司官网、融资新闻、管线信息、ClinicalTrials.gov 结果
- 手写调研笔记或访谈纪要
- 你已经整理好的 target shortlist

素材越结构化，输出越接近可直接转成 PPT 的状态。

## 如何调用

最稳的方式是直接点名 skill：

```text
使用 wuxi-bd-ppt-playbook。我会给你一批素材，请按照 WuXi Singapore Market Understanding Report 的风格、分析方式和逻辑框架，生成一套类似的 PPT deck。
```

生成新 deck blueprint：

```text
使用 wuxi-bd-ppt-playbook，基于这些资料生成一套 Australia biopharma market understanding report 的 slide-by-slide blueprint，用于 BD target landscaping。
```

分析已有截图：

```text
使用 wuxi-bd-ppt-playbook，分析这个 PPT 截图文件夹，提炼设计风格、章节逻辑、页面模板和可复用 playbook。
```

生成 Target Profile：

```text
使用 wuxi-bd-ppt-playbook，把这些公司资料整理成 WuXi 风格的 Target Profile + Key Stakeholder 页面方案。
```

如果要实际生成 `.pptx` 文件：

```text
使用 wuxi-bd-ppt-playbook 先设计完整 storyline 和 slide-by-slide blueprint，然后结合 pptx skill 生成 .pptx 文件。
```

## 推荐工作流

1. **给素材**

   提供市场资料、公司资料、投资机构名单、截图、表格或调研笔记。

2. **先生成 blueprint**

   让 skill 输出完整 storyline 和 slide-by-slide blueprint，确认逻辑是否正确。

3. **补证据**

   根据它列出的 evidence gaps 补充来源，尤其是市场规模、融资、管线、关键人、合作关系等硬事实。

4. **生成 PPT**

   如果需要文件，继续要求它结合 `pptx` skill 生成 `.pptx`。

5. **审阅与迭代**

   检查每页是否有明确结论、证据、BD 意义和视觉模板；不确定内容必须保留标记。

## 输出通常长什么样

分析模式通常输出：

- Deck Goal And Audience
- Chapter Logic
- Page Role Table
- Visual System
- Reusable Page Templates
- Evidence And Confidence Gaps
- Reusable Playbook

生成模式通常输出：

- Deck Objective
- Storyline
- Slide-By-Slide Blueprint
- Evidence Input Requirements
- Target Profile Template
- Stakeholder Mapping Template
- Visual Rules
- Open Data Gaps And Assumptions

## 证据纪律

这个 skill 会严格区分：

- `观察`：素材里直接能看到的信息
- `推断`：基于素材做出的分析判断
- `低置信度`：截图不清、来源不足、不能硬写的部分

它不会把模糊截图里的文字强行补全成事实，也不会凭空编造市场规模、融资金额、管线进度、关键人身份或合作关系。

## 目录结构

```text
wuxi-bd-ppt-playbook/
├─ SKILL.md
├─ README.md
├─ evals/
│  └─ evals.json
└─ references/
   ├─ style-guide.md
   ├─ storyline-blueprint.md
   ├─ page-templates.md
   └─ singapore-screenshot-observations.md
```

## 注意事项

- 这个 skill 本身负责分析、规划和生成 deck blueprint。
- 如果要读写真实 `.pptx` 文件，需要同时使用 `pptx` skill。
- 如果要查证市场、公司、临床或融资事实，需要额外做来源检索。
- 当前内置的 Singapore 截图观察只作为风格和逻辑参考，不是公司事实来源。
- 如果当前会话没有自动触发，直接写 `使用 wuxi-bd-ppt-playbook` 即可。
