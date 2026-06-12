# ZGCA Beamer Template (中关村学院 LaTeX Beamer 模板)

这是一个为**中关村学院 (Zhongguancun Academy, ZGCA)** 定制的 LaTeX Beamer 幻灯片模板。本模板基于 [UCAS Beamer](https://github.com/wzl-plasmid/ucas-beamer) 及 [SINTEF Presentation](https://www.overleaf.com/latex/templates/sintef-presentation/jhbhdffczpnx) 衍生修改，专门适配了中关村学院与中关村人工智能研究院的联合视觉识别系统。

---

## 🌟 模板特色

* **色彩契合**：使用中关村学院标准蓝色（`#0363c9`）作为主题色，区块、高亮等要素的颜色与之协调搭配。
* **联合标识**：集成中关村学院与中关村人工智能研究院的联合双 Logo（提供蓝/白两色版本），支持在封面、内页页眉以及致谢页中优雅呈现。
* **大楼背景**：封面与章节页提取并裁剪自学院 C5 教学大楼实景，且图片经过极致无损压缩（仅 ~1MB），在保证超高清质量的同时让编译出的 PDF 更加轻量。
* **对齐优化**：页眉标题与左侧的纸飞机小图标（`logo_icon`）实现了精准的纵向居中对齐，右上角 Logo 的可读性也进行了放大优化。
* **丰富版式**：
  * 标准内容页（支持列表逐步淡入、公式、图表排版）
  * 优雅的卡片块设计（`block` 与 `colorblock`）
  * 实用的侧图混排版式（`sidepic` 环境）
  * 明亮的过渡章节页（`chapter` 环境）
  * 干净大气的封面与致谢页（自动隐藏页码，防止重叠）

---

## 🛠️ 编译与使用指南

### 1. 前置要求
* 推荐安装完整的 TeX 发行版（如 **TeX Live** 或 **MiKTeX**）。
* 编译必须使用 **XeLaTeX**（以支持 CJK 中文及特殊字体的渲染）。

### 2. 编译命令
在项目根目录下，运行以下命令（建议运行两次以确保目录与交叉引用更新正确）：

```bash
xelatex zgca-beamer-sample.tex
xelatex zgca-beamer-sample.tex
```

### 3. 项目结构说明

* `zgca-beamer-sample.tex`：模板的使用演示源文件，包含各种排版版式的实例。
* `zgca-beamer-sample.pdf`：编译生成的高清幻灯片样例。
* `beamerthemezgca.sty`：中关村学院 Beamer 主题定制样式包。
* `zgcacolor.sty`：中关村学院标准色定义文件。
* `assets/`：核心视觉资产目录。
  * `background.png`：封面大楼实景高清背景图（16:9）。
  * `background_negative.png`：过渡章节实色明亮背景图。
  * `logo_RGB.png` / `logo_RGB_negative.png`：蓝/白联合双 Logo 标识。
  * `logo_icon.png` / `logo_icon_negative.png`：蓝/白纸飞机小图标。

---

## 🤝 致谢

本模板的开发参考了 [UCAS Beamer](https://github.com/wzl-plasmid/ucas-beamer) 及 [SINTEF Beamer Theme](https://www.overleaf.com/latex/templates/sintef-presentation/jhbhdffczpnx)，感谢原作者的开源贡献。
