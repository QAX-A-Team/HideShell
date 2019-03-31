# HideShell
A JSP backdoor that enables under Tomcat hiding arbitrary JSP files, in addition to their access logs. JSPs hidden by hideshell.jsp remain accessbile **until the next reboot of Tomcat instance**.

## Environments tested
- Tomcat 7
- Tomcat 8

## How it works?

- [Tomcat 源代码调试笔记 - 看不见的 Shell](https://mp.weixin.qq.com/s/x4pxmeqC1DvRi9AdxZ-0Lw)

- [Tomcat 源代码调试 - 看不见的 Shell 第二式之隐藏任意 Jsp 文件](https://mp.weixin.qq.com/s/1ZiLD396088TxiW_dUOFsQ)

- [Tomcat 源代码调试 - 看不见的 Shell 第二式增强之无痕](https://mp.weixin.qq.com/s/7b3Fyu_K6ZRgKlp6RkdYoA)

## TL;DR   
Hideshell.jsp hides JSP files by simplying deleting them, while persuading Tomcat into believing that files are still there, thus serving them as usual.
