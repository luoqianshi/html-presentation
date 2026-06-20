# Purple Gold Presentation 预览卡

此小文件仅用于标题页预览。生成最终 deck 时，请阅读下面列出的完整设计文档。

## 文件

- 完整设计文档：`themes/purple-gold-presentation/design.md`
- 预览卡：`themes/purple-gold-presentation/preview.md`

## 选择元数据

- Slug: `purple-gold-presentation`
- Tagline: 继承 Blue Professional 的宽松视频友好布局，切换为 Purple Gold 的近黑画布、紫色标题与金色强调。
- Mood: dark, cinematic, professional, modern, tutorial
- Tone: confident, clear, polished, modern
- Formality: medium-high
- Density: medium
- Scheme: dark
- Best for: 需要暗色电影感外观同时保持 Blue Professional 宽松低密度布局的视频友好幻灯片。适合教程、知识讲解、投资者更新和知识分享类 deck，紫色承担结构，金色承担强调。
- Avoid for: 需要明亮/playful 配色、 heavy 渐变、企业蓝或彩虹强调的场景。也不适合浅色背景或紧凑信息密集型布局。

## 视觉快照

Purple Gold Presentation 继承了 Blue Professional 低密度、视频友好的布局系统，并将其包裹在近黑电影感配色中。紫色（`#b98eff`）承担结构——标题、分隔线、徽章、流程标记。金色（`#ffc402`）承担强调——关键词、高亮、结论。最终结果是一套在视频录制中依然清晰可读的暗色、自信 deck。

## 预览要素

- Palette:
  - bg: #08090d
  - bg_cover: #070609
  - primary: #b98eff
  - accent_gold: #ffc402
  - text: #f6f2e8
  - text-muted: #aaa59a
  - text-light: #746f66
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
