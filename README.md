# 合肥工业大学 Beamer 主题集合

本项目是在前人的基础上编写的展示用 Beamer 主题集合。目前提供以下几种主题：

| 主题名称             | 作者                            | 封面截图                                     | 内页截图                                     |
| ---------------- | ---------------------------------- | ---------------------------------------- | ---------------------------------------- |
| `CambridgeUS-hfut` | [nauta](https://github.com/nautaa) | ![CambridgeUS-hfut-front](https://github.com/HFUTTUG/HFUT-Beamer/blob/images/CambridgeUS-hfut-front.png) | ![CambridgeUS-hfut-inner](https://github.com/HFUTTUG/HFUT-Beamer/blob/images/CambridgeUS-hfut-inner.png) |
| [`hfut-sx`](https://github.com/sxhfut/Beamer-HFUT) | [孙晓](https://github.com/sxhfut/)   | ![hfut-front](https://github.com/HFUTTUG/HFUT-Beamer/blob/images/hfut-sx-front.png) | ![hfut-inner](https://github.com/HFUTTUG/HFUT-Beamer/blob/images/hfut-sx-inner.png) |
| [`hfut-BinChen`](https://github.com/HFUT-BinChen/HFUT-Beamer) | [陈斌](https://github.com/HFUT-BinChen) | ![hfut-BinChen-front](https://github.com/HFUTTUG/HFUT-Beamer/blob/images/hfut-BinChen-front.png) | ![hfut-BinChen-inner](https://github.com/HFUTTUG/HFUT-Beamer/blob/images/hfut-BinChen-inner.png) |

可以在`example.tex`中的`\usetheme{...}`中填入主题名进行调整主题的调整。默认采用16:9比例，可以删除`\documentclass[aspectratio=169]{beamer}`中的`[aspectratio=169]`切换回4:3比例。

对于 Beamer 的中文缩进和段间距问题，可使用以下的代码片段进行修正。建议仅在需要的地方使用，不要直接作用于全局。

```latex
\setlength{\parskip}{6pt}
\setlength{\parindent}{2em}
```

## 更多资料

- [Beamer 用户手册](https://github.com/latexstudio/LaTeXPackages-CN/raw/master/beamer/beamer%E7%94%A8%E6%88%B7%E6%89%8B%E5%86%8C%EF%BC%88V3.24%EF%BC%89%E4%B8%AD%E8%AF%91%E7%89%88.pdf)

## TODO
- hfut-beamer-setup.tex/.sty：考虑到每个人的beamer设置习惯不一样（有无导航符号等），需要提供一个setup文件方便进行设置
- 字体的配置：一些系统没有微软雅黑等适合幻灯片的字体。
- 模块化的颜色主题