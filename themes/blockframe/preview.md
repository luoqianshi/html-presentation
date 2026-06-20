# BlockFrame 预览卡

此小文件仅用于标题页预览。生成最终 deck 时，请阅读下面列出的完整设计文档。

## 文件

- 完整设计文档：`themes/blockframe/design.md`
- 预览卡：`themes/blockframe/preview.md`

## 选择元数据

- Slug: `blockframe`
- Tagline: 新粗野主义糖果色块 + 4px 粗黑边框 + 硬偏移阴影，高能量设计导向风格。
- Mood: bold, playful, graphic, fresh, confident
- Tone: confident, graphic, pop, design-led
- Formality: medium-low
- Density: medium
- Scheme: light
- Best for: 需要强烈图形感和设计主导气质的内容：创意机构提案、独立产品发布、品牌重塑、设计评审、现代教程。也适合希望用活泼视觉打破传统金融科技/研究内容的场景。
- Avoid for: 需要安静、克制、传统权威感的场景（监管披露、正式法律文件、极简商务汇报）。

## 视觉快照

BlockFrame 是一套**新粗野主义演示系统**，建立在五条铁律之上：每个区域都有 4px 黑色实线边框、每个浮起元素都有 8px 黑色硬偏移阴影、每个角都是直角、每个强调色都是高饱和糖果 pastel、每个布局都可以故意歪一点。系统的乐趣来自这些规则的碰撞——带边框的卡片撞上带边框的卡片、阴影叠着阴影、倾斜装饰故意刺破网格。全页背景限定为奶油色 `#FFDC8B`、米白色 `#FFFDF5` 与结束页黑色；粉、浅蓝、绿、黄仅作为标签、图标、图表和小装饰色。

## 预览要素

- Palette:
  - black: #000000
  - white: #FFFFFF
  - offwhite: #FFFDF5
  - pink: #FE90E8
  - blue: #C0F7FE
  - green: #99E885
  - yellow: #F7CB46
  - cream: #FFDC8B
- Typography: Inter 标题/正文 + Space Grotesk 标签/计数器；中文回退 Noto Sans SC（精确字号见完整设计文档）
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
