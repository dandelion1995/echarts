# 02/bar.html;
### Echarts.init()
初始化 Echarts实例
setOption 用指定数据绘图

### Option对象
+ 标题： title
+ 图例： legend
+ X轴： xAxis
+ 数据： series:
		- Name
		- type
		- data

# 02/line.html
在bar的基础上添加series数据，把type改成line即可

# 03/title.html
title.html标题负责显示整个图表的标题
+ Text: 标题文字
+ SubText： 子标题
+  Left,top，right,bottom 标题位置
+  borderColor： 边框颜色
+  borderWidth:  边框宽度

在官网的文档，配置项手册可查看所有配置属性

#  03/toolbox.html 组件的工具栏
+ show： 是否显示
+ Feature: 具体显示的功能
+ saveAsImage: 保存图片
+ Restore: 还原
+ dataView: 数据视图
+ dataZoom: 缩放视图
+ magicType: 动态类型切换

# 03/ tooltip.html 组件的工具栏
+ show: 是否显示
+ Trigger: 触发方式，axis就是x轴出发 

# 03/mark.html
### 标记线： markline
+ 标记线的添加
+ 最大值，平均值，最小值的标记线

### 标记点： markpoint
+ 标记点的添加
+ 最大值，平均值，最小值的标记点
+ 任意位置的标记点
+ symbol:    ECharts 提供的标记类型包括 'circle', 'rect', 'roundRect', 'triangle', 'diamond', 'pin', 'arrow', 'none'

# 饼图
### 04/pie.html
+ 饼图展示数据的特点
	- 展示百分比
	- Type是pie
+ Center是圆心坐标
+ Radius半径
+ Name图例名字
+ selectedModel是否支持多选

# 仪表图
+ 仪表图展示数据的特点
	- type是gauge
+ 动态修改仪表图数据
~~~
  //动态修改仪表图数据
        setInterval(function(){
            //使用随机数生成data
            option.series[0].data[0].value = (Math.random() * 100).toFixed(2)- 0;
            
            myChart.setOption(option,true);
        },2000)
~~~

# 地图、雷达图、散点图

# 可视化组件的使用

##	多个坐标系配合
	+ 两个图标合并展示
	+ 设置两个y轴
	+ 配置多个yaxis属性
~~~
	   yAxisIndex: 1, //默认只想第一个y轴，指定指向第2个y轴数据
~~~
## dataZoom组件
## 值域漫游



# Echarts扩展知识
## 模块化
	webpack中使用
	
## 异步获取数据绘图






