# 概率论期中考答案解析



time:20210419

author:hwb

[toc]



## 填空题

总体难度: 6

### 1

![image-20210419141749205](https://hwb-pic.oss-cn-shenzhen.aliyuncs.com/img/image-20210419141749205.png?x-oss-process=style/hwb_shuiyin)

AB + AC + BC



### 2

![image-20210419141759310](https://hwb-pic.oss-cn-shenzhen.aliyuncs.com/img/image-20210419141759310.png?x-oss-process=style/hwb_shuiyin)

4个人生日不在同一天 <==> 1 - 四个人生日在同一天:
$$
P = 1- C^1_{365}* \frac{1}{365^4} = 1 - \frac{1}{365^3}
$$

### 3

![image-20210419141957059](https://hwb-pic.oss-cn-shenzhen.aliyuncs.com/img/image-20210419141957059.png?x-oss-process=style/hwb_shuiyin)
$$
f_X(x) =\begin{cases}\frac{1}{2}, x\in (0,2)\\
0,others \end{cases}
$$

$$
F_X(x) =\begin{cases}\frac{x}{2}, x\in (0,2)\\0,others \end{cases}
$$

y (0,4)

$$
f_Y(y)=F^{'}_Y(y) = F^{'}_X(\sqrt{y}) = \frac{dF_X('x')}{d'x'} * \frac{dx}{dy} = f_X(\sqrt{y})* \frac{1}{2\sqrt{y}} = \frac1{4\sqrt{y}}
$$

result:
$$
f_Y(y) =\begin{cases}\frac{1}{4\sqrt{y}}, y\in (0,4)\\
0,others \end{cases}
$$

### 4

![image-20210419145557021](https://hwb-pic.oss-cn-shenzhen.aliyuncs.com/img/image-20210419145557021.png?x-oss-process=style/hwb_shuiyin)

题目求AB非
$$
P(A) = P(A \overline{B}) + P(AB)\\
P(AB) = 0.5-0.2 = 0.3
$$


### 5

![image-20210419145617813](https://hwb-pic.oss-cn-shenzhen.aliyuncs.com/img/image-20210419145617813.png?x-oss-process=style/hwb_shuiyin)

二项分布/伯努利分布 npq

### 6

![image-20210419145653316](https://hwb-pic.oss-cn-shenzhen.aliyuncs.com/img/image-20210419145653316.png?x-oss-process=style/hwb_shuiyin)

**时间**均值 0

### 7

![image-20210419145721165](https://hwb-pic.oss-cn-shenzhen.aliyuncs.com/img/image-20210419145721165.png?x-oss-process=style/hwb_shuiyin)

![image-20210419145733145](https://hwb-pic.oss-cn-shenzhen.aliyuncs.com/img/image-20210419145733145.png?x-oss-process=style/hwb_shuiyin)

刻在骨子里的关系式:
$$
S_X(\omega) = \int R_X(\tau) e^{-j\omega \tau} d\tau
$$

### 8

![image-20210419145926323](https://hwb-pic.oss-cn-shenzhen.aliyuncs.com/img/image-20210419145926323.png?x-oss-process=style/hwb_shuiyin)
$$
\begin{aligned}
f(x) &= \frac{a}{1+x^2}\\
\int^{+\infty}_{-\infty} f(x)dx &= a* \arctan{x}|^{+\infty}_{-\infty}=1 \\
a(\frac{\pi}{2}- (-\frac{\pi}{2})) &= 1\\
a &=\frac{1}{\pi}

\end{aligned}
$$


### 9

![image-20210419202914370](https://hwb-pic.oss-cn-shenzhen.aliyuncs.com/img/image-20210419202914370.png?x-oss-process=style/hwb_shuiyin)

**送分题**

问的边缘分布,这个是标准二元高斯分布:
$$
f_X(x) = \frac1{\sqrt{2\pi} \sigma_1} e^{-\frac{(x-\mu_1)^2}{2\sigma_1^2}}, -\infty < x<+\infty
$$

$$
f_Y(y) = \frac1{\sqrt{2\pi} \sigma_2} e^{-\frac{(y-\mu_2)^2}{2\sigma_2^2}}, -\infty < y<+\infty
$$

### 10

![image-20210419204409712](https://hwb-pic.oss-cn-shenzhen.aliyuncs.com/img/image-20210419204409712.png?x-oss-process=style/hwb_shuiyin)

随机变量变换问题,**送分题**

假设X服从正态分布(为了符号好写)
$$
X \sim N(E(X), \sqrt{D(X)} )\\
X^* = \frac{X- E(X)}{\sqrt{D(X)}}
$$
即$X^*$退化为标准正态分布:
$$
X \sim N(0, 1 )
$$


## 大题

### 二

![image-20210419204721017](https://hwb-pic.oss-cn-shenzhen.aliyuncs.com/img/image-20210419204721017.png?x-oss-process=style/hwb_shuiyin)
$$
\begin{aligned}
E(3X+1) =  &(-2*3 + 1)*0.1 + \\  &(-1*3 +1)*0.2 +\\ &(0*3+1)*0.3 +\\ &(1*3 + 1)*0.4 = \\
&-0.5 + (-0.4) +0.3 + 1.6=1
\end{aligned}
$$

$$
\begin{aligned}
E(X^2) =  &(-2)^2*0.1 + \\  &(-1)^2*0.2 +\\ &(0)^2*0.3 +\\ &(1)^2*0.4 = \\
&0.4 + 0.2 + 0 + 0.4 =1
\end{aligned}
$$

### 三

![image-20210419205859514](https://hwb-pic.oss-cn-shenzhen.aliyuncs.com/img/image-20210419205859514.png?x-oss-process=style/hwb_shuiyin)

由对称性:
$$
P(0<X<2) =P(2<X<4)= 0.3\\
P(X<2) = 0.5\\
P(X<0) = P(X<2) - P(0<X<2) = 0.2
$$

### 四

![image-20210419210213156](https://hwb-pic.oss-cn-shenzhen.aliyuncs.com/img/image-20210419210213156.png?x-oss-process=style/hwb_shuiyin)

![image-20210419210221432](https://hwb-pic.oss-cn-shenzhen.aliyuncs.com/img/image-20210419210221432.png?x-oss-process=style/hwb_shuiyin)

技术活:

![image-20210419210422292](https://hwb-pic.oss-cn-shenzhen.aliyuncs.com/img/image-20210419210422292.png?x-oss-process=style/hwb_shuiyin)

答案应该有问题,改的时候取方案1

### 五 

<img src="https://hwb-pic.oss-cn-shenzhen.aliyuncs.com/img/image-20210419210520862.png?x-oss-process=style/hwb_shuiyin" alt="image-20210419210520862" style="zoom:66%;" />

见板书

1. 离散随机变量 画表

![image-20210423141757925](https://hwb-pic.oss-cn-shenzhen.aliyuncs.com/img/image-20210423141757925.png?x-oss-process=style/hwb_shuiyin)

### 六

![image-20210419210851648](https://hwb-pic.oss-cn-shenzhen.aliyuncs.com/img/image-20210419210851648.png?x-oss-process=style/hwb_shuiyin)

(1) 用概率密度函数积分和=1
$$
\begin{aligned}
\int^{+\infty}_{-\infty} f(x) &= \int^{+\infty}_{1000} \frac{c}{x^2}dx = 1\\

-\frac{c}{x}|^{+\infty}_{1000} &=1\\
-c(0-\frac1{1000}) &= 1\\
c&=1000
\end{aligned}
$$

(2)条件概率定义

$$
\begin{aligned}

P(X\le 1700|1500< X<2000) &= \frac{P(X\le 1700,1500< X<2000)}{P(1500< X<2000)}\\
&=\frac{P(1500< X\le 1700)}{P(1500< X<2000)}\\

&=\frac{\int^{1700}_{1500} \frac{1000}{x^2}dx}{\int^{2000}_{1500} \frac{1000}{x^2}dx}\\
&=\frac{24}{51} = \frac{8}{17} \approx 0.4706
\end{aligned}
$$
(3) 先求损坏概率,由于各灯之间独立同分布,用二项分布就完事了
$$
P(A) =P(0\leq X<1500) =\int^{1500}_{1000} \frac{1000}{x^2}dx = \frac13
$$
所以损坏概率服从伯努利分布:
$$
Y\sim B(3,\frac13)\\
P(Y=1) = P_3(1) = C^1_3 (\frac13)(\frac23)^2 = \frac49
$$

### 七

![image-20210423141307038](https://hwb-pic.oss-cn-shenzhen.aliyuncs.com/img/image-20210423141307038.png?x-oss-process=style/hwb_shuiyin)

![image-20210423141349508](https://hwb-pic.oss-cn-shenzhen.aliyuncs.com/img/image-20210423141349508.png?x-oss-process=style/hwb_shuiyin)

此题简单,不作解析,不写f(x,y)扣2分

解:(1)

![image-20210423141638018](https://hwb-pic.oss-cn-shenzhen.aliyuncs.com/img/image-20210423141638018.png?x-oss-process=style/hwb_shuiyin)

## 八

送分题

![image-20210423142147337](https://hwb-pic.oss-cn-shenzhen.aliyuncs.com/img/image-20210423142147337.png?x-oss-process=style/hwb_shuiyin)

![image-20210423142709349](https://hwb-pic.oss-cn-shenzhen.aliyuncs.com/img/image-20210423142709349.png?x-oss-process=style/hwb_shuiyin)

![image-20210423142700032](https://hwb-pic.oss-cn-shenzhen.aliyuncs.com/img/image-20210423142700032.png?x-oss-process=style/hwb_shuiyin)








