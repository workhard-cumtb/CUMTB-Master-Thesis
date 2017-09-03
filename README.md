# 中国矿业大学（北京）学术型硕士学位论文模板

使用注意事项：
1. 安装TexLive 2016
2. 使用XeLaTeX+bibtex+XeLaTeX+XeLaTeX编译顺序
3. 以管理员身份运行命令行窗口，输入以下命令fc-cache -fv，回车等待字体缓存更新完成。（切记这步非常重要，不然编译tex文件的时间会很长）

测试平台：
windows 8.1 64位


说明：
使用xelatex而不使用pdflatex是为了跨平台而不需要更改源文件，因此本模板在Linux和MacOS上编译都是没有问题的，如有问题欢迎在Issues下面留言。 


模板格式依据来源于[矿大（北京）研究生院官网](http://yjs.cumtb.edu.cn/index.php?m=content&c=index&a=show&catid=89&id=271)


查看本机字体
```bash
fc-list :lang=zh-cn > zh.txt
fc-list :lang=en-us > en.txt
```
