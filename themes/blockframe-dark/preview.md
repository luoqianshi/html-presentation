# BlockFrame Dark 预览卡

此小文件仅用于标题页预览。生成最终 deck 时，请阅读下面列出的完整设计文档。

## 文件

- 完整设计文档：`themes/blockframe-dark/design.md`
- 预览卡：`themes/blockframe-dark/preview.md`

## 选择元数据

- Slug: `blockframe-dark`
- Tagline: BlockFrame 的夜间模式：纯黑画布 + 白色粗边框 + 糖果色荧光光晕，视频友好的高对比粗野主义风格。
- Mood: bold, playful, graphic, dark, cinematic
- Tone: confident, graphic, pop, design-led
- Formality: medium-low
- Density: medium
- Scheme: dark
- Best for: 需要强烈图形感和设计主导气质的暗色内容：创意机构提案、独立产品发布、品牌重塑、设计评审、现代教程、视频分镜。高对比配色在视频压缩后依然清晰。
- Avoid for: 需要明亮、柔和或传统权威感的场景（正式商务汇报、监管披露、浅色品牌展示）。

## 视觉快照

BlockFrame Dark 是 BlockFrame 的夜间版本，建立在五条铁律之上：每个区域都有 4px 白色实线边框、每个浮起元素都有 8px 白色硬偏移阴影、每个角都是直角、每个强调色都是高饱和糖果 pastel、每个布局都可以故意歪一点。与日间版不同，全页背景限定为近黑色 `#0a0a0a`，卡片使用深灰 `#141414`，粉、浅蓝、绿、黄仅作为标签、图标、卡片和小装饰色，并带有柔和光晕。系统额外增加了 10vw 水平内边距，确保视频导出时平台 UI 不会遮挡内容。

## 预览要素

- Palette:
  - black: #0a0a0a
  - card: #141414
  - white: #f6f6f6
  - muted: #a0a0a0
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
