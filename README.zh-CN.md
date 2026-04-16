<div align="center">

# hkust-beamer-template

**一个非官方、社区维护的 HKUST 风格 Beamer 模板，适合学术汇报与课程展示。**

<p>
  <a href="LICENSE"><img alt="MIT License" src="https://img.shields.io/badge/license-MIT-blue.svg"></a>
  <img alt="LaTeX" src="https://img.shields.io/badge/LaTeX-Beamer-0f4c81.svg">
  <img alt="Engine" src="https://img.shields.io/badge/engine-XeLaTeX-7b3f00.svg">
  <img alt="Format" src="https://img.shields.io/badge/format-16:9-2f6b73.svg">
  <img alt="Status" src="https://img.shields.io/badge/status-unofficial-lightgrey.svg">
</p>

<p>
  适合作为 thesis talk、组会、课程报告和研究汇报的轻量级起点。
</p>

<p>
  <a href="README.md">English</a>
</p>

</div>

---

## 预览

**[查看示例 PDF](docs/previews/hkust-beamer-template-preview.pdf)**

<sub>下面的截图都可以点击查看高清原图。</sub>

<p align="center">
  <a href="docs/previews/hkust-beamer-template-preview.pdf">
    <img src="docs/previews/title-hero.png" alt="标题页预览" width="100%">
  </a>
</p>

<p align="center">
  <a href="docs/previews/content-slide.png">
    <img src="docs/previews/content-slide.png" alt="内容页预览" width="49%">
  </a>
  <a href="docs/previews/table-slide.png">
    <img src="docs/previews/table-slide.png" alt="表格页预览" width="49%">
  </a>
</p>

## 这个模板适合做什么？

这个仓库提供了一个开箱即用的 Beamer 主题，采用 HKUST 风格的视觉设计，省去每次做汇报都从空白幻灯片开始的麻烦。

它的目标是：

- **上手快** —— clone 下来，改几个字段就能编译；
- **默认干净** —— 页眉页脚平衡、配色克制、16:9 版式宽松；
- **容易改** —— 示例 deck 很小，结构清楚，便于继续扩展。

## 功能特点

- HKUST 风格的蓝 / 金配色
- 适合现代投影和屏幕的 16:9 Beamer 布局
- 顶部带 section 进度点的导航栏
- 单行页脚，包含作者、标题和页码
- 内置示例 deck：`slide.tex`
- 如果本机没有 Arial，会自动回退到 `TeX Gyre Heros`

## 快速开始

### 1）克隆仓库

```bash
git clone https://github.com/Liu-KM/hkust-beamer-template.git
cd hkust-beamer-template
```

### 2）编译示例 deck

```bash
xelatex -interaction=nonstopmode slide.tex
xelatex -interaction=nonstopmode slide.tex
```

### 3）修改 `slide.tex` 中的元信息

主要改这些字段：

- `\author{...}`
- `\institute{...}`
- `\title{...}`
- `\subtitle{...}`
- `\date{...}`

然后把示例页面替换成你自己的内容即可。

## 项目结构

```text
.
├── HKUST_Beamer.sty      # 主题定义
├── slide.tex             # 示例 deck
├── pic/                  # 模板依赖的视觉素材
├── docs/previews/        # README 截图 + 示例 PDF
├── DISCLAIMER.md         # HKUST 相关素材的使用说明
├── LICENSE               # 本仓库代码/文档的 MIT 许可证
├── README.md             # 英文版说明
└── README.zh-CN.md       # 中文版说明
```

## 自定义建议

- 最简单的方式是直接复制 `slide.tex` 里的示例页面，保持整体风格统一。
- 占位图页可以替换成你自己的 plot、系统图或实验图。
- 标题、副标题、日期、院系信息都集中在一处修改，不需要四处同步。
- 如果你想调整颜色系统或导航栏样式，可以从 `HKUST_Beamer.sty` 开始改。

## 品牌说明

> 这个仓库**不是** HKUST 官方项目。
> 它只是一个受 HKUST 汇报风格启发的社区模板。

仓库中包含的 HKUST 相关视觉素材，仅用于让模板能够直接使用。这些名称、标识和 logo **不** 随本仓库的 MIT 许可证一起授权。

在复用或再分发这些素材前，请先阅读 [DISCLAIMER.md](DISCLAIMER.md)。

HKUST 官方相关页面：

- Brand Assets Unit: <https://brand.hkust.edu.hk/>
- Official Marks or Logos: <https://brand.hkust.edu.hk/hkust-marks>
- University policy / guidelines entry: <https://dst.hkust.edu.hk/support-%26-resources//university-policies-%26-guidelines>

## 许可证

本仓库中由维护者编写的 LaTeX 代码、主题代码和说明文档，采用 [MIT License](LICENSE) 发布。

HKUST 的名称、标识、logo 及其他官方品牌素材仍归 HKUST 所有，除非 HKUST 另有明确说明，否则不包含在该许可证内。
