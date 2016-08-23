用Rmarkdown制作PDF时（需要安装CTEX套件，完全安装），如果里面有中文字符，在生成PDF的时候经常会出错。因此常有一些几种方式处理：
 
（1）将.rmd文件生成md，然后用pandoc生成PDF
（2）用Rstudio生成html，在用chrome浏览器打开，通过打印方式，生成PDF
 
以上两种都很麻烦，很喜欢Rstudio里面直接knitr pdf的感觉。
 
感谢高光银童鞋发现以下的新方法，可以在某种程度上方面操作
 
具体内容如下：
 
1.需要安装Rstudio的最新版本
2.安装rticles包
library(devtools)
devtools::install_github("rstudio/rticles")
 
3.新建rmarkdown文件-From Template--Ctex Document
 
这里的ctex模版是文章模版，如果需要presentation格式，需要自己修改下latex模版。
