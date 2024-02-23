# FundamentalsOfComputerGraphics-CN

<div align=center>

<img src="src/img/cover.png" style="zoom:100%;" />

**《计算机图形学基础（第五版）》（中文译本）**

</div>

## Introduction - 介绍

本仓库包含《计算机图形学基础（第五版）》的中文翻译，译文以 mdBook 生成的网页和 XeLaTeX 生成的 PDF 文件两种形式提供，网页内容更新进度可能会落后于 PDF 文件。

## Build - 构建

### Install dependence - 安装依赖

* 安装 mdBook
  ```bash
  # 从源码构建 mdBook 工具
  cargo install mdbook
  # 从源码构建最新版 mdBook 工具
  cargo install --git https://github.com/rust-lang/mdBook.git mdbook
  # Mac 系统使用 homebrew 安装 mdBook 工具
  brew install mdbook
  # Arch linux使用 pacman 包管理器安装 mdBook 工具
  pacman -S mdbook
  ```

* 安装 TeX
  ```bash
  # TeX Live 安装
  wget -c https://mirrors.tuna.tsinghua.edu.cn/CTAN/systems/texlive/Images/texlive2023-20230313.iso
  # Windows
  # 1）解压 iso 文件
  # 2）进入解压目录
  ./install-tl-windows.bat # 也可双击运行该批处理文件
  # linux
  mount ./texlive2023-20230313.iso /mnt
  cd /mnt
  perl install-tl # 或者./install-tl -gui
  
  # MacTEX 安装
  # MacOS
  wget -c https://mirror.ctan.org/systems/mac/mactex/MacTeX.pkg
  # 双击运行MacTeX.pkg
  ```

### Clone repository - 克隆存储库

```bash
# 克隆存储库
git clone git@github.com:zouyonghe/FundamentalsOfComputerGraphics-CN.git
# 进入目录
cd FundamentalsOfComputerGraphics-CN
```

### Usage - 用法

* 使用 mdBook
  ```bash
  # 在浏览器中打开图书
  mdbook serve --open
  # 或者运行根目录下的 tex-run.bat 文件（Windows）
  
  # 构建图书
  mdbook build
  # 或者运行根目录下的 tex-build.bat 文件（Windows）
  ```
* 使用 XeLaTeX
    ```bash
    # 进入 ./tex 目录    
    cd tex
    # 编译 PDF 文件
    xelatex FundamentalsComputerGraphics.tex
    ```

## Translation Specification - 翻译规范

* 善用、多用 Google、Wikipedia、剑桥在线词典和牛津在线词典来确定中英文单词、术语的翻译
* 中文写作规范请参考 [中文技术文档写作风格指南](https://zh-style-guide.readthedocs.io/zh-cn/latest/)
* 术语的翻译请统一遵循以下格式
  ```LaTeX
  % 没有耳熟能详的缩写
  齐次坐标（\textit{homogeneous coordinate}）
  % 有广为人知的缩写
  应用程序接口（\textit{API, application program interface}）
  ```
* 首字母缩写的翻译请统一遵循以下格式
  ```LaTeX
  KISS（“保持简单、愚蠢”，\textit{"keep it simple, stupid"}）
  ```
* 原书中所有的边栏备注请使用 `note` 环境
  ```LaTeX
  \begin{note}
  % 具体内容
  \end{note}
  ```
* 需要补充“译注”的地方请使用 `\footnote[]{}`
* 原书中 "such as..." 引导的成分以及其他举例子、解释说明成分请放到（）中
  ```LaTeX
  原文：A key part of any graphics program is to have good classes 
  or routines for geometric entities such as vectors and matrices, 
  as well as graphics entities such as RGB colors and images.
  译文：所有图形程序的一个关键部分是为几何实体（如向量和矩阵）以及图形实体
  （如RGB颜色和图像）提供良好的类或例程。
  % 放在括号中的内容往往是可以翻译成“例如……”、“比如……”、“也就是说……”等形式的内容
  ```
* 根据句意对原文标点进行适当修改，比如把句号替换成逗号来避免独立句子过多、把句号替换成分号来连接两个关系紧密的句子等等。

## Changelog - 更新日志

<div align=center>

|    章节    | 开始时间  | 结束时间  |  状态  |  译者  | 校对者 |
| :--------: | :-------: | :-------: | :----: | :----: | :----: |
|   第一章   | 2022.7.5  | 2022.7.10 | 已完成 | buding |Hugo HU|
|   第二章   | 2022.7.11 |     -     | 进行中 | buding, Hugo HU |Hugo HU|
|   第三章   | 2022.8.17 |   2022.8.30  | 已完成 |Hugo HU|Hugo HU|
|   第四章   | 2022.8.31 |     -     | 进行中 | Hugo HU|        |
|   第五章   |     -     |     -     | 未开始 |   -    |        |
|   第六章   |  2023.1.9 |     -     | 进行中 | 二之花 |        |
|   第七章   |     -     |     -     | 未开始 |   -    |        |
|   第八章   |     -     |     -     | 未开始 |   -    |        |
|   第九章   |     -     |     -     | 未开始 |   -    |        |
|   第十章   |     -     |     -     | 未开始 |   -    |        |
|  第十一章  |     -     |     -     | 未开始 |   -    |        |
|  第十二章  |     -     |     -     | 未开始 |   -    |        |
|  第十三章  |     -     |     -     | 未开始 |   -    |        |
|  第十四章  |     -     |     -     | 未开始 |   -    |        |
|  第十五章  |     -     |     -     | 未开始 |   -    |        |
|  第十六章  |     -     |     -     | 未开始 |   -    |        |
|  第十七章  |     -     |     -     | 未开始 |   -    |        |
|  第十八章  |     -     |     -     | 未开始 |   -    |        |
|  第十九章  |     -     |     -     | 未开始 |   -    |        |
|  第二十章  |     -     |     -     | 未开始 |   -    |        |
| 第二十一章 |     -     |     -     | 未开始 |   -    |        |
| 第二十二章 |     -     |     -     | 未开始 |   -    |        |
| 第二十三章 |     -     |     -     | 未开始 |   -    |        |

</div>

## FAQ - 常见问题

### 如何参与本书翻译？

因本书翻译工作量巨大，希望志同道合者共同参与。

尚需如下角色成员：
- 翻译：完成书籍各章节翻译工作，优先在 LaTeX 文件中更新译文内容并同步至 Markdown 文件；
- 校对：完成书籍各章节校对工作，从表述、排版等方面对译文进行审阅；
- 推广（待定）。

若您希望贡献，请首先fork本仓库，并在Issues中提出想要翻译的章节，请认真、耐心地进行翻译，力求用词准确、通俗易懂，并且文档格式符合标准，翻译完成后请发起PR，经审核后可合入主线，您的名字也将进入本书的译者列表。

### 发现书籍谬误，如何提出？

因为译者水平有限，在翻译的过程中出现疏漏、错误、语义不明等情况在所难免，如果在阅读的过程中遇到上述情况，烦请读者悉心指出，帮助译者订正。

- 请fork本仓库，对谬误部分进行订正，然后发起PR，经审核后可合入主线。
- 参见“联系”，向译者提出修改意见。

## Support - 支持

如需获取其他帮助，请在Issues提出问题，也可参照“联系”，获取帮助。

### Dos - 文档

[mdBook Documentation](https://rust-lang.github.io/mdBook/)

[计算机图形学基础（第五版）](https://www.routledge.com/Fundamentals-of-Computer-Graphics/Marschner-Shirley/p/book/9780367505035)

### Contact - 联系

🍮buding 

QQ：1259085392 

EMAIL：1259085392z@gmail.com 

QQ群：584041033（进群验证：计算机图形学基础）

## Authors and acknowledgment - 贡献者和感谢

感谢 [Steve Marschner](https://www.cs.cornell.edu/\~srm/) 和 [Peter Shirley](https://www.petershirley.com/) 以及其他贡献者共同参与编写完成《计算机图形学基础》这部图形学巨著。

# Declaration of responsibility - 责任声明

本项目遵守美国版权法规定，作者 Steve Marschner 和 Peter Shirley 具有本书的著作权。本项目目的在于面向中文（华语）用户推广和普及计算机图形学知识，仅供计算机图形学相关专业者及爱好者学习和交流使用。本项目为公益项目，不曾也不将以任何盈利形式进行盈利。同时，因译者水平有限，译本可能存在歧义、错误乃至误导性内容，烦请读者认真思考、谨慎鉴别，并希望读者能在发现书籍谬误时及时通过“联系”方式向译者进行反馈。
