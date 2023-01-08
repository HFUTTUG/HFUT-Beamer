# 合肥工业大学 Beamer 主题集合

![visitors](https://visitor-badge.glitch.me/badge?page_id=HFUTTUG.Beamer)

本项目是在前人的基础上编写的展示用 Beamer 主题集合。目前提供以下几种主题，你可以点击PDF链接查看更细致的结果：

| 主题名称             | 作者                            | 封面截图                                     | 内页截图                                     | PDF                          |
| ---------------- | ---------------------------------- | ---------------------------------------- | ---------------------------------------- | ---------------------------------------- |
| `hfut-CambridgeUS` | [nauta](https://github.com/nautaa) | ![hfut-CambridgeUS-front](https://github.com/HFUTTUG/HFUT-Beamer/raw/images/hfut-CambridgeUS-front.png) | ![hfut-CambridgeUS-inner](https://github.com/HFUTTUG/HFUT-Beamer/raw/images/hfut-CambridgeUS-inner.png) | [🔗](https://github.com/HFUTTUG/HFUT-Beamer/raw/images/hfut-CambridgeUS.pdf) |
| [`hfut-sx`](https://github.com/sxhfut/Beamer-HFUT) | [孙晓](https://github.com/sxhfut/)   | ![hfut-front](https://github.com/HFUTTUG/HFUT-Beamer/raw/images/hfut-sx-front.png) | ![hfut-inner](https://github.com/HFUTTUG/HFUT-Beamer/raw/images/hfut-sx-inner.png) | [🔗](https://github.com/HFUTTUG/HFUT-Beamer/raw/images/hfut-sx.pdf) |
| [`hfut-BinChen`](https://github.com/HFUT-BinChen/HFUT-Beamer) | [陈斌](https://github.com/HFUT-BinChen) | ![hfut-BinChen-front](https://github.com/HFUTTUG/HFUT-Beamer/raw/images/hfut-BinChen-front.png) | ![hfut-BinChen-inner](https://github.com/HFUTTUG/HFUT-Beamer/raw/images/hfut-BinChen-inner.png) | [🔗](https://github.com/HFUTTUG/HFUT-Beamer/raw/images/hfut-BinChen.pdf) |

我们建议在你使用模板前，先看看`example.tex`提供的样例指导。这样遇到一些问题也比较好寻找解决方案。

可以在`example.tex`中的`\usetheme{...}`中填入主题名进行调整主题的调整。默认采用16:9比例，可以删除`\documentclass[aspectratio=169]{beamer}`中的`[aspectratio=169]`切换回4:3比例。

对于 Beamer 的中文缩进和段间距问题，可使用以下的代码片段进行修正。建议仅在需要的地方使用，不要直接作用于全局。

```latex
\setlength{\parskip}{6pt}
\setlength{\parindent}{2em}
```

## 编译指南

我们可以用`latexmk -xelatex -shell-escape example`命令编译示例文档。当然使用vscode也可以直接编译，我们也提供了针对LaTeX Workshop扩展的[配置文件](https://github.com/HFUTTUG/HFUT-Beamer/blob/master/.vscode/settings.json)。

> 注意：我们在样例文件中使用了`minted`宏包，这个宏包需要在编译时附上`-shell-escape`选项，并且需要安装Python和[Pygments](https://pygments.org/)。如果你不需要在你的文档中打印代码，或是希望使用`listings`宏包，那么请移除在示例文档中所有用到`minted`宏包的部分（`mintinline`命令，或者是`minted`环境）。

## 更多资料

- [Beamer 用户手册](https://github.com/latexstudio/LaTeXPackages-CN/raw/master/beamer/beamer%E7%94%A8%E6%88%B7%E6%89%8B%E5%86%8C%EF%BC%88V3.24%EF%BC%89%E4%B8%AD%E8%AF%91%E7%89%88.pdf)
- [LaTeX 新手入门指南](https://github.com/HFUTTUG/HFUT_Thesis/wiki/新手指南)
- [参与开发](https://github.com/HFUTTUG/HFUT_Thesis/wiki/参与开发)

## 写在后面

- 鸣谢上面引用的3个项目，没有它们就没有我们这个合集。
- 有意加入[@HFUTTUG](https://github.com/HFUTTUG)的同学可发送[📧Email](mailto:hfuttug@163.com)
- 编译错误？请在这里新建一个issue。或者欢迎加入我们的QQ群（904943223）进行讨论。

## TODO
- hfut-beamer-setup.tex/.sty：考虑到每个人的beamer设置习惯不一样（有无导航符号等），需要提供一个setup文件方便进行设置

- 模块化的颜色（color）、内部（inner）、外部（outer）和字体（font）主题

    - 最好是多个主题之间能够共享