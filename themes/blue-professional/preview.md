# Blue Professional 预览卡

此小文件仅用于标题页预览。生成最终 deck 时，请阅读下面列出的完整设计文档。

## 文件

- 完整设计文档：`themes/blue-professional/design.md`
- 预览卡：`themes/blue-professional/preview.md`

## 选择元数据

- Slug: `blue-professional`
- Tagline: 奶油色纸张背景搭配电光钴蓝强调，干净现代的专业风格。
- Mood: professional, modern, calm, trustworthy
- Tone: clean, considered, polished, neutral
- Formality: medium-high
- Density: medium
- Scheme: light
- Best for: 适合需要现代、克制且略带权威感的场景：B2B SaaS 产品演示、咨询交付物、顾问更新、投资者报告。也是希望显得专业但不死板的干净选择。
- Avoid for: 不适合需要热烈、 playful 或刻意非正式氛围的场景，冷峻的电光蓝克制感会显得过于 polished。

## 视觉快照

Blue Professional 是一套**咨询级演示系统**，适用于高管简报、研究交付物和季度回顾。其基础视觉前提是**克制但有一个强烈的承诺**：温暖的奶油色画布（`{colors.bg}` — `#fdfae7`）和单一的饱和钴蓝（`{colors.primary}` — `#1e2bfa`），承担每一个强调、指标、行动号召、眉标和图表填充。没有第二品牌色，没有粉彩调色板，没有冷暖配对——只有奶油色、钴蓝色和用于正文的中性灰阶。

## 预览要素

- Palette:
  - bg: #fdfae7
  - primary: #1e2bfa
  - text: #111111
  - text-muted: #6b6b6b
  - text-light: #9a9a9a
  - positive: #059669
  - negative: #dc2626
- Typography: Space Grotesk 标题 + Inter 正文（精确字号见完整设计文档）
- Signature move: 见完整设计文档中的标志性布局、质感与装饰词汇。

## 国际化 / CJK 预览注意事项

- 如果预览使用中文或其他 CJK 文字，保持 CJK 字间距为 0，放宽行高，避免对 CJK 文本使用 uppercase 变换。
- 选定后使用完整 `design.md` 的 CJK 章节获取精确字体配对与脚本特定调整。

## 预览规则

- 在固定舞台模型内精确构建一张 1920x1080 的标题页。
- 保留完整设计文档中描述的配色、字体角色、表面节奏和装饰词汇。
- 使用用户的真实标题/副标题/场景；不要复制演示 slide 内容。
- 渲染出的预览必须像真实的第一页，而不是模板选择卡。
- 切勿在 slide 上放置内部工作流文字：不要出现 `preview`、`generated from`、`preview.md`、`template`、`preset`、`style option`、`Option A/B/C`、文件名、路径或源文档标签。
- 切勿在 slide 上放置模板名称或 slug；仅在聊天消息中提及。
- 除非用户明确要求这些词出现在 deck 中，否则不要放置用户需求注释，如期望氛围、受众或内部使用标签。
- 可见 chrome 仅使用真实 deck 内容：deck 标题、真实章节标题、日期、作者、公司、页码，或用户材料中的真实内容短语。
- 不要读取 `template.html` 用于预览生成。
- 不要读取其他模板的 `design.md` 文件。
- 用户选择此模板生成完整 deck 后，先阅读完整设计文档再生成最终幻灯片。
