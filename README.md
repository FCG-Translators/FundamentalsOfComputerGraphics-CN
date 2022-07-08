# FundamentalsOfComputerGraphics-CN

计算机图形学基础（中文译本）

<img src="src/img/cover.png" style="zoom:100%;" />

## Introduction - 介绍

本仓库是《计算机图形学基础（第五版）》的中文翻译，支持mdbook和xelatex两种格式。

## Installation - 安装
###  dependence - 依赖
  - mdbook
```bash
# 从源码构建mdbook工具
cargo install mdbook
# 从源码构建最新版mdbook工具
cargo install --git https://github.com/rust-lang/mdBook.git mdbook
# mac系统使用homebrew安装mdbook工具
brew install mdbook
# Arch linux使用pacman包管理器安装mdbook工具
pacman -S mdbook
```
  - tex
```bash
# TeX Live安装
wget -c https://mirrors.tuna.tsinghua.edu.cn/CTAN/systems/texlive/Images/texlive2022-20220321.iso
# windows
# 1）解压iso文件
# 2）进入解压目录
./install-tl-windows.bat # 也可双击运行该批处理文件
# linux
mount ./texlive2022-20220321.iso /mnt
cd /mnt
perl install-tl # 或者./install-tl -gui

# MacTEX安装
# macOS
wget -c https://mirror.ctan.org/systems/mac/mactex/MacTeX.pkg
# 双击运行MacTeX.pkg
```
### repository - 存储库
```bash
# 克隆存储库
git@github.com:zouyonghe/FundamentalsOfComputerGraphics-CN.git
# 进入目录
cd FundamentalsOfComputerGraphics-CN
```

## Usage - 用法
- mdbook
```bash
# 在浏览器中打开图书
mdbook serve --open

# 构建图书
mdbook build
```
- xelatex
```bash
# 进入tex目录
cd tex
# 编译pdf图书
xelatex FundamentalsComputerGraphics.tex
```
## Changelog - 更新日志

## FAQ - 常见问题

### 如何参与本书翻译？

因本书翻译工作量巨大，希望志同道合者共同参与。
若您希望贡献，请首先fork本仓库，并在Issues中提出想要翻译的章节，翻译完成后发起PR，经审核后可合入主线。

### 发现书籍谬误，如何提出？

请fork本仓库，对谬误部分进行订正，然后发起PR，经审核后可合入主线。
参见“联系”，向译者提出修改意见。

## Support - 支持

如需获取其他帮助，请在Issues提出问题，也可参照“联系”，获取帮助。

### Dos - 文档

[mdBook Documentation](https://rust-lang.github.io/mdBook/)

### Contact - 联系

🍮buding
QQ：1259085392
EMAIL：1259085392z@gmail.com

## Authors and acknowledgment - 贡献者和感谢

感谢 [Steve Marschner](https://www.cs.cornell.edu/\~srm/)和[Peter Shirley](https://www.petershirley.com/)以及其他贡献者共同参与编写完成《计算机图形学基础》这部图形学巨著。
