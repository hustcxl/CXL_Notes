# MATLAB常用命令学习笔记
 matlab 文档使用非常方便，库函数和命令都有非常详细的解释和示例，但是由于库过于庞大，无法全部掌握，仅将一些特殊功能的函数记下来，以便快速查阅参考。
## 1. 绘图
### 绘图命令
* fplot 函数绘图 
* subplot 绘制图组 
* imagesc绘制二维色阶图
* pcolor绘制各种类型伪彩图，例如时频表示
* mesh 三维图
* compass 绘制矢量
* text 向数据点添加文本说明
* annotation  创建注释
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
* solve 方程求解，dsolve微分方程求解
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
* fit_ellipse [拟合椭圆](https://ww2.mathworks.cn/matlabcentral/fileexchange/3215-fit_ellipse)
* [相关性和卷积](https://ww2.mathworks.cn/help/signal/correlation-and-convolution.html?s_tid=CRUX_lftnav)
* [polyfit](https://ww2.mathworks.cn/help/matlab/ref/polyfit.html)
## 4.工具函数
* findpeaks 极值点求取，可以设置间隔参数，另参考EMD工具包中的extr函数
* sortrows 矩阵行排序
* find 查找一定条件的点 
* eval 执行文本命令
* extractBefore 提取前几个字符串
* copyfile 拷贝文件
* fullfile 构建完整文件名
## 5. 矩阵和数组
* [MATLAB文档矩阵和数组](https://ww2.mathworks.cn/help/matlab/matrices-and-arrays.html?s_tid=CRUX_lftnav)
* fliplr 翻转行向量
* max向量的最大值，maxk 求取K个最大值
* reshap 重构矩阵
* repmat 重复数组副本
## 6.信号处理工具箱
* awgn 向信号添加高斯白噪声
* envelope 求信号包络  
* angle 相位角
* unwrap 更正相位角以生成更平滑的相位图
* [tfridge 时频脊线检测](https://ww2.mathworks.cn/help/signal/ref/tfridge.html?searchHighlight=tfridge&s_tid=doc_srchtitle)
* [instfreq 瞬时频率](https://ww2.mathworks.cn/help/signal/ref/instfreq.html?searchHighlight=instfreq&s_tid=doc_srchtitle)
 与tfbox工具箱中同名，调用方式存在冲突。
 * [hilbert 与瞬时频率](https://ww2.mathworks.cn/help/signal/ug/hilbert-transform-and-instantaneous-frequency.html)
 * [ordertrack 转速跟踪](https://ww2.mathworks.cn/help/signal/ref/ordertrack.html#bvflud5)
 * [振动分析相关示例和函数](https://ww2.mathworks.cn/help/signal/vibration-analysis.html?s_tid=CRUX_lftnav)
 * [tsa Time-synchronous信号平均](https://ww2.mathworks.cn/help/signal/ref/tsa.html?searchHighlight=tachorpm&s_tid=doc_srchtitle)
 
 - 阶次分析相关  

 函数	| 功能
 :--: | :--:
 envspectrum	| Envelope spectrum for machinery diagnosis(包络谱)
orderspectrum	 | Average spectrum versus order for vibration signal（振动信号的平均谱与阶）
ordertrack	 | Track and extract order magnitudes from vibration signal（跟踪并提取振动信号的阶数）
orderwaveform 	| 	Extract time-domain order waveforms from vibration signal（从振动信号中提取时域阶次波形）
rpmfreqmap	 | Frequency-RPM map for order analysis（阶次分析频率转速map分析）
rpmordermap	| Order-RPM map for order analysis（阶次转速map分析）
rpmtrack	| Track and extract RPM profile from vibration signal（跟踪并从振动信号中提取RPM剖面）
tachorpm	 | Extract RPM signal from tachometer pulses（从转速表脉冲中提取RPM信号）
tsa		 | Time-synchronous signal average（时间同步压缩信号平均）

- [时频分析](https://ww2.mathworks.cn/help/signal/time-frequency-analysis.html)  


 函数   | 功能
 :-- | :--
emd		| Empirical mode decomposition 经验模态分解
fsst		| Fourier synchrosqueezed transform 傅里叶同步压缩变换
ifsst		| Inverse Fourier synchrosqueezed transform 
hht		| Hilbert-Huang transform 希尔波特黄变换
instfreq	| Estimate instantaneous frequency 瞬时频率
kurtogram	| Visualize spectral kurtosis 可视化谱峰度
pkurtosis	| Spectral kurtosis from signal or spectrogram 光谱峰度从信号或光谱图
pentropy	| Spectral entropy of signal 信号谱熵
pspectrum	| Analyze signals in the frequency and time-frequency domains 分析频域和时频域的信号
spectrogram	| Spectrogram using short-time Fourier transform 使用短时傅里叶变换的谱图
xspectrogram	| Cross-spectrogram using short-time Fourier transforms 使用短时傅里叶变换的交叉谱图
stft		| Short-time Fourier transform 短时傅里叶变换
iscola		| Determine whether window-overlap combination is COLA compliant 确定窗口重叠组合是否符合COLA
istft		| Inverse short-time Fourier transform 短时傅里叶变换逆变换
tfridge		| Time-frequency ridges 时频脊线
wvd		| Wigner-Ville distribution and smoothed pseudo Wigner-Ville distribution 魏格纳-维纳分布
xwvd		| Cross Wigner-Ville distribution and cross smoothed pseudo Wigner-Ville distribution


[:back:返回主目录](../README.md)
