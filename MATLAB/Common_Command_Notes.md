# MATLAB常用命令学习笔记
 matlab 文档使用非常方便，库函数和命令都有非常详细的解释和示例，但是由于库过于庞大，无法全部掌握，仅将一些特殊功能的函数记下来，以便快速查阅参考。
## 1. 绘图
### 绘图命令
* fplot 函数绘图 
* subplot 绘制图组 
* imagesc绘制二维色阶图
* pcolor绘制各种类型伪彩图，例如时频表示
* mesh 三维图
### 绘图调整
[绘图调整参考文档](https://ww2.mathworks.cn/help/matlab/graphics-object-identification.html?searchHighlight=%E5%9B%BE%E5%BD%A2%E5%AF%B9%E8%B1%A1%E7%9A%84%E6%A0%87%E8%AF%86&s_tid=doc_srchtitle)
* axis 坐标调整
* gca 获取当前坐标区域或图
* gcf 当前图窗的句柄


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
* spline 样条插值
* floor 负无穷四舍五入
* ceil 正无穷四舍五入
* round 四舍五入最近的整数
* conj 复共轭

* [相关性和卷积](https://ww2.mathworks.cn/help/signal/correlation-and-convolution.html?s_tid=CRUX_lftnav)
## 4.工具函数
* findpeaks 极值点求取，可以设置间隔参数，另参考EMD工具包中的extr函数
* sortrows 矩阵行排序
* find 查找一定条件的点 
* awgn 向信号添加高斯白噪声
 


## 5. 矩阵和数组
* [MATLAB文档矩阵和数组](https://ww2.mathworks.cn/help/matlab/matrices-and-arrays.html?s_tid=CRUX_lftnav)
* fliplr 翻转行向量
