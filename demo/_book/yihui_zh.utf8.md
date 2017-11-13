--- 
title: "R bookdownplus"
author: "Peng Zhao"
date: "2017-11-13"
output:
  bookdown::pdf_book:
    keep_tex: yes
    dev: "cairo_pdf"
    latex_engine: xelatex
    citation_package: natbib
    template: tex/template_yihui_zh.tex
    pandoc_args: --chapters
    toc_depth: 3
    toc_unnumbered: no
    toc_appendix: yes
    quote_footer: ["\\begin{flushright}", "\\end{flushright}"]
documentclass: ctexbook
bibliography: [bib/bib.bib]
biblio-style: apalike
link-citations: yes
colorlinks: no
lot: yes
lof: yes
geometry: [b5paper, tmargin=2.5cm, bmargin=2.5cm, lmargin=3.5cm, rmargin=2.5cm]
site: bookdown::bookdown_site
description: "一个简单的中文书示例。"
github-repo: yihui/bookdown-chinese
#cover-image: images/cover.jpg
---

　　

\mainmatter

<!--chapter:end:index.Rmd-->


# 前言 {-}

你好，世界。我写了一本书。这本书是这样的，第 \@ref(intro) 章介绍了啥啥，然后是啥啥……

我用了两个 R 包编译这本书，分别是 **knitr**\index{knitr} [@xie2015] 和 **bookdown**\index{bookdown} [@R-bookdown]。以下是我的 R 进程信息：


```r
sessionInfo()
```

```
## R version 3.4.2 (2017-09-28)
## Platform: x86_64-w64-mingw32/x64 (64-bit)
## Running under: Windows >= 8 x64 (build 9200)
## 
## Matrix products: default
## 
## locale:
## [1] LC_COLLATE=Chinese (Simplified)_China.936 
## [2] LC_CTYPE=Chinese (Simplified)_China.936   
## [3] LC_MONETARY=Chinese (Simplified)_China.936
## [4] LC_NUMERIC=C                              
## [5] LC_TIME=Chinese (Simplified)_China.936    
## 
## attached base packages:
## [1] stats     graphics  grDevices utils     datasets  methods   base     
## 
## other attached packages:
## [1] bookdownplus_1.3.2
## 
## loaded via a namespace (and not attached):
##  [1] compiler_3.4.2  backports_1.1.1 magrittr_1.5    bookdown_0.5   
##  [5] rprojroot_1.2   htmltools_0.3.6 tools_3.4.2     rstudioapi_0.7 
##  [9] yaml_2.1.14     Rcpp_0.12.13    stringi_1.1.5   rmarkdown_1.6  
## [13] knitr_1.17      stringr_1.2.0   digest_0.6.12   evaluate_0.10.1
```

## 致谢 {-}

非常感谢谁谁以及谁谁对我的帮助。艾玛，要不是他们神一样的队友，我两年前就写完这本书了。

\BeginKnitrBlock{flushright}<p class="flushright">张三  
于 A 村某角落</p>\EndKnitrBlock{flushright}

# 作者简介 {#author .unnumbered}

上不了厅堂，下得了厨房。敲得了代码，逮得住蟑螂。

`\mainmatter`

# 牛刀小试 {#intro}

现在我们可以试试 **bookdown** 的一些初级功能了，例如图表。图 \@ref(fig:hello) 是一幅无趣的散点图，表 \@ref(tab:iris) 是一份枯燥的数据。


```r
par(mar = c(4, 4, 1, .1))
plot(cars, pch = 19)
```

\begin{figure}
\includegraphics[width=0.9\linewidth]{yihui_zh_files/figure-latex/hello-1} \caption{雷猴啊，散点图！}(\#fig:hello)
\end{figure}


```r
knitr::kable(
  head(iris), caption = '雷猴啊，iris 数据！',
  booktabs = TRUE
)
```

\begin{table}

\caption{(\#tab:iris)雷猴啊，iris 数据！}
\centering
\begin{tabular}[t]{rrrrl}
\toprule
Sepal.Length & Sepal.Width & Petal.Length & Petal.Width & Species\\
\midrule
5.1 & 3.5 & 1.4 & 0.2 & setosa\\
4.9 & 3.0 & 1.4 & 0.2 & setosa\\
4.7 & 3.2 & 1.3 & 0.2 & setosa\\
4.6 & 3.1 & 1.5 & 0.2 & setosa\\
5.0 & 3.6 & 1.4 & 0.2 & setosa\\
5.4 & 3.9 & 1.7 & 0.4 & setosa\\
\bottomrule
\end{tabular}
\end{table}

就这样，你可以一直编下去，直到编不下去。

\cleardoublepage 

# (APPENDIX) 附录 {-}

# 余音绕梁 {#sound}

呐，到这里朕的书差不多写完了，但还有几句话要交待，所以开个附录，再啰嗦几句，各位客官稍安勿躁、扶稳坐好。



<!--chapter:end:body.Rmd-->

