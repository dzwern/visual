python绘图工具汇总

（1）matplotlib

官方网站:https://matplotlib.org/

matplotlib是一个python的2D绘图库，它以各种硬拷贝格式和跨平台的交互式环境生成出版质量级别的图形，通过matplotlib，可以绘制折线图，散点图，柱形图，饼图，直方图，子图等等， matplot使用numpy进行数组运算，并调用一系列其他的python库来实现硬件交互

pylab是matplotlib面向对象绘图库的一个接口，语法和matlab十分相似，可以使用matlab对应的命令

绘图简介

使用matplotlib库绘制图形，大致需要以下5个步骤 （1）创建一个图纸（figure） （2）在图纸上创建一个或者多个绘图(plotting)区域 （3）在plotting区域上描绘点，线等 （4）在plotting添加修饰标签 （5）添加其他diy进行修饰

方法	含义
matplotlib.pyplot.angle_spectrum	绘制电子波谱图
matplotlib.pyplot.bar	绘制柱状图
matplotlib.pyplot.barh	绘制直方图
matplotlib.pyplot.broken_barh	绘制水平直方图
matplotlib.pyplot.contour	绘制等高线图
matplotlib.pyplot.errorbar	绘制误差线
matplotlib.pyplot.hexbin	绘制六边形图案
matplotlib.pyplot.hist	绘制柱形图
matplotlib.pyplot.hist2d	绘制水平柱形图
matplotlib.pyplot.imshow	图像绘图
matplotlib.pyplot.pie	绘制饼形图
matplotlib.pyplot.quiver	绘制量场图
matplotlib.pyplot.scatter	绘制散点图
matplotlib.pyplot.specgram	绘制光谱图
matplotlib.pyplot.subplot	绘制子图
（2）plotly

官方网站：

https://plotly.com/
plotly是一个强大的开源可视化框架，它通过构建基于浏览器显示的Web形式的可交互图表来展示信息，可以创建多种精美图形和地图，

plotly是一个基于d3.js开发的一个js的库，可以提供js，python，R等使用，

其中plotly中绘制图像有在线和离线两种方式，一般常用的是离线的方式，离线绘图有分为plotly.offline.plot()和plotly.offline.iplot()两种方式，前者是以离线的方式在当前工作目录下生成html格式的图像文件，并自动打开，后者是在jupyter notebook中专用的方法

（3）seaborn

官方网站：

http://seaborn.pydata.org/
seaborn是基于matplotlib的图形可视化python包，它提供了一种高度交互式界面

seaborn是在matplotlib的基础上进行更高级的API封装，从而使得作图更加容易，同时它能兼容numpy与pandas数据结构以及scipy与statsmodels等统计模式

header 1	header 2
scatterplot	散点图
lineplot	线图
replot	关系图
stripplot	分布散点图
boxplot	箱型图
violineplot	小提琴图
swarmplot	分布密度散点图
barplot	条形图
countplot	计数图
piontplot	点图
displot	直方图
kdeplot	核密度图
jointplot	联合分布图
pairplot	变量关系组图
heatmap	热力图
clustermap	聚类图
（4）pycharts

官方网址：

https://pyecharts.org/#/zh-cn/basic_charts
echarts是百度开源的数据可视化，而pycharts是基于python的数据可视化

特性： （1）简介的API设计，支持链式调用

（2）囊括了30+种常见图表，应有尽有

（3）支持主流Notebook 环境，Jupyter Notebook 和JupyterLab

（4）可轻松集成至Flask, Django等主流Web框架

（5）高度灵活的配置项，可轻松搭配出精美的图表

（6）详细的文档和示例，帮助开发者更快的上手项目

（7）多达400+地图文件以及原生的百度地图，为地理数据可视化提供强有力的支持

（5）Altair

官方网站：

https://altair-viz.github.io/
Altair是python的一个公认的统计可视化库，API简单，友好，一致，并建立在强大的交互图形语法上，Altair API不包含实际的可视化呈现代码，而是按照交互图形语法规范发出的JSON数据结构，由此产生的数据可以在用户界面中呈现，这种优雅简单行产生了漂亮且有效的可视化效果，且只需要很少的代码就可以实现结果

数据源为DataFrame格式，它是由不同的数据类型的列组成，DataFrame是一种整洁的格式，其中的行与样本相对应，而列与观察到的变量相对应，数据通过数据转换映射到使用组的视觉属性（位置，颜色，大小，形状，面板等）

（6）Bokeh 官方网站：

https://bokeh.org/
Bokeh是一个python交互可视化库，支持Web浏览器展示（图标可以输出为json对象，HTML文档或者可交互的网络应用）它提供风格优雅、简洁的D3.js的 图形化样式，并将此功能扩展到高性能交互的数据集，数据流上，使用Bokeh可以快速便捷地创建交互式绘图，仪表板和数据应用程序等

https://hub.gke.mybinder.org/user/bokeh-bokeh-notebooks-jlb2c34b/notebooks/tutorial/00 - Introduction and Setup.ipynb

（7）Holoviews

官方网站：

http://holoviews.org/
Holoviews是一个具有交互功能的可视化工具，并且对于网络的要求没有plotly和pyecharts那么的高。可以用非常少的代码就可以完成数据分析的可视化展示，它将matplotlib和Bokeh结合了起来

优点：超快捷构建交互 opts配置：瞬间变美 加号和乘号

（8）Folium

官方网站：

https://www.osgeo.cn/folium/
Folium建立在python生态系统的数据打包优势和leaflet.js类库之上，可以在python中操作数据，然后通过folium在leaflet地图上可视化表达

folium 可以轻松地在交互式leaflet地图上可视化Python中操作的数据。它既允许将数据绑定到choropleth 可视化的地图，也允许将丰富的 vector/raster/HTML 可视化作为地图上的标记。

该库具有许多来自 OpenStreetMap、Mapbox 和 Stamen 的内置分站机, 并支持带有 Mapbox 或云制作 API 密钥的自定义分站机。 folium 支持图像、视频、GeoJSON 和 TopoJSON 覆盖。

（9）geoplotlib 地图类

官方网站：

https://andrea-cuttone.github.io/geoplotlib/api.html
geolpotlib是python的一个用于地理数据可视化和绘制地图的工具箱，并提供了一个原始和所有可视化之间的基本接口，支持在纯python中开发硬件加速的交互式可视化，并提供点映射，内核密度估计，空间图，泰森多边形图，形状文件和许多更常见的空间可视化的实现，除了为常用的地理数据可视化提供内置的可视化功能之外，geoplotlib还允许通过定义定制层来定义复杂的数据可视化，创建动画

（10）ggplot

官方网站：

http://ggplot.yhathq.com/
ggplot是一个基于R的ggplot2的图形语法的python的绘图系统，实现了更少的代码绘制更专业的图形，

它使用一个高级且富有表现力的API来实现线，点灯元素的添加，颜色的更改等不同类型的可视化组件的组合或添加，而不需要重复使用相同的代码，然而这对那些试图进行高度定制的的来说，ggplot并不是最好的选择，尽管它也可以制作一些非常复杂、好看的图形。 ggplot与pandas紧密联系。如果你打算使用ggplot，最好将数据保存在DataFrames中。

（11）Gleam

官方网站：

https://github.com/dgrtwo/gleam
Gleam 借用了R中 Shiny 的灵感。 它允许你只利用 Python 程序将你的分析变成可交互的网络应用，你不需要会用HTML CSS 或者 JaveScript。Gleam 可以使用任何一种 Python 的可视化库。当你创建一个图表的时候，你可以在上面加上一个域，这样用户可以用它来对数据排序和过滤了。

（12）leather

官方网站：

https://leather.readthedocs.io/en/latest/examples.html
leather是一种可读且用户界面友好的API，适用于现在就需要图标并且对图表是不是完美并不在乎的人，它可以使用所有的数据类型，最终生成SVG图像，

（13）mayavi2

官方网站：

http://code.enthought.com/pages/mayavi-project.html
Mayavi2是一个通用的、跨平台的三维科学数据可视化工具。可以在二维和三维空间中显示标量、向量和张量数据。可通过自定义源、模块和数据过滤器轻松扩展。Mayavi2也可以作为一个绘图引擎，生成matplotlib或gnuplot脚本，也可以作为其他应用程序的交互式可视化的库，将生成的图片嵌入到其他应用程序中。

（14）missingno

官方网站：

https://github.com/ResidentMario/missingno
没有高质量的数据，就没有高质量的数据挖掘结果，当我们做监督学习算法，难免会碰到混乱的数据集，缺失的值，当缺失比例很小时，可直接对缺失记录进行舍弃或进行手工处理，missingno提供了一个小型的灵活的、易于使用的数据可视化和实用工具集，用图像的方式让你能够快速评估数据缺失的情况，而不是在数据表里面步履维艰。你可以根据数据的完整度对数据进行排序或过滤，或者根据热度图或树状图来考虑对数据进行修正。 missingno 是基于matplotlib建造的一个模块，所以它出图速度很快，并且能够灵活的处理pandas数据

（15）mpld3

官方网站：

mpld3基于python的graphing library和D3js，汇集了matplotlib流行的项目的javascript库，用于创建web交互式数据可视化，通过一个简单的API，将matplotlib图形导出为HTML代码，这些HTML代码可以在浏览器中使用

（16）NetworkX

NetworkX 是一个python包，用于创建、操纵和研究复杂网络的结构，以及学习复杂网络结构，功能及其动力学

NetworkX提供了适合各种数据结构的图表，二合字母和多重图，还有大量标准的图算法，网络结构和分析措施，可以产生随机网络，合成网络或经典网络，且节点可以是文本，图像，XML记录等，并提供了一些示例数据

NetworkX测试的代码覆盖率超过90%，是一个多样化，易于教学，能够快速生成图形的python平台

（17）pygal

pygal是一种开放标准的矢量图形语言，它基于XML，可以生产多个输出格式的高分辨率Web图形页面，还支持给定数据的HTML表导出，用户可以直接用代码来描绘图像，可以用任何文字处理工具打开SVG图像，通过改变部分代码来使图像具有交互功能，并且插入到HTML中通过浏览器来观看

（18）pyQtGragh

pyQtGragh是在PyQt4和numpy的基础上构建纯python的GUI图形库，它主要用于数学，科学，工程领域，尽管PyQtGragh完全是在python中编写的，但它本身就是一个非常有能力的图形系统，可以进行大量的数据处理，数学运算，使用了Qt的GraghicsView框架优化和简化了工作流程，实现以最少的工作量完成数据可视化，且速度也非常的快

（19）python-igragh

python界面的igragh高性能图形库，主要针对复杂的网络研究和分析

（20）vincent

Vincent是一个很酷的可视化工具，它以python数据结构作为数据源，然后把它翻译成Vega可视化语法，并且能够在d3js上运行，这让你可以使用python脚本来创建漂亮的3D图形来展示你的数据，Vincent底层使用pandas和dataframe数据，并且支持大量的图表，条形图，线图，散点图，热力图等等。

（21）vispy

vispy是一个高性能的交互式2D/3D的数据可视化库，利用图形处理器GPU通过OpenGL库来显示非常大的数据集

包括： （1）支持数百万点阵的高质量交互科学图表 （2）实时的数据可视化展示 （3）3D模型的快速交互可视化 （4）OPenGL可视化演示 （6）快速可伸缩的可视化部件