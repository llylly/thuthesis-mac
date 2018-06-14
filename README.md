## ThuThesis for Mac

*By llylly*

Enable ThuThesis to typeset bachelor thesis in right format in MacOS.

让ThuThesis在Mac上排版出符合格式要求的毕设论文.

## 环境要求

安装这些字体:

- SimSun #宋体
- SimHei #黑体
- LiSu #Mac上的隶书

## 使用方法

先安装[ThuThesis](https://github.com/xueruini/thuthesis). 再用这个仓库中的文件替换.

## 修改之处

+ **[6.1 initial]**thuthesis.cls中, 用要求的win环境字体, 替代了默认的mac字体. 使用自动加粗设置.
+ **[6.1 initial]**figures中, 放入了从毕设通知中扒下来的声明和授权页, 并设置生成的时候使用这些页.
  + **[6.15 update]**发现直接使用声明页有个严肃的问题, 就是页码对不上... 因此改为直接生成. 扫描件的正确使用方式应为答辩完签完字后再把那个扫描件放过来.
+ **[6.15 update]**在main.tex中加入了``\usepackage[resetfonts]{cmap}``用于建立中文字体的映射, 这样就可以复制汉字出来了.
+ **[6.15 update]**在main.tex使用multibib宏包和appena环境将外文综述/翻译的参考文献独立编号. 在附录A中使用\citeappena, \bibliographyappena, \bibliographystyleappena系列命令即可使用之.
+ **[6.15 update]**在main.tex中引入lstlisting宏包, 并加入了网上扒下来的一段YAML高亮定义. 如果需要用到YAML代码, 有了它就可以自动提供酷炫的高亮支持了.
+ **[6.15 update]**加入了.latexmkrc文件, 该文件加入了一项latexmk的配置, 使得仿宋字体也会被嵌入PDF文件. 不然仿宋体文字在win的Adobe Reader中打开会乱码.
+ **[6.15 update]**删除了之前不小心加入的.aux文件.



*最后更新: 2018年6月15日*

