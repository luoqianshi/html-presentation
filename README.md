# HTML Presentation · 视频友好版

一套专为**视频演示**优化的 HTML 幻灯片工具。适合 B 站讲解视频、知识分享、教程分镜、investor update 等需要把幻灯片导出为高清 PNG/视频帧的场景。

> 📺 **视频教程**：[本项目使用教程](https://www.bilibili.com/video/BV1HToiBCEwg)

与原项目相比，本版本更强调：

- **字号更大**：标题与正文整体放大，远距离/小屏幕都清晰可读。
- **信息密度更低**：每页一个重点，避免信息过载。
- **左右大留白**：`10vw` 边距，避免被平台字幕、头像、按钮遮挡。
- **高对比配色**：深黑背景 + 紫色/黄色强调，视频压缩后依然清晰。
- **单文件输出**：所有 CSS、JS 内联，复制一个 HTML 即可开始制作。

## 快速开始

### 1. 创建演示文稿

复制基础模板：

```bash
cp templates/presentation.html my-presentation.html
```

用浏览器直接打开 `my-presentation.html`，按页面注释添加 `<section class="slide">...</section>` 内容即可。

### 2. 导出 PNG 分镜

安装依赖：

```bash
pip install -r requirements.txt
playwright install chromium
```

导出幻灯片图片：

```bash
python screenshot_html_slides.py themes/blue-professional/template.html -o slides_out
```

输出为 `slides_out/page_1.png`、`slides_out/page_2.png`...，分辨率 1920×1080，可直接拖入剪辑软件。

## 目录结构

```
html-presentation-video/
├── README.md                          # 本文件
├── SKIL.md                            # 视频友好设计规范
├── requirements.txt                   # Python 依赖
├── .gitignore                         # Git 忽略配置
├── screenshot_html_slides.py          # 截图导出 1920×1080 PNG
├── templates/
│   └── presentation.html              # 基础模板（复制起点）
├── themes/                            # 完整主题库
│   ├── blue-professional/             # 蓝/米白专业风
│   ├── purple-gold-presentation/      # 紫/金暗色电影感
│   ├── index.json                     # 主题索引
│   ├── README.md                      # 主题库说明
│   ├── AGENTS.md                      # Agent 使用手册
│   └── scripts/                       # 主题库脚本
├── frontend-slides/                   # 原始 Skill/插件文档（精简）
│   ├── README.md
│   ├── SKILL.md
│   ├── STYLE_PRESETS.md
│   ├── animation-patterns.md
│   ├── html-template.md
│   └── viewport-base.css
```

## 视频友好设计要点

1. **单页单点**：每页只讲一件事，标题即结论。
2. **字体够大**：标题最小 34px（4vw），正文最小 17px（1.7vw）。
3. **左右留白**：默认 `padding: 6vh 10vw`，留出安全边距。
4. **主体放大**：`.content-wrapper` 默认 `transform: scale(1.45)`，让核心内容占据画面主要区域。
5. **少装饰**：无噪点纹理、无大面积发光、无渐变文字，避免视频压缩后出现脏边。
6. **控件自动隐藏**：截图脚本会自动隐藏翻页控件、进度条和右侧圆点，只保留干净画面。

## 截图脚本常用参数

| 参数 | 说明 | 默认值 |
|------|------|--------|
| `-o, --output-dir` | 输出目录 | `slides_out` |
| `--prefix` | 文件名前缀 | `page` |
| `--mode` | 截图模式：`standard` / `balanced` / `compact` / `auto` | `standard` |
| `--device-scale` | 设备像素比 | `2` |
| `--content-scale` | 额外页面缩放 | `1.0` |
| `--wait` | 初始加载等待（毫秒） | `1000` |

## 技术规范

- 每页 slide 使用 `<section class="slide">...</section>`。
- 当前激活 slide 使用 `.active` class，翻页只操作 class。
- 所有样式与脚本内联，不依赖外部资源。
- 详细规范见 `SKIL.md`。

## 致谢与来源

本项目是在 **Zara Zhang** 开源项目的基础上进行改编和二次开发：

- [frontend-slides](https://github.com/zarazhangrui/frontend-slides) — Claude Code 插件/Skill，提供 Slide Engine、动画模式与模板选择框架。
- [beautiful-html-templates](https://github.com/zarazhangrui/beautiful-html-templates) — 可复用的 HTML 幻灯片模板库，包含 `blue-professional`、`purple-gold-presentation` 等主题。

感谢原作者的出色工作。原项目采用 MIT License，本改编版本同样遵循 MIT License。

详细致谢与来源声明见 [`NOTICE.md`](./NOTICE.md)，完整许可证文本见 [`LICENSE`](./LICENSE)。

## 与原项目的区别

本目录是从原 `html-presentation` 整理出的**上传专用版本**，在原作者工作的基础上做了以下调整：

- **视频友好化改造**：整体放大字号、降低信息密度、增加左右留白、提升对比度，删除噪点纹理，更适合视频压缩场景。
- **精简结构**：删除 `.git/`、`__pycache__/`、生成日志、截图缓存等冗余文件；删除具体项目输出（如 `vibecoding-ep03/`、`口播稿.md`）。
- **精简主题库**：保留最适用于视频演示的 `blockframe`、`blue-professional` 和 `purple-gold-presentation`，并更新了索引与说明文档。
- **改进截图脚本**：自动隐藏更多模板自带的导航控件，导出画面更干净。

## License

MIT
