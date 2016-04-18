The Not So Short Introduction To LaTeX (中文版 lshort)
===

编译要求
---
将发行版内的 ctex 宏包、xeCJK 宏包更新到最新，并确认 lshort-zh-cn-style.sty 引用的宏包都已正确安装并更新到最新。

lshort 中文版使用 Fandol 宏包作为中文字体。fontspec 会对此字体报 script-not-exist 的警告，可以忽视。

编译方式
---
在 src 目录下按照以下顺序编译：
```
xelatex lshort-zh-cn
makeindex lshort-zh-cn
xelatex lshort-zh-cn
```
如果编译正确生成 PDF，之后将 PDF 移动到根目录。

Windows 下已在 src 目录提供 bat 脚本，Linux 下提供了用于 GNU Make 工具的 Makefile（未验证）。