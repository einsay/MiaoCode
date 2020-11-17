![](https://s3.ax1x.com/2020/11/17/DERSdH.png)
## 编程环境
0. python自带的编程环境 IDLE
1. 新建python文件：NEW FILE（记住这个单词）
2. 代码的缩进，比如我们的if 条件语句下面的四个空格都是代码缩进，直接点击键盘上tab键也可以
3. 代码注释：(1)单行代码注释: # (2)多行代码注释:每一行前面加上# 或者使用'''代码块'''
4. 程序运行: 会显示>>>
5. 文件保存: 结尾是.py(python的缩写)
6. 文件退出：exit()
## Turtle库
```python
import turtle  # 导入画图工具

# t = turtle.Pen()  # 修改画笔的名字，可以不修改
turtle.shape("turtle")#改变形状
turtle.screensize(400, 300, "yellow")  # 设置画布的长宽和背景颜色
turtle.pencolor("red")#修改画笔颜色
turtle.pensize(5)#设置画笔的粗细

turtle.forward(100)#前进100
# turtle.forward(-100)#后退100
turtle.left(90)#左转90
# turtle.left(-90)#右转90
turtle.right(90)#右转90
# turtle.right(-90)#左转90

#填充颜色，后填充的颜色会覆盖之前填充的颜色
turtle.fillcolor("green")#设置填充颜色
turtle.begin_fill()#开始填充
#绘制图形
turtle.end_fill()#结束填充

#抬笔放笔，up()  goto()  down()
turtle.penup()#抬起画笔，这个时候如果移动画笔的话不会留下痕迹的，因为画笔在天上
turtle.goto(100,100)#去到指定的坐标(x,y)
turtle.pendown()#放下画笔，画笔落地移动的时候才能留下痕迹  

#画圆形
turtle.dot(100,"red")#直径为100的红色实心圆
turtle.circle(100)#半径为100的空心圆
turtle.circle(100,90)#角度为90的圆弧
turtle.circle(100,steps=4)#不会画圆形！！！！只会画出圆形的内切多边形！！！重点

#没讲过的知识，重点复习
turtle.speed(0)#修改画笔的速度1-10逐渐增大，10和0是最大的
turtle.clear()#把当前窗口的所有图形全部清除，但是画笔的位置不会变
turtle.reset()#初始化画布，全部成了一开始啥也没有的样子
turtle.color("red", "yellow")#同时设置画笔颜色和填充颜色
turtle.hideturtle()#隐藏画笔形状
turtle.setheading(90)#turtle.seth(90)
turtle.stamp()#复制当前图形


turtle.done()  # 防止画布关闭

```python
#输入输出(input输入的是字符串)
#1直接输入字符串 "" eg：名字 兴趣爱好  性别 （中文，英文，符号）
# a = input("请输入一个名字")
# print("您刚才输入的是",a)#变量两边不需要加双引号
# print("您刚才输入的是" + a)

# #2间接输入数字 eg:身高 体重 年龄 年纪 整数 小数
# b = int(input("请输入一个数字"))#"1"
# c = float(input("请输入一个数字"))#"1.0"
# d = eval(input("请输入一个数字"))
# print("您刚才输入的是",d)#变量两边不需要加双引号
# #str()把数字转化成字符串
# print("您刚才输入的是" + str(d))#加号如果又一遍是字符串，另外一边也要是字符串


#变量名的命名规则，可以一直赋值
#字符串的加法乘法，双引号(单引号)！！！！  字符串不能和数字相加
#保留字
#['False', 'None', 'True', 'and', 'as', 'assert', 'break', 'class', 'continue', 'def', 'del', 'elif', 'else', 'except', 'finally', 'for', 'from', 'global', 'if', 'import', 'in', 'is', 'lambda', 'nonlocal', 'not', 'or', 'pass', 'raise', 'return', 'try', 'while', 'with', 'yield']

#基本运算，优先级，名称
#赋值运算等号
#比较运算
#逻辑运算 and or not print(1<2 and 2<3)  print(1<2 or 2>3)  print(not 1<2)
'''
1, x or y 的值只可能是x或y. x为大于0的就输出x, x为0就输出y

2, x and y 的值只可能是x或y. x为大于0就输出y, x为0就输出0
'''
a*=a+b #a = a*(a+b)

