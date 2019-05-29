# MATLAB常用命令学习笔记
 matlab 文档使用非常方便，库函数和命令都有非常详细的解释和示例，但是由于库过于庞大，无法全部掌握，仅将一些特殊功能的函数记下来，以便快速查阅参考。
## 1. 绘图
### 绘图命令
* 函数绘图 fplot
* 绘制图组 subplot
* imagesc 绘制二维色阶图
* pcolor 绘制各种类型伪彩图，例如时频表示

### 绘图调整
* axis 坐标调整

## 2. 函数
* syms 创建系统变量与函数
* finverse 求函数的反函数
* linspace 生成线性间距向量
* logspace生成对数间距向量

## 3. 数学
* diff 微分
* trapz 梯形数值积分
* cumtrapz 累积梯形数值积分
* lambertw x\*ex的反函数

## 4.工具函数
* findpeaks 极值点求取，可以设置间隔参数，另参考EMD工具包中的extr函数
