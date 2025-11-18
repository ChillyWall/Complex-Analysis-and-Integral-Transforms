# 复数与复变函数

## 复数

### 有关定义

规定 $i^2=-1$ 并正常参与四则运算。

有 $z=x+yi$ 中 $x,y$ 分别称为实部和虚部，记作
 $x=\operatorname{Re}(z),y=\operatorname{Im}(z).$

当 $x=0,y \ne 0$ 时称为纯虚数，而 $y=0$ 的时候我们直接看作实数。

两复数相等**当且仅当**它们的实部和虚部**分别相等**。

复数等于0**当且仅当**它的实部和虚部**同时等于0**.

!!!note 复数中**无法定义大小关系**
    假设存在这样的序关系“$ > $”。

    1. 假设 $i > 0$
    - 由乘法保序性：$i \cdot i > 0 \cdot  i\Rightarrow -1 > 0$ （矛盾）

    2. 假设 $i < 0$
    - 则 $-i > 0$
    - 由乘法保序性：$(-i) \cdot (-i) > 0 \cdot (-i) \Rightarrow i^2 > 0$ ⇒ $-1 > 0$ （矛盾）

    两种假设都导致 $-1 > 0$ 的矛盾，因此在复数中**无法定义**满足序关系性质的大小关系。

设两复数 $z_{1}=x_{1}+iy_{1}$，$z_{2}=x_{2}+iy_{2}$

**1. 两复数的和、差：**
$$
z_{1} \pm z_{2} = (x_{1} \pm x_{2}) + i(y_{1} \pm y_{2})
$$

**2. 两复数的积：**
$$
z_{1} \cdot z_{2} = (x_{1}x_{2} - y_{1}y_{2}) + i(x_{2}y_{1} + x_{1}y_{2})
$$

**3. 两复数的商：**
$$
\frac{z_{1}}{z_{2}} = \frac{x_{1}x_{2} + y_{1}y_{2}}{x_{2}^{2} + y_{2}^{2}} + i\frac{x_{2}y_{1} - x_{1}y_{2}}{x_{2}^{2} + y_{2}^{2}}
$$

### 共轭复数

**定义**：实部相同而虚部绝对值相等符号相反的两个复数称为共轭复数。

**表示方法**：与 $z$ 共轭的复数记为 $\bar{z}$。

**数学表达式**：
若 $z = x + iy$，则其共轭复数 $\bar{z} = x - iy$（其中 $x$, $y$ 为实数，$i$ 为虚数单位）。

!!!note
    两个共轭复数 $z,\bar{z}$ 的积是一个实数。

**四则运算**：

1. 基本运算
   - **加减法**：$\overline{z_{1} \pm z_{2}} = \bar{z}_{1} \pm \bar{z}_{2}$
   - **乘法**：$\overline{z_{1} \cdot z_{2}} = \bar{z}_{1} \cdot \bar{z}_{2}$
   - **除法**：$\overline{\left(\dfrac{z_{1}}{z_{2}}\right)} = \dfrac{\bar{z}_{1}}{\bar{z}_{2}}$

2. 自反性
   - $\overline{\bar{z}} = z$（共轭的共轭等于自身）

3. 模的平方
   - $z \cdot \bar{z} = [\operatorname{Re}(z)]^{2} + [\operatorname{Im}(z)]^{2} = |z|^2$

4. 实部与虚部提取
   - $z + \bar{z} = 2\operatorname{Re}(z)$
   - $z - \bar{z} = 2i\operatorname{Im}(z)$

## 复平面

### 定义

1. 复数 $z = x + iy$ 与有序实数对 $(x, y)$ 成一一对应。
2. 一个建立了直角坐标系的平面可以用来表示复数。这种用来表示复数的平面叫**复平面**。
3. 通常把**横轴**叫**实轴**或 $x$ 轴，**纵轴**叫**虚轴**或 $y$ 轴。

复数 $z = x + iy$ 可以用复平面上的点 $(x, y)$ 表示。

### 模

将 $z = x + iy$ 用复平面上的向量 $\overrightarrow{OP}$ 表示，此时 $|z|=\left|\overrightarrow{OP}\right|=\sqrt{x^2+y^2}.$

显然：

1. $|x|\le |z|$
2. $|y|\le |z|$
3. $|z| \le |x|+|y|$
4. $z\bar{z}=|z|^2$

### 幅角

当 $z=0$ 时，幅角**不确定**。

当 $z \ne 0$ 时：

1. 以正实轴为始边，以表示复数 $z$ 的向量 $\overrightarrow{OP}$ 为终边的角 $\theta$ 称为 $z$ 的幅角，记作 $\operatorname{Arg}z.$
2. 把满足 $-\pi<\theta_0<\pi$ 的 $\theta_0$ 称为幅角主值：

$$
\operatorname{arg}z=
\begin{cases}
\arctan \dfrac{y}{x}, & x > 0 \\
\pm \dfrac{\pi}{2}, & x = 0,y \ne 0 \\
\arctan \dfrac{y}{x}\pm \pi, & x<0,y\ne 0\\
\pi & x<0, y=0
\end{cases}
$$
其中$-\dfrac{\pi}{2}<\arctan\dfrac{y}{x}<\dfrac{\pi}{2}.$

### 平行四边形法则

平行四边形法则计算加减法与向量加减法的方法一致。

### 复数差和模的性质

因为 $|z_{1}-z_{2}|$ 表示点 $z_{1}$ 和 $z_{2}$ 之间的距离，故：

1. $|z_{1} + z_{2}| \le |z_{1}| + |z_{2}|$ （三角不等式）

2. $|z_{1} - z_{2}| \ge \left| |z_{1}| - |z_{2}| \right|$ （反向不等式）

一对共轭复数 $z$ 和 $\bar{z}$ 在复平面内的位置是关于实轴对称的。

### 三角表示和指数表示

利用
$
\begin{cases}
x = r\cos\theta\\
y = r\sin\theta
\end{cases}
$

将复数表示为
$$z=r(\cos\theta+i\sin\theta)\tag{三角表示}$$

再利用欧拉公式：$e^{i\theta}=\cos\theta+i\sin\theta$

我们将复数表示成：
$$z=re^{i\theta}\tag{指数表示}$$

### 一些证明

$$
\begin{aligned}
|z_1z_2|&=\sqrt{(z_1z_2)\overline{(z_1z_2)}}\\
&=\sqrt{(z_1z_2)(\bar{z}_1\bar{z}_2)}\\
&=\sqrt{(z_1\bar{z}_1)(z_2\bar{z}_2)}\\
&=|z_1||z_2|
\end{aligned}
$$
$$
\begin{aligned}
\left|z_{1}+z_{2}\right|^{2} &=\left(z_{1}+z_{2}\right)\overline{\left(z_{1}+z_{2}\right)}=\left(z_{1}+z_{2}\right)\left(\bar{z}_{1}+\bar{z}_{2}\right)\\
&=z_{1}\bar{z}_{1}+z_{2}\bar{z}_{2}+\bar{z}_{1} z_{2}+z_{1}\bar{z}_{2}\\
&=\left|z_{1}\right|^{2}+\left|z_{2}\right|^{2}+\bar{z}_{1} z_{2}+z_{1}\bar{z}_{2}
\end{aligned}
$$

因为 $\bar{z}_{1}z_{2}+z_{1}\bar{z}_{2}=2\operatorname{Re}(z_{1}\bar{z}_{2})$,于是
$$
\begin{aligned}
\left|z_{1}+z_{2}\right|^{2}&=\left|z_{1}\right|^{2}+\left|z_{2}\right|^{2}+2\operatorname{Re}(z_{1}\bar{z}_{2}) \\
&\leq\left|z_{1}\right|^{2}+\left|z_{2}\right|^{2}+2\left|z_{1}\bar{z}_{2}\right| \\
&=\left|z_{1}\right|^{2}+\left|z_{2}\right|^{2}+2\left|z_{1}\right|\left|z_{2}\right| \\
&=\left(\left|z_{1}\right|+\left|z_{2}\right|\right)^{2}
\end{aligned}
$$

两边同时开方得 $\left|z_{1}+z_{2}\right|\leq\left|z_{1}\right|+\left|z_{2}\right|$。

### 直线方程

写出一个直线的参数方程：

$$
\left\{
\begin{array}{l}
x = x_1 + t (x_2 - x_1) \\
y = y_1 + t (y_2 - y_1)
\end{array}
\right.
\quad t \in (-\infty, +\infty)
$$

于是它的复数形式为：

$$
z=z_1+t(z_2-z_1)\quad t\in (-\infty,+\infty)
$$
从 $z_1$ 到 $z_2$ 的直线段就取 $t \in (0,1)$ ，取 $t=\dfrac{1}{2}$ 就能得到中点坐标为 $\dfrac{z_1+z_2}{2}$。

## 复球面

### 复球面定义

取复平面与球面切于 $z=0$，球面上点 $S$ 和原点重合为 $S$ 极/南极。另一端为 $N$ 极/北极。

### 对应

对于除 $N$ 外任意一点 $P$，连接 $NP$ 就能建立复球面和复平面的对应。

然后规定复数中有一个“无穷大”来对应 $N$ 点。记号仍然用 $\infty$ 这个符号。

### 扩充复平面

加上了无穷远点的复平面称为扩充复平面。

不包括无穷远点的叫有限复平面或者直接叫复平面。

$\operatorname{Re}(\infty), \operatorname{Im}(\infty), \operatorname{Arg}(\infty)$ 等概念都没有意义，然后我们规定它的模是 $+\infty$。

无穷远点的邻域是一个半径足够大的圆的外部。

### 无穷的四则运算

1. 加法：$\alpha + \infty = \infty + \alpha = \infty$, $(\alpha \neq \infty)$

2. 减法：$\alpha - \infty = \infty - \alpha = \infty$, $(\alpha \neq \infty)$

3. 乘法：$\alpha \cdot \infty = \infty \cdot \alpha = \infty$, $(\alpha \neq 0)$

4. 除法：$\frac{\alpha}{\infty} = 0$, $\frac{\infty}{\alpha} = \infty$, $(\alpha \neq \infty)$, $\frac{\alpha}{0} = \infty$, $(\alpha \neq 0)$

5. 神秘的运算依然神秘，$\infty \pm \infty, 0 \cdot \infty, \frac{\infty}{\infty}, \frac{0}{0}$ 依然**没有意义**。

## 乘除幂根

### 乘和除

若 $z_1=r_1(\cos\theta_1+i\sin\theta_1),z_2=r_2(\cos\theta_2+i\sin\theta_2)$，则
$$
\begin{aligned}
z_{1}z_{2} &= r_{1}r_{2}(\cos\theta_{1}+i\sin\theta_{1})(\cos\theta_{2}+i\sin\theta_{2}) \\
&= r_{1}r_{2}[(\cos\theta_{1}\cos\theta_{2}-\sin\theta_{1}\sin\theta_{2})+i(\sin\theta_{1}\cos\theta_{2}+\sin\theta_{2}\cos\theta_{1})] \\
&= r_{1}r_{2}[\cos(\theta_{1}+\theta_{2})+i\sin(\theta_{1}+\theta_{2})]
\end{aligned}
$$
于是
$$
|z_1z_2|=r_1r_2=|z_1||z_2|,\\
\operatorname{Arg}z_1z_2=\operatorname{Arg}z_1+\operatorname{Arg}z_2.
$$

!!!note
    需要注意：
    这里的 $\operatorname{Arg}$ 绝对不可以写成 $\operatorname{arg}$，因为这个式子的意思是两个集合相等。

    可以理解为这两个的区别：

    ```c
    set Arg(complex z);   // 结果是一个包含所有幅角的集合
    angle arg(complex z); // 结果是一个幅角，代表主值
    ```

    也就是说，$\operatorname{arg}z_1z_2=\operatorname{arg}z_1+\operatorname{arg}z_2$ 是**不一定成立**的。

也就是：**模量相乘，幅角相加**。

从几何上看可以视为缩放和旋转，而且可以把结论推广到**更多个复数相乘的情况**。

并且同样可以拓展到商：**模量相除，幅角相减**。

写成指数形式就是：

若 $z_1=r_1e^{i\theta_1}, z_2=r_2e^{i\theta_2}$，则
$$
z_1z_2=r_1r_2e^{i(\theta_1+\theta_2)},\frac{z_1}{z_2}=\frac{r_1}{r_2}e^{i(\theta_1-\theta_2)}.
$$

### 幂和根

幂的定义和实数是一样的。
$$
z^n=\overbrace{z\cdot z \cdots z}^{n\text{个}},\\
z^{-n}=\frac{1}{z^n}.
$$
然后，对于 $n \in \mathbb{N^*}$，$z_n=r_n(\cos n \theta + i \sin n \theta)$。

**棣莫佛公式**：当 $z$ 的模 $r=1$，即 $z=\cos\theta+i\sin\theta$ 时，
$$ (\cos\theta+i\sin\theta)^n=\cos n\theta+i\sin n\theta. $$

复数开根的时候，**几次方根必有几个结果**，所以把开根当成一个**多值函数**。

$$
\sqrt[n]{z}=r^\frac{1}{n}\left(\cos\frac{\theta+2k\pi}{n}+i\sin\frac{\theta+2k\pi}{n} \right),k=0,1,\cdots,n-1.
$$
当 $k=0,1,2,\cdots,n-1$ 时，得到 $n$ 个相异的根：
$$
\begin{aligned}
w_0 &= r^{\frac{1}{n}} \cdot \left( \cos\frac{\theta}{n} + i\sin\frac{\theta}{n} \right)\\
w_1 &= r^{\frac{1}{n}} \cdot \left( \cos\frac{\theta + 2\pi}{n} + i\sin\frac{\theta + 2\pi}{n} \right)\\
&\cdots\\
w_{n-1} &= r^{\frac{1}{n}} \cdot \left( \cos\frac{\theta + 2(n-1)\pi}{n} + i\sin\frac{\theta + 2(n-1)\pi}{n} \right)\\
w_n&=w_0,w_{n+1}=w_1,\cdots
\end{aligned}
$$
几何上看，就是以原点为中心，$r^\frac{1}{n}$ 为半径的圆的内接正 $n$ 边形的 $n$ 个顶点。
!!!note
    一旦涉及开根运算，务必不要忘记写 $k=0,1,\cdots$ 来表示所有值！

## 区域

### 相关定义

**邻域**：平面上以 $z_0$ 为中心， $\delta$ 为半径的圆：$|z-z_0|<\delta$ 内部的点的集合称为 $z_0$ 的**邻域**。

**去心邻域**：把 $z_0$ 自己去掉，也就是 $0 < |z-z_0| < \delta$

!!!note
    无穷远点也有邻域和去心邻域，分别是**包含/不包含自身在内**，满足 $|z| > M$ 的集合。

    需要注意的是，这里 $\delta,M>0$ 就可以，定义邻域的时候不要求它们足够大或者足够小。

**内点**：设 $G$ 为一平面点集，$z_0$ 为 $G$ 中任意一点。如果存在 $z_0$ 的一个邻域，该邻域内的所有点都属于 $G$，那么 $z_0$ 称为 $G$ 的内点。

**开集**：如果 $G$ 内每一点都是它的内点，那么 $G$ 称为开集。

**区域**：
如果平面点集 $D$ 满足以下两个条件，则称它为一个区域：

1. $D$ 是一个**开集**；
2. $D$ 是**连通的**，即 $D$ 中任何两点都可以用完全属于 $D$ 的一条折线连结起来。

**边界点、边界**：
设 $D$ 是复平面内的一个区域，如果点 $P$ 不属于 $D$，但在 $P$ 的任意小的邻域内总有 $D$ 中的点，这样的点 $P$ 称为 $D$ 的**边界点**。
> 通俗理解的话，边界和边界点的定义很符合直观，然后开集就是不带边界，区域就是还要求没有从中间断开。

**有界和无界**：
存在 $M > 0$ 使得对于 $\forall z,|z| < M$ 则 $D$ 有界。否则无界。

### 单连通域和多连通域

**平面曲线的复数表示**：
$$
z=z(t)=x(t)+iy(t),a \le t \le b
$$

- 连续曲线：$x(t)$ 和 $y(t)$ 是连续的实变函数。

- 光滑曲线：在 $[a,b]$ 上 $x'(t),y'(t)$ 连续，且对于 $\forall t, [x'(t)]^2 + [y'(t)]^2 \ne 0$。

- 起点：$z(a)$
- 终点：$z(b)$
- 重点：$\exists t_1 \ne t_2, z(t_1)=z(t_2)$。
- 简单曲线：没有重点（自身不相交）。

> 几段光滑曲线相接称为按段光滑曲线。
>
> 如果起点终点重合,也就是 $z(a)=z(b)$，为简单闭曲线。

任何一条简单闭曲线把复平面唯一地分为三个互不相交的点集：内部，外部，边界。

**单连通域**：
任意作简单闭曲线，曲线内部总属于该区域。
> 也就是没有洞。

**多连通域**：
不是单连通域的区域。
> 有洞。哪怕只有一个空心点也是有洞。

!!!tip
    极坐标方程的曲线看对称性，看 $\theta$ 和 $-\theta$（上下），$\pi - \theta$（左右）的关系。

    $r^2 = 2\cos 2\theta$ 也就是 $|z+1|\cdot |z-1| = 1$ 是双叶玫瑰线。
    
    其内部不是区域。

## 复变函数

### 一些定义

定义的画风和实变函数很像：

设 $G$ 是一个复数 $z = x + iy$ 的集合。如果有一个确定的法则存在，按这个法则，对于集合 $G$ 中的每一个复数 $z$，就有一个或几个复数 $w = u + iv$ 与之对应，则称复变数 $w$ 是复变数 $z$ 的函数（简称复变函数），记作 $w = f(z)$。

**单值函数和多值函数**：
一个 $z$ 对应一个 $w$，还是对应许多个 $w$。

**定义集合和函数值集合**：
定义域和值域的复变版。符号：$G$ 和 $G^*$。

**复变函数与自变量的关系**：
$w=f(z)$ 相当于两个关系式：
$$
u=u(x,y),v=v(x,y)
$$

### 映射

如果用 $z$ 平面上的点表示自变量 $z$ 的值，而用另一个平面 $w$ 上的点表示函数 $w$ 的值，则函数 $W=f(z)$ 在几何上就可以看作是把平面上的一个点集 $G$（定义集合）变到 $w$ 平面上的一个点集 $G*$（函数值集合）的**映射**（或变换）。

此映射简称为函数 $w=f(z)$ 构成的映射。

如果 $G$ 中的点 $z$ 被映射 $w = f(z)$ 映射成 $G^*$ 中的点 $w$，则 $w$ 称为 $z$ 的**象（映象）**，而 $z$ 称为 $w$ 的**原象**。

两个特殊映射：

1. $w=\bar{z}$：关于实轴的对称映射。
2. $w=z^2$：
    - 能够把与实轴交角为 $\alpha$ 的角形域映射成交角为 $2\alpha$ 的角形域。
    - 因为对应于 $u=x^2-y^2,v=2xy$ 这两个实变函数，所以它可以把 $z$ 平面上两族分别以 $y=\pm x$ 和两坐标轴为渐近线的等轴双曲线：
    $$
    x^2-y^2=c_1,2xy=c_2
    $$
    分别映射成两族平行直线：
    $$
    u=c_1,v=c_2.
    $$
    - 考虑直线 $x=\lambda$ 的象的参数方程：
    $$
    \begin{cases}
    u &= \lambda^2-y^2,\\
    v &=2\lambda y.
    \end{cases}
    $$
    而消去参数 $y$：
    $$
    v^2=4\lambda^2(\lambda^2-u)
    $$
    是以原点为焦点而开口朝右的抛物线。
3. 反函数：$G^*$ 中的每个 $w$ 一定对应了一个或几个 $z$，于是确定了一个单值或多值的反函数，也叫逆映射。
   > 如果函数和反函数都是单值函数，我们称其是**一一对应**的。
   >
   > 并且，此后我们不再区分函数和映射。

## 复变函数的极限和连续性

### 极限

设函数 $w=f(z)$ 定义在 $z_0$ 的去心邻域 $0 < |z - z_0| < \rho$ 内，如果有一确定的数 $A$ 存在，对于任意给定的 $\varepsilon > 0$，相应地必有一正数 $\delta(\varepsilon)$ 使得当 $0 < |z - z_0| < \delta$ $(0 < \delta \leq \rho)$ 时，有 $|f(z) - A| < \varepsilon$，则称 $A$ 为 $f(z)$ 当 $z$ 趋向于 $z_0$ 时的极限。
记作 $\lim_{z \to z_0} f(z) = A$（或 $f(z) \xrightarrow{z \to z_0} A$）

> 定义中 $z \to z_0$ 的方式是**任意的**。

### 极限计算的定理

1. 设 $ f(z) = u(x, y) + i v(x, y) $，$ A = u_0 + i v_0 $，$ z_0 = x_0 + i y_0 $，那末 $\lim_{z \to z_0} f(z) = A$ 的充要条件是：
    $$
    \lim_{\substack{x \to x_0 \\ y \to y_0}} u(x, y) = u_0, \quad \lim_{\substack{x \to x_0 \\ y \to y_0}} v(x, y) = v_0.
    $$
2. 极限运算法则与实变函数的极限运算法则是类似的。若 $\lim_{z \to z_0}f(z)=A, \lim_{z \to z_0}g(z)=B$，则：
    1. $\lim_{z \to z_0}[f(z) \pm g(z)] = A \pm B $
    2. $\lim_{z \to z_0}[f(z)g(z)]=AB$
    3. $\lim_{z \to z_0}\dfrac{f(z)}{g(z)}=\dfrac{A}{B},(B \ne 0)$

### 连续

如果 $\lim\limits_{z \to z_0} f(z) = f(z_0)$，那末我们就说 $f(z)$ 在 $z_0$ 处连续。如果 $f(z)$ 在区域 $D$ 内处处连续，我们说 $f(z)$ 在 $D$ 内连续。

函数 $f(z)$ 在曲线 $C$ 上 $z_0$ 处连续的意义是 $\lim\limits_{z \to z_0} f(z) = f(z_0)$，$z \in C$。

### 连续的相关定理

1. 函数 $f(z) = u(x, y) + iv(x, y)$ 在 $z_0 = x_0 + iy_0$ 处连续的充要条件是：$u(x, y)$ 和 $v(x, y)$ 在 $(x_0, y_0)$ 处连续。

2. 在 $z_0$ 连续的两个函数 $f(z)$ 和 $g(z)$ 的和、差、积、商（分母在 $z_0$ 不为零）在 $z_0$ 处仍连续。

3. 如果函数 $h = g(z)$ 在 $z_0$ 连续，函数 $w = f(h)$ 在 $h_0 = g(z_0)$ 连续，那末复合函数 $w = f[g(z)]$ 在 $z_0$ 处连续。

!!!note 特殊的：

   1. 有理整函数（多项式）
        $$
        w=P(z)=a_{0}+a_{1}z+a_{2}z^{2}+\cdots+a_{n}z^{n}
        $$
        对复平面内的所有点 $z$ 都是连续的；
   2. 有理分式函数
        $$
        w=\frac{P(z)}{Q(z)}
        $$
        其中 $P(z)$ 和 $Q(z)$ 都是多项式，在复平面内使分母不为零的点也是连续的。

## 章末杂项

1. 二次方程求根公式是
    $$
    x=\frac{-b \pm \sqrt{b^2-4ac}}{2a}
    $$
    但是对于复数来说，**开根是一个多值函数**。所以这时候没有必要再写 $\pm$ 号，因为 $\sqrt{b^2-4ac}$ 事实上**已经同时包含了两个结果**。
2. 需要注意的是 $\sqrt{z^2}=|z|$ 不再成立，因为开根是多值函数，而且绝对值和模也不一样。取而代之的是 $\sqrt{z^2}=\pm z$。
    !!!note
        归根结底是由于这个根号的含义**发生了改变**，从实数的**算术平方根**变成了复数的**二次方根**，而二次方根其实本来就有两个。
3. 神秘小例题：
   $w=\dfrac{1}{z}$ 会把以下曲线映射成 $w$ 平面上的什么曲线？

   1. $x^2+y^2=r^2 \to u^2+v^2=(\dfrac{1}{r})^2$
   2. $x=a \to (u-\dfrac{1}{2a})^2+v^2=(\dfrac{1}{2a})^2$

!!!note
    其实很好理解：$w=\dfrac{1}{z}$可不就是把原点和无穷远点的地位互换了吗？

# 解析函数

## 复变函数的导数和微分

### 导数

**定义**：设函数 $w=f(z)$ 定义于区域 $D$，$z_{0}$ 为 $D$ 中的一点，点 $z_{0}+\Delta{z}$ 不出 $D$ 的范围。
如果极限 $\lim\limits_{\Delta{z} \to 0} \dfrac{f(z_{0}+\Delta{z})-f(z_{0})}{\Delta{z}}$ 存在，就称 $f(z)$ 在 $z_{0}$ 可导。
这个极限值称为 $f(z)$ 在 $z_{0}$ 的导数，记作
$$
f^{\prime}(z_{0})=\left.\dfrac{dw}{dz}\right|_{z=z_{0}}=\lim_{\Delta{z} \to 0} \dfrac{f(z_{0}+\Delta{z})-f(z_{0})}{\Delta{z}}.
$$

!!!note
    在定义中应注意：

    $z_{0}+\Delta z \to z_{0}$（即 $\Delta z \to 0$）的方式是**任意的**。

    即 $z_{0}+\Delta z$ 在区域 $D$ 内以任意方式趋于 $z_{0}$ 时，

    比值 $\dfrac{f(z_{0}+\Delta z)-f(z_{0})}{\Delta z}$ 都趋于同一个数。

    如果函数 $f(z)$ 在区域 $D$ 内处处可导，我们就称 $f(z)$ 在区域 $D$ 内可导。

就函数的可导性而言：如果一个复变函数能写的只和 $z$ 有关而不依靠 $\bar{z}$ （依靠 $x,y$ 也算），那么它**可导**（甚至**解析**），并且表现得像对应的实变函数。

### 导数法则

1. $(c)' = 0$，其中 $c$ 为复常数。

2. $(z^{n})' = nz^{n-1}$，其中 $n$ 为正整数。

3. $[f(z)\pm g(z)]^{\prime}=f^{\prime}(z)\pm g^{\prime}(z)$

4. $[f(z)g(z)]^{\prime}=f^{\prime}(z)g(z)+f(z)g^{\prime}(z)$

5. $\left[\dfrac{f(z)}{g(z)}\right]^{\prime}=\dfrac{f^{\prime}(z)g(z)-f(z)g^{\prime}(z)}{g^{2}(z)}$，其中 $g(z)\neq 0$

6. $\{f[g(z)]\}^{\prime}=f^{\prime}(w)g^{\prime}(z)$，其中 $w=g(z)$

7. $f^{\prime}(z)=\dfrac{1}{\varphi^{\prime}(w)}$，其中 $w=f(z)$ 与 $z=\varphi(w)$ 是两个互为反函数的单值函数，且 $\varphi^{\prime}(w)\neq 0$

### 微分

**复变函数微分的概念在形式上和实变的一致。**

如果函数在 $z_0$ 的微分存在，则称 $f(z)$ 在 $z_0$ **可微**。

在某一点的可导和可微**等价**，且在一个**区域**内可微的意思是**处处可微**。

### 解析

如果 $f(z)$ 在 $z_0$ 和 $z_0$ 的邻域内处处可导，称它在 $z_0$ **解析**。

处处解析称为在区域上解析。

在区域内，**可导**，**解析**，**处处可导**，**处处解析**这四个词**等价**。

对于一点，可导的要求要比解析低。

### 奇点

如果函数 $f(z)$ 在 $z_0$ 点**不解析**，则称 $z_0$ 点为 $f(z)$ 的奇点。

注意：对于一个单独的点，可能出现**可导**却**不解析**的情况。

!!!note
    一个比较神人的函数：$f(z)=|z|^2$

    这个函数仅在 $z=0$ 这一点可导，所以处处不解析。*在 $z=0$ 也**不解析**！因为解析要求在某一点的邻域也可导。*

### 解析的相关定理

1. 除非分母为零，解析函数的和差积商在原解析范围内仍然解析。
2. 解析函数复合，在原解析范围内仍然解析。

## 函数解析的充要条件

### 柯西-黎曼方程

*此方程有时候会用这两个人名的首字母 C 和 R 表示为 **CR方程。***

函数 $f(z)$ 在一点可导的充要条件是：

1. $u(x,y)$ 和 $v(x,y)$ 在这一点可微。
2. 在这一点满足柯西黎曼方程：

$$
\frac{\partial u}{\partial x} = \frac{\partial v}{\partial y},\quad \frac{\partial u}{\partial y} = -\frac{\partial v}{\partial x}.
$$

得到求导公式：
$$
\begin{aligned}
   f'(z) &= \frac{\partial u}{\partial x}+i\frac{\partial v}{\partial x}\\
   &=-i\frac{\partial u}{\partial y}+\frac{\partial v}{\partial y}\\
   &=\frac{\partial u}{\partial x}-i\frac{\partial u}{\partial y}\\
   &=\frac{\partial v}{\partial y}+i\frac{\partial v}{\partial x}
\end{aligned}
$$

!!!note
    另外：柯西黎曼方程等价于 $\dfrac{\partial f}{\partial \bar{z}}=0$。

    凭直觉来说，这意味着一个不依赖 $\bar{z}$ 的函数应当是解析的，一个解析的函数也不该出现任何的 $x,y,\bar{z}$ 之类的东西。
    
    但是瞪眼法只能观察显式形式，其实并不能确定这个函数到底和 $\bar{z}$ 有没有关系。比如 $f(x)=|z|^2=z\bar{z}$ 就是一个经典诈骗。
    
    还有复变数指数函数
    $$
    \begin{aligned}
        f(z)&=e^x(\cos y+i\sin y)\\
        &=e^{x+iy}=e^z
    \end{aligned}
    $$
    形式上也有 $x$ 和 $y$，但是它在复平面内**处处可导**，**处处解析**。

### 判定方法

1. 如果用求导公式和法则证实 $f(z)$ 导数在区域内处处存在，那么根据定义它是解析的。
2. 偏导连续这个条件比可微更强，而且判定柯西黎曼方程的时候偏导数还是要算。很多时候可微都是用偏导连续直接得到的。

!!!note 例题引出的一些内容
    另一个神人函数 $f(z)=\sqrt{|xy|}$ 在 $z=0$ 处虽然满足柯西黎曼方程，因为在这一点 $u_x=u_y=v_x=v_y=0$，但是这个函数在这一点，不！可！导！（沿着 $y=kx$ 趋于零就会发现 $k$ 无法消去）

    因此需要注意的是，虽然一眼看上去柯西黎曼方程更难满足，实际上 $u$ 和 $v$ 的可微性也不是什么省油的灯，而且**会坑人**。

    此外，显然如果一个解析函数的 $u,v$ 中有一个是常函数，整个解析函数会被锁死成常函数，这是显而易见的，因为柯西黎曼方程会锁定所有偏导数全为0。

    但是，如果 $u$ 是 $v$ 的函数或者反之，这个解析函数也**只能是常函数**：

    不妨假设 $u=F(v)$。那么
    $$
    \frac{\partial v}{\partial x}=F'(u)\frac{\partial u}{\partial x},\quad \frac{\partial v}{\partial y}=F'(u)\frac{\partial u}{\partial y}
    $$
    然后柯西黎曼方程开始发力：
    $$
    \frac{\partial u}{\partial y}=-F'(u)\frac{\partial u}{\partial x},\quad \frac{\partial u}{\partial x}=F'(u)\frac{\partial u}{\partial y}
    $$
    等下，这看着感觉已经只能全为 $0$ 了，但是还不够严谨。所以把第二个式子带进第一个式子里面：
    $$
    \frac{1}{F'(u)} \frac{\partial u}{\partial x} = -F'(u) \frac{\partial u}{\partial x}
    $$
    于是
    $$
    \left[1 + (F'(u))^2\right] \frac{\partial u}{\partial x} = 0
    $$
    左边中括号里的内容必定大于零，那只能 $\dfrac{\partial u}{\partial x}=0$。这个先河一开直接宣告所有偏导归零，函数变成常函数。

    ~~柯西黎曼方程的威力比你想的要逆天~~

!!!note 顺带一提的怪东西
    两条曲线正交的意思是它们**交点处**的**切线互相垂直**。

    然后，对于一个解析函数而言，它的实部等值线族 $u(x,y)=C_1$ 和虚部等值线族 $v(x,y)=C_2$ 是正交的。

    一个很简单的解释是，这两个等值线族在某一点的法向量分别是 $(u_x,u_y)$ 和 $(v_x,v_y)$。而根据柯西黎曼方程，它们两个求内积结果为 $u_xv_x+u_yv_y=u_x(-u_y)+u_y(u_x)=0$。

    如果 $u_y,v_y$ 其一为零，那另一个必不为零。而且就算一个水平，另一个必定铅直，正交是跑不了的。

## 复变数初等函数

### 复变数指数函数

**定义**：曾提到过的
$$
w=f(z)=e^x(\cos y +i\sin y)
$$
往往用 $\exp z$ 或者 $e^z$ 表示。它等价于：
$$
\begin{cases}
    |\exp z|=e^x\\
    \operatorname{Arg}(\exp z)=y+2k\pi
\end{cases}
\quad (k \in \mathbb{Z})
$$

**加法定理**：
$$
\exp z_1 \cdot \exp z_2 = \exp (z_1+z_2)
$$

**周期性**：与实变函数的 $e^x$ 有所不同，它是**有周期**的，周期为 $2k\pi i$，也就是说 $\exp(z+2k\pi i)=\exp z \cdot \exp(2k\pi i)=\exp z$。

### 复变数对数函数

规定满足 $\exp w=z(z \ne 0)$ 的函数 $w=f(z)$ 为对数函数，记为
$$
w=\operatorname{Ln}z=\ln |z|+i\operatorname{Arg}z
$$

因为用到了同为多值函数的 $\operatorname{Arg}$，显然这也是一个多值函数。

所以自然就会有一个单值函数的版本 $\ln z = \ln |z|+i\operatorname{arg}z$，使用单值函数版本的 $\operatorname{arg}$。

!!!note
    注意这里式子左边的 $\ln$ 指的是复变的单值版本，右边的则指的是实变对数函数。

    你可以把它理解为函数重载。

    并且这样定义过后，这个复变版本的 $\ln$ 在 $z=x>0$ 的时候可以退为实变函数的 $\ln$。

在实变函数中，$\ln x(x<0)=\text{NaN}$，而复变版本的 $\operatorname{Ln}$ 和 $\ln$ 是一种推广。

**性质**：

1. $\operatorname{Ln}(z_1 \cdot z_2)=\operatorname{Ln}z_1+\operatorname{Ln}z_2$
2. $\operatorname{Ln}\dfrac{z_1}{z_2}=\operatorname{Ln}z_1-\operatorname{Ln}z_2$
3. $\operatorname{Ln}z^n=n\operatorname{Ln}z$ 和 $\operatorname{Ln}\sqrt[n]{z}=\dfrac{1}{n}\operatorname{Ln}z$ **不再成立**，将 $\operatorname{Ln}$ 换为 $\ln$ **也不成立**。
4. $n\operatorname{Ln}z=\overbrace{\operatorname{Ln}z+\cdots+\operatorname{Ln}z}^{n个}$ 也不再成立。这个很有迷惑性，你可以认为 $\operatorname{Ln}$ 函数返回一个包含所有值的集合，因此`operator+`、`operator=`被**重载**为集合的闵可夫斯基加法、集合的相等。

!!!note
    需要注意的是：
    1. 因为 $\operatorname{Ln}$ 依赖于 $\operatorname{Arg}$，所以等式中等号的含义是两侧的集合相等。
    2. 因此，如果尝试将 $\operatorname{Ln}$ 替换为 $\ln$ ，**等号无法成立**。
    3. 以上两条全部是因为幅角的特殊性和周期性，这和处理三角函数问题的时候如出一辙。

**连续性**：
在**除去了负实轴和原点之后的复平面**内，主值**分支**和其他各**分支**处处连续，处处可导。并且
$$
(\ln z)'=\frac{1}{z},\quad (\operatorname{Ln}z)'=\frac{1}{z}
$$

### 乘幂与幂函数

规定对于 $z \ne 0$，复变数幂函数为
$$
w=z^b=\exp(b\operatorname{Ln}z)
$$

规定当 $z=0$ 时，$b$ 应为正实数，并且 $0^b=0$。

显然因为对数函数是多值的且有无穷多个，复变数幂函数也应该有无穷多个值。除非：

1. $b$ 为正整数，这时候有单一值。（可理解为退化成乘方的定义）
2. $b=\dfrac{p}{q}$，其中 $p,q$ 互质，$q>0$。这时候有 $q$ 个值。（可理解为它退化成先乘方再开根，于是遵循几次方根几个值）
3. 当 $p=1,q=n$，这时候退化为 $n$ 次方根。

**解析性**：

1. $z^n$ 在复平面内单值解析，$\left(z^n\right)'=nz^{n-1}$。
2. $z^{\frac{1}{n}}$ 是多值函数，有n个分支，各个分支在**除原点和负实轴的复平面内**解析。
    $$
    \left(z^{\frac{1}{n}}\right)'=\frac{1}{n}z^{\frac{1}{n}-1}
    $$
3. 其他情况下也是多值函数，且 $b$ 不是有理数时无穷多值。它的各个分支在**除原点和负实轴外的复平面内**解析，$\left(z^b\right)'=bz^{b-1}$。

### 三角和双曲函数

根据 $e^{iy}=\cos y+i\sin y,\quad e^{-iy}=\cos y-i\sin y$，将两式相加减，得到
$$
\cos y=\frac{e^{iy}+e^{-iy}}{2},\quad \sin y=\frac{e^{iy}-e^{-iy}}{2i}.
$$

把上面的 $y$ 换成 $z$ 即可把三角函数推广到复数。

显然 $\sin z$ 是奇函数，$\cos z$ 是偶函数。它们的周期都为 $2\pi$。

它们在复平面内都解析。导数公式和实变版本一致：
$$
(\sin z)'=\cos z,\quad (\cos z)'=-\sin z.
$$

当 $z=yi$ 为纯虚数，
$$
\cos yi=\frac{e^{-y}+e^y}{2}=\cosh y,\\
\sin yi=\frac{e^{-y}-e^y}{2i}=i\sinh y.
$$

**正弦函数和余弦函数的几组重要公式**：

$$
\left\{
\begin{array}{l}
\cos(z_{1}+z_{2})=\cos z_{1}\cos z_{2}-\sin z_{1}\sin z_{2}, \\
\sin(z_{1}+z_{2})=\sin z_{1}\cos z_{2}+\cos z_{1}\sin z_{2}, \\
\sin^{2}z+\cos^{2}z=1.
\end{array}
\right.
$$

$$
\left\{
\begin{array}{l}
\cos(x+y i)=\cos x\cosh y-i\sin x\sinh y, \\
\sin(x+y i)=\sin x\cosh y+i\cos x\sinh y.
\end{array}
\right.
$$

当 $y \to \infty,|\sin yi| \to \infty,|\cos yi| \to \infty$。这和实变函数是不一样的。

**双曲函数**：
定义双曲余弦和双曲正弦为
$$
\begin{aligned}
    \cosh z &= \frac{e^z+e^{-z}}{2},\\
    \sinh z &= \frac{e^z-e^{-z}}{2}.
\end{aligned}
$$
当 $z$ 为实数时，又和实变版本的定义一致。

$\sinh z$ 为奇函数，$\cosh z$ 为偶函数。它们的周期都是 $2\pi i$。

导数公式形式和实变的一致：
$$
(\sinh z)'=\cosh z,\quad (\cosh z)'=\sinh z.
$$

并有：
$$
\begin{aligned}
    \cosh y i=\cos y,\quad
    \sinh y i=i \sin y.\\
    \begin{cases}
    \cosh (x+yi)=\cosh x \cos y+i \sinh x \sin y,\\
    \sinh (x+yi)=\sinh x \cos y+i \cosh x \sin y.
    \end{cases}.
\end{aligned}
$$

### 反三角函数和反双曲函数

设 $z=\cos w$，则记作 $w=\operatorname{Arccos} z$。

由 $z=\cos w=\dfrac{e^{iw}+e^{-iw}}{2}$，得 $e^{iw}-2ze^{iw}+1=0$。

于是 $e^{iw}=z+\sqrt{z^2-1}$，取对数得到
$$
\operatorname{Arccos}z=-i\operatorname{Ln}(z+\sqrt{z^2-1}).
$$

同理可得：
$$
\begin{aligned}
    \operatorname{Arcsin}z&=-i\operatorname{Ln}(iz+\sqrt{1-z^2}),\\
    \operatorname{Arctan}z&=-\frac{i}{2}\operatorname{Ln}\frac{1+iz}{1-iz}.
\end{aligned}
$$

反双曲函数的定义：
$$
\begin{aligned}
 \operatorname{Arsinh}z &= \operatorname{Ln}(z + \sqrt{z^{2}+1}) \\
\operatorname{Arcosh}z &= \operatorname{Ln}(z + \sqrt{z^{2} - 1}) \\
\operatorname{Artanh}z &= \dfrac{1}{2}\operatorname{Ln}\dfrac{1 + z}{1 - z}
\end{aligned}
$$

# 复变函数的积分

## 复变函数积分

### 有向曲线

设 $C$ 为平面上给定的一条光滑（或按段光滑）曲线，如果选定 $C$ 的两个可能方向中的一个作为正方向（或正向），那么我们就把 $C$ 理解为带有方向的曲线，称为**有向曲线**。

如果 $A$ 到 $B$ 作为曲线 $C$ 的正向，那么 $B$ 到 $A$ 就是曲线 $C$ 的负向，记为 $C^{-}$.

**简单闭曲线的正向**：
简单闭曲线 $C$ 的正向是指，当曲线上的点 $P$ 顺此方向前进时，邻近 $P$ 点的曲线的内部始终位于 $P$ 点的左方。与之相反的方向就是曲线的负方向。

### 积分定义

设函数 $ w = f(z) $ 定义在区域 $ D $ 内，$ C $ 为区域 $ D $ 内起点为 $ A $ 终点为 $ B $ 的一条光滑的有向曲线。把曲线 $ C $ 任意分成 $ n $ 个弧段，设分点为  
$$
A = z_0, z_1, \cdots, z_{k-1}, z_k, \cdots, z_n = B,
$$
在每个弧段 $\widehat{z_{k-1}z_k}\quad (k = 1, 2, \dots, n )$ 上任意取一点 $\zeta_k$。

作和式
$$
S_{n} = \sum_{k=1}^{n} f(\zeta_{k}) \cdot (z_{k} - z_{k-1}) = \sum_{k=1}^{n} f(\zeta_{k}) \cdot \Delta z_{k},
$$
这里 $\Delta z_{k} = z_{k} - z_{k-1}$，$\Delta s_{k}$ 为弧段 $z_{k-1}z_{k}$ 的长度，记 $\delta = \max\limits_{1 \leq k \leq n} \{\Delta s_{k}\}$.
当 $n$ 无限增加且 $\delta \to 0$ 时，如果不论对 $C$ 的分法及 $\zeta_{k}$ 的取法如何，$S_{n}$ 有唯一极限，那么称这极限值为函数 $f(z)$ 沿曲线 $C$ 的积分，记为
$$
\int_{C} f(z)dz=\lim_{\delta \to 0}\sum^n_{k=1}f(\zeta_k)\cdot \Delta z_k.
$$

### 积分存在的条件和计算法

**存在的条件**：
如果 $f(z)$ 是连续函数，而 $C$ 是光滑曲线，则 $\int_C f(z)dz$一定存在。

$\int_C f(z)dz=\int_C udx-vdy+i\int_C vdx+udy$.

**积分的计算法**：
可以通过两个二元实变函数的线积分来计算。
$$
\begin{aligned}
\int_C f(z) \, dz
&= \int_\alpha^\beta \left\{ u[x(t), y(t)] x'(t) - v[x(t), y(t)] y'(t) \right\} \, dt \\
&\quad + i \int_\alpha^\beta \left\{ v[x(t), y(t)] x'(t) + u[x(t), y(t)] y'(t) \right\} \, dt \\
&= \int_\alpha^\beta \left\{ u[x(t), y(t)] + i v[x(t), y(t)] \right\} \left\{ x'(t) + i y'(t) \right\} \, dt \\
&= \boxed{\int_\alpha^\beta f[z(t)] z'(t) \, dt}
\end{aligned}
$$

!!!note
    就是把参数方程的复数形式直接带进去。

    于是这变成了一个实参数 $t$ 的定积分，唯一的不同就是被积函数是复变的了。

如果 $C$ 是 $C_1,C_2,\cdots,C_n$ 等光滑曲线连接成的按段光滑曲线，则
$$
\int_{C} f(z)\mathrm{d} z=\int_{C_{1}} f(z)\mathrm{d} z+\int_{C_{2}} f(z)\mathrm{d} z+\cdots+\int_{C_{n}} f(z)\mathrm{d} z.
$$

## 10.13

### 积分的性质

复积分与实变函数的定积分有类似的性质。

1. **反向路径性质**
$$ \int_{C} f(z)dz=-\int_{C^{-}}f(z)dz $$

2. **常数倍性质**
$$ \int_{C} kf(z)dz=k\int_{C} f(z)dz \quad (k为常数) $$

3. **线性性质**
$$ \int_{C}[f(z)\pm g(z)]dz=\int_{C}f(z)dz\pm \int_{C}g(z)dz $$

4. **估值定理**

    设曲线 $C$ 的长度为 $L$, 函数 $f(z)$ 在 $C$ 上满足 $ \left |f(z)\right |\leq M $, 那么
    $$ \left|\int_{C}f(z)dz\right|\leq\int_{C}\left |f(z)\right | ds\leq ML $$

### 柯西-古萨基本定理

如果一个复变函数 $ f(z) $ 在一个**单连通区域** $ D $ 内是**解析**的，那么 $ f(z) $ 沿 $ D $ 内任意一条**简单闭合曲线** $ C $ 的积分都等于零。

!!!note
    1. 这里的 $C$ 可以不是简单曲线。
    2. 这个定理也成为柯西积分定理。

### 基本定理的推广

#### 复合闭路定理

1. 闭路变形原理

    设 $C_{1}$ 与 $C_{2}$ 是两条简单闭曲线，$C_{2}$ 在 $C_{1}$ 的内部，$f(z)$ 在 $C_{1}$ 与 $C_{2}$ 所围的多连通域 $D$ 内解析，而在 $D + C_{1} + C_{2}$ 上连续，则
    $$ \int_{C_{1}} f(z) \, dz = \int_{C_{2}} f(z) \, dz. $$

    !!!note
        **注**：如果我们把如上两条简单闭曲线 $C_{1}$ 及 $C_{2}^{-}$ 看成一条复合闭路 $\Gamma$，而且它的正向为：外面的闭曲线 $C_{1}$ 按逆时针进行，里面的闭曲线 $C_{2}$ 按顺时针进行（即沿 $\Gamma$ 的正向进行时，$\Gamma$ 的内部总在 $\Gamma$ 的左手边），那么
        $$
        \oint_{\Gamma} f(z) \, dz = 0.
        $$
        该定理说明，在区域内的一个解析函数沿闭曲线的积分，不因闭曲线在区域内作连续变形而改变它的值，只要在变形过程中曲线**不经过**函数 $f(z)$ **不解析**的点。
2. 复合闭路定理

    设 $C$ 为多连通域 $D$ 内的一条简单闭曲线，$C_1, C_2, \ldots, C_n$ 是在 $C$ 内部的简单闭曲线，它们互不包含也互不相交，并且以 $C, C_1, C_2, \ldots, C_n$ 为边界的区域全含于 $D$。如果 $f(z)$ 在 $D$ 内解析，那么
    $$
    \oint_{C} f(z) \, dz = \sum_{k=1}^{n} \oint_{C_k} f(z) \, dz,
    $$
    其中 $C$ 及 $C_k$ ($k = 1, 2, \ldots, n$) 均取正方向；

    或
    $$
    \oint_{\Gamma} f(z) \, dz = 0.
    $$
    其中 $\Gamma$ 为由 $C$ 及 $C_k$ ($k = 1, 2, \cdots, n$) 所组成的复合闭路（其方向是：$C$ 按逆时针进行，$C_k$ ($k = 1, 2, \cdots, n$) 按顺时针进行）。

### 柯西积分公式

设 $f(z)$ 在区域 $D$ 内处处解析，$C$ 为 $D$ 内的任何一条正向简单闭曲线，它的内部完全含于 $D$，$z_0$ 为 $C$ 内的任一点，那么

$$
f(z_{0}) = \frac{1}{2\pi i} \oint_{C} \frac{f(z)}{z - z_{0}} \, dz.
$$

!!!note 说明
    1. 把函数在 $C$ 内部任一点的值用它在边界上的值表示。（这是解析函数的又一特征）

    2. 公式不但提供了计算某些复变函数沿闭路积分的一种方法，而且给出了解析函数的一个积分表达式。（这是研究解析函数的有力工具）

    3. 一个解析函数在圆心处的值等于它在圆周上的平均值。即，如果 $C$ 是圆周 $z = z_{0} + R \cdot e^{i\theta}$，则有：
    $$
    f(z_{0}) = \frac{1}{2\pi} \int_{0}^{2\pi} f(z_{0} + R \cdot e^{i\theta}) \, d\theta
    $$

### 高阶导数公式

设函数 $ f(z) $ 在区域 $ D $ 内解析，$ C $ 为 $ D $ 内任意一条包含点 $ z_0 $ 的简单正向闭曲线，且 $ C $ 及其内部完全包含于 $ D $，则 $ f(z) $ 的各阶导数均存在，且 $ f(z) $ 在点 $ z_0 $ 处的 $ n $ 阶导数为：

$$
f^{(n)}(z_0) = \frac{n!}{2\pi i} \oint_{C} \frac{f(z)}{(z - z_0)^{n+1}}  dz \quad (n = 1, 2, \cdots)
$$

## 原函数和不定积分

### 定理

**定理一**  
如果 $f(z)$ 在单连通域内解析，则**积分与路径无关**。

**定理二**  
如果 $f(z)$ 在单连通域 $B$ 内解析，则 $F(z)=\int_{z_0}^{z}f(\zeta)d\zeta$ 必为 $B$ 内一个解析函数，使得 $F'(z)=f(z)$。

!!!note
    这和微积分中对变上限积分的求导定理差不多。

### 原函数的定义

如果函数 $\varphi(z)$ 在区域 $B$ 内的导数为 $f(z)$，即 $\varphi^{\prime}(z)=f(z)$，那么称 $\varphi(z)$ 为 $f(z)$ 在区域 $B$ 内的原函数。

显然 $F(z)=\int_{z_0}^{z}f(\zeta)d\zeta$ 是 $f(z)$ 的一个原函数。

### 原函数之间的关系

$f(z)$ 的任何两个原函数相差一个常数。

### 不定积分的定义

称 $f(z)$ 的原函数的一般表达式 $F(z)+c$（$c$ 为任意常数）为 $f(z)$ 的不定积分，记作

$$
\int f(z)dz=F(z)+c.
$$

**定理三**（类似于牛顿-莱布尼兹公式）

如果函数 $f(z)$ 在单连通域 $B$ 内处处解析，$G(z)$ 为 $f(z)$ 的一个原函数，那么

$$
\int_{z_0}^{z_1} f(z)dz=G(z_1)-G(z_0)
$$

这里 $z_0, z_1$ 为域 $B$ 内的两点。

!!!note Morera定理
    若函数 $f(z)$ 在单连通区域 $D$ 内连续，且对 $D$ 内任一条逐段光滑的简单闭曲线 $C$，都有

    $$
    \oint_C f(z) \, dz = 0,
    $$

    则函数 $f(z)$ 在区域 $D$ 内解析。

## 解析函数和调和函数

### 调和函数

如果二元实变函数 $\varphi(x,y)$ 在区域 $D$ 内具有二阶连续偏导数，并且满足拉普拉斯方程

$$
\frac{\partial^{2}\varphi}{\partial x^{2}} + \frac{\partial^{2}\varphi}{\partial y^{2}} = 0,
$$

那么称 $\varphi(x,y)$ 为区域 $D$ 内的**调和函数**。

### 解析函数和调和函数的关系

**定理：**  
任何在区域 $D$ 内解析的函数，它的实部和虚部都是 $D$ 内的调和函数。

### 共轭调和函数

设 $u(x,y)$ 为区域 $D$ 内给定的调和函数，我们把使 $u+iv$ 在 $D$ 内构成解析函数的调和函数 $v(x,y)$ 称为 $u(x，y)$ 的共轭调和函数。

换句话说，在 $D$ 内满足方程 $\frac{\partial u}{\partial x} = \frac{\partial v}{\partial y}$, $\frac{\partial u}{\partial y} = -\frac{\partial v}{\partial x}$ 的两个调和函数中，$v$ 称为 $u$ 的共轭调和函数。

### 偏积分法

如果已知一个调和函数 $u$，那么就可以利用**柯西黎曼方程**求得它的共轭调和函数，从而构成一个解析函数 $u+vi$。这种方法称为**偏积分法**。

### 不定积分法

已知调和函数 $u(x，y)$ 或 $v(x，y)$，用不定积分求解析函数的方法称为不定积分法。

# 级数

## 复数项级数

### 复数列的极限

设 $\{\alpha_n\} (n=1,2,\cdots)$ 为一复数列，其中 $\alpha_n = a_n + ib_n$，又设 $\alpha = a + ib$ 为一确定的复数。如果任意给定 $\varepsilon > 0$，相应地都能找到一个正数 $N(\varepsilon)$，使 $|\alpha_n - \alpha| < \varepsilon$ 在 $n > N$ 时成立，那么 $\alpha$ 称为复数列 $\{\alpha_n\}$ 当 $n \to \infty$ 时的极限，记作
$$\lim_{n \to \infty} \alpha_n = \alpha$$
此时也称复数列 $\{\alpha_n\}$ 收敛于 $\alpha$。

!!!note
    复数列收敛的充要条件是
    $$
    \boxed{\lim_{n\to \infty}a_n=a,\quad \lim_{n\to \infty}b_n=b.}
    $$
    也就是说，复数列的敛散性可以转化为两个实数列的敛散性。

### 级数的概念

#### 级数定义

设 $\{\alpha_n\} = \{a_n + ib_n\} (n=1,2,\cdots)$ 为一复数列，表达式

$$
\sum_{n=1}^{\infty} \alpha_n = \alpha_1 + \alpha_2 + \cdots + \alpha_n + \cdots
$$

称为**复数项无穷级数**。其最前面 $n$ 项的和

$$
s_n = \alpha_1 + \alpha_2 + \cdots + \alpha_n
$$

称为级数的**部分和**。

#### 收敛与发散

如果部分和数列 $ \{s_{n}\} $ 收敛，那么级数 $ \sum\limits_{n=1}^{\infty}\alpha_{n} $ 收敛，并且极限 $ \lim\limits_{n\to\infty}s_{n}=s $ 称为级数的和。

如果部分和数列 $ \{s_{n}\} $ 不收敛，那么级数 $ \sum\limits_{n=1}^{\infty}\alpha_{n} $ 发散。

#### 收敛的条件

级数 $ \sum\limits_{n=1}^{\infty} \alpha_n = \sum\limits_{n=1}^{\infty} (a_n + i b_n) $ 收敛的充要条件是：级数 $ \sum\limits_{n=1}^{\infty} a_n $ 和 $ \sum\limits_{n=1}^{\infty} b_n $ 都收敛。

!!!note 必要条件
    因为实数项级数$ \sum\limits_{n=1}^{\infty} a_{n} $和$ \sum\limits_{n=1}^{\infty} b_{n} $收敛的必要条件是$ \lim\limits_{n\to\infty} a_{n}=0 $和$ \lim\limits_{n\to\infty}b_{n}=0 $。

    所以复数项级数$ \sum\limits_{n=1}^{\infty} \alpha_{n} $收敛的必要条件是

    $$
    \boxed{\lim\limits_{n\to\infty} \alpha_{n}=0}
    $$

!!!tip
    判别级数的敛散性时，可先考察$ \lim\limits_{n \to \infty} \alpha_n \not= 0 $

    $$
    \text{如果}\begin{cases}
    \lim\limits_{n \to \infty} \alpha_n \neq 0, & \text{级数发散} \\
    \lim\limits_{n \to \infty} \alpha_n = 0, & \text{应进一步判断}
    \end{cases}
    $$

#### 绝对收敛和条件收敛

如果 $\sum\limits_{n=1}^{\infty} \left| \alpha_n \right|$ 收敛，那么 $\sum\limits_{n=1}^{\infty} \alpha_n$ 也收敛。

且不等式 $\left| \sum\limits_{n=1}^{\infty} \alpha_n \right| \le \sum\limits_{n=1}^{\infty} \left| \alpha_n \right|$ 成立。

!!!info 注意
    $\sum\limits_{n=1}^{\infty} \left| \alpha_n \right|$ 的各项都是非负的实数，应用正项级数的审敛法则判定。

**定义**  
如果 $ \sum\limits_{n=1}^{\infty}|\alpha_{n}| $ 收敛，那末称级数 $ \sum\limits_{n=1}^{\infty}\alpha_{n} $ 为**绝对收敛**。

非绝对收敛的收敛级数称为**条件收敛级数**。

!!!note 说明
    由 $ |\alpha_{n}|=\sqrt{a_{n}^{2}+b_{n}^{2}}\leq|a_{n}|+|b_{n}| $，

    所以 $ \sum\limits_{n=1}^{\infty}a_{n} $ 与 $ \sum\limits_{n=1}^{\infty}b_{n} $ 绝对收敛时，$ \sum\limits_{n=1}^{\infty}\alpha_{n} $ 也绝对收敛。

    综上：
    $$
    \boxed{\sum\limits_{n=1}^{\infty}\alpha_{n} \text{绝对收敛} \Leftrightarrow\sum\limits_{n=1}^{\infty}a_{n} \text{与} \sum\limits_{n=1}^{\infty}b_{n} \text{绝对收敛}}
    $$

## 幂级数

### 复变函数项级数、部分和

设 $\{f_n(z)\}(n=1,2,\ldots)$ 为一复变函数序列，其中各项在区域 $D$ 内有定义。表达式
$$
\sum_{n=1}^{\infty} f_n(z) = f_1(z) + f_2(z) + \cdots + f_n(z) + \cdots
$$
称为复变函数项级数，记作 $\sum_{n=1}^{\infty}f_{n}(z)$。
级数最前面n项的和
$$
s_{n}(z)=f_{1}(z)+f_{2}(z)+\cdots +f_{n}(z)
$$
称为这级数的**部分和**。

### 和函数

如果对于 $D$ 内的某一点 $z_0$，若 $\sum\limits_{n=1}^{\infty} f_n(z_0)$ 收敛，那末称级数 $\sum\limits_{n=1}^{\infty} f_n(z)$ 在 $z_0$ 收敛。其和记为 $S(z_0)$。

如果级数在 $D$ 内处处收敛，那末它的和一定是 $z$ 的一个函数 $s(z)$：

$$ s(z) = f_1(z) + f_2(z) + \cdots + f_n(z) + \cdots $$

称为该级数在区域 $D$ 上的**和函数**。

### 幂级数概念

当 $f_n(z) = c_{n-1}(z-a)^{n-1}$ 或 $f_n(z) = c_{n-1}z^{n-1}$ 时，得到函数项级数的特殊情形：
$$
\sum_{n=0}^{\infty} c_n (z-a)^n = c_0 + c_1(z-a) + c_2(z-a)^2 + \cdots + c_n(z-a)^n + \cdots
$$
或

$$
\sum_{n=0}^{\infty} c_n z^n = c_0 + c_1 z + c_2 z^2 + \cdots + c_n z^n + \cdots
$$
这种级数称为幂级数。​

### 敛散性

#### 收敛定理（Abel定理）

如果级数 $\sum_{n=0}^{\infty} c_{n} z^{n}$ 在 $z = z_{0} (\neq 0)$ 处收敛，那么对满足 $|z| < |z_{0}|$ 的 $z$，级数必**绝对收敛**。

如果在 $z = z_{0}$ 处级数发散，那么对满足 $|z| > |z_{0}|$ 的 $z$，级数必**发散**。

#### 收敛圆与收敛半径

对于一个幕级数，其收敛半径的情况有三种：

1. 对所有的正实数都收敛。由阿贝尔定理知：**级数在复平面内处处绝对收敛**。
2. 对所有的正实数，除了 $z=0$ 之外都发散。此时，**级数在复平面内除了原点之外处处发散**。

    !!! example
        对于 $1+z+2^2z^2+\cdots+n^nz^n$ 这个级数，当 $z \ne 0$ 时，通项是**不趋于零**的，级数发散。

3. 同时存在使得级数发散和收敛的正实数。这时，幂级数 $\sum\limits _{n=0}^{\infty}c_nz^n$ 的收敛范围是一个以原点为中心的圆域。

#### 收敛半径的求法

##### 比值法

$$
\boxed{
    \text{如果} \lim_{n \to \infty} \left|\frac{c_{n+1}}{c_n}\right| = \lambda \ne 0, \quad \text{则收敛半径} R=\frac{1}{\lambda}.
}
$$

!!!info 注意
    如果：
       1. $\lambda = 0$，则级数 $\sum\limits _{n=0}^{\infty}c_n z^n$ 在复平面内处处收敛，即 $\boxed{R=\infty}$。
       2. $\lambda = \infty$（极限不存在），则级数 $\sum\limits _{n=0}^{\infty}c_n z^n$ 对于复平面内除 $n=0$ 外的一切 $z$ 均发散，也就是 $\boxed{R=0}$。

##### 根植法

$$
\boxed{
    \text{如果} \lim_{n \to \infty} \sqrt[n]{|c_n|} = \lambda \ne 0, \quad \text{则收敛半径} R = \frac{1}{\lambda}.
}
$$
注意事项和比值法一致。

### 幂级数的运算和性质

#### 有理运算

设
$$
f(z)=\sum_{n=0}^{\infty} a_{n}z^{n},\quad R=r_{1},\qquad g(z)=\sum_{n=0}^{\infty} b_{n}z^{n},\quad R=r_{2}.
$$

则有：
$$
\begin{aligned}
    f(z)\pm g(z)&=\sum_{n=0}^{\infty} a_{n}z^{n}\pm\sum_{n=0}^{\infty} b_{n}z^{n}\\
    &=\sum_{n=0}^{\infty}(a_{n}\pm b_{n})z^{n}.\\
    & (R=\min(r_{1},r_{2}), \quad |z| < R)\\
    \\
    f(z)\cdot g(z)&=\left(\sum_{n=0}^{\infty} a_{n}z^{n}\right)\cdot\left(\sum_{n=0}^{\infty} b_{n}z^{n}\right)\\
    &=\sum_{n=0}^{\infty}\left(a_{n}b_{0}+a_{n-1}b_{1}+\cdots+a_{0} b_{n}\right)z^{n}.\\
    & (R=\min(r_{1},r_{2}), \quad |z| < R)
\end{aligned}
$$

#### 代换（复合）运算

**定理**：
如果当 $|z|<r$ 时，$f(z)=\sum\limits _{n=0}^{\infty} a_{n}z^{n}$，又设在 $|z|<R$ 内 $g(z)$ 解析且满足 $|g(z)|<r$，那末当 $|z|<R$ 时，$f[g(z)]=\sum\limits_{n=0}^{\infty} a_{n}[g(z)]^{n}$。

!!! note 说明
    此代换运算常应用于将函数展开成幂级数。

#### 复变幂函数在收敛圆内的性质

**定理**
设幂级数 $\sum\limits_{n=0}^{\infty} c_{n}(z-a)^{n}$ 的收敛半径为 $R$，则

1. 它的和函数 $f(z) = \sum\limits_{n=0}^{\infty} c_{n}(z-a)^{n}$ 是收敛圆 $|z-a| < R$ 内的解析函数。
2. $f(z)$ 在收敛圆 $|z-a| < R$ 内的导数可将其幂级数逐项求导得到，即
    $$
    f'(z) = \sum_{n=1}^{\infty} n c_{n}(z-a)^{n-1}.
    $$
3. 在收敛圆内可以逐项积分，也就是
    $$
    \int\limits _c f(z)\mathrm{d}z = \sum _{n=0}^{\infty} c_n\int\limits _c (z-a)^n \mathrm{d}z, \quad c \subset \{ z | \left| z-a \right| < R \}.
    $$
    或
    $$
    \int _a^z f(\zeta)\mathrm{d}z = \sum _{n=0}^{\infty}\frac{c_n}{n+1}(z-a)^{n+1}.
    $$

!!! note
    简而言之，在收敛圆内，幂函数的**和函数解析**；幂函数可以**逐项求导**或者**逐项积分**。

# 留数

## 孤立奇点

prompt：把图片中的内容转为markdown，包裹在代码块中发送给我，注意不要添加额外的内容，公式用美元符号而不是反斜线括号的风格。

### 孤立奇点的概念

如果函数 $f(z)$ 在 $z_0$ 不解析, 但 $f(z)$ 在 $z_0$
的某一去心邻域 $0 < |z - z_0| < \delta$ 内处处解析, 则称
$z_0$ 为 $f(z)$ 的孤立奇点.

### 孤立奇点的分类

#### 可去奇点

如果洛朗级数中不含有 $z-z_0$ 的负幂项，则孤立奇点 $z_0$称为 $f(z)$ 的可去奇点。

!!!note
    1. $z_0$ 是 $f(z)$ 的可去奇点，而
    $$
    f(z)=c_0+c_1(z-z_0)+\cdots+c_n(z-z_0)^n+\cdots\quad(0<\left|z-z_0\right|<\delta)
    $$
    则和函数 $F(z)$ 在 $z_0$ 解析。
    2. 无论 $f(z)$ 在 $z_0$ 是否有定义，补充 $f(z_0)=c_0$ 则 $f(z)$ 在 $z_0$ 解析。
    $$
    f(z_{0})=\lim _{z\rightarrow z_{0}}f(z)\qquad
    f(z)=\begin{cases}
    F(z), & z\neq z_{0} \\
    c_{0}, & z=z_{0}
    \end{cases}
    $$

    可以证明，若 $\lim _{z\rightarrow z_{0}}f(z)$ 的极限存在为有限值，则 $z_{0}$ 是可去奇点。

!!!tip 判定方法
    1. **由定义判断**：  
        如果 $f(z)$ 在 $z_{0}$ 的洛朗级数无负幂项则 $z_{0}$ 为 $f(z)$ 的可去奇点。
    2. **判断极限** $\lim_{z\to z_{0}}f(z)$：  
        若极限存在且为有限值，则 $z_{0}$ 为 $f(z)$ 的可去奇点。

#### 极点

##### 极点定义

如果洛朗级数中只有有限多个 $z-z_{0}$ 的负幂项，其中关于 $(z-z_{0})^{-1}$ 的最高幂为 $(z-z_{0})^{-m}$，即 $f(z)=c_{-m}(z-z_{0})^{-m}+\cdots+c_{-2}(z-z_{0})^{-2}+c_{-1}(z-z_{0})^{-1}+c_{0}+c_{1}(z-z_{0})+\cdots$ (m $\geqslant 1$, $c_{-m}\neq 0$)，或

$$ f(z)=\frac{1}{(z-z_{0})^{m}}g(z) $$

则孤立奇点 $z_{0}$ 称为函数 $f(z)$ 的 $m$ 级极点。

!!!note 说明
    1. $$ g(z)=c_{-m}+c_{-m+1}(z-z_{0})+c_{-m+2}(z-z_{0})^{2}+\cdots $$
    特点：
       1. 在 $|z-z_{0}|<\delta$ 内是解析函数
       2. $g(z_{0})\neq 0$

    2. 如果 $z_{0}$ 为函数 $f(z)$ 的极点，则

    $$ \lim_{z\to z_{0}}f(z)=\infty. $$

##### 极点判定方法

1. **由定义判别**

    $f(z)$ 的洛朗展开式中含有 $z-z_{0}$ 的负幂项为有限项。

2. **由定义的等价形式判别**

    在点 $z_{0}$ 的某去心邻域内 $f(z)=\dfrac{g(z)}{(z-z_{0})^{m}}$，其中 $g(z)$ 在 $z_{0}$ 的邻域内解析，且 $g(z_{0})\neq 0$。

3. **利用极限** $\lim\limits _{z\to z_{0}}f(z)=\infty$ 判断。

#### 本性奇点

**定义**：
如果洛朗级数中**含有无穷多个** $z-z_{0}$ 的负幂项，则孤立奇点 $z_{0}$ 称为 $f(z)$ 的本性奇点。

!!!example
    例如
    $$
    e^{\frac{1}{z}}=\underbrace{1+z^{-1}+\frac{1}{2!}z^{-2}+\cdots+\frac{1}{n!}z^{-n}+\cdots}_\text{含有\textbf{无穷多个} $z$ 的负幂项}\quad(0< |z| <\infty)
    $$

    所以 $z=0$ 为本性奇点，同时 $\lim\limits_{z\to 0}e^{\frac{1}{z}}$ 不存在。

!!!note 特点
    在本性奇点的邻域内 $\lim\limits_{z\to z_{0}}f(z)$ 不存在且不为 $\infty$。

#### 总结

| 孤立奇点 | 洛朗级数特点 | $\lim_{z \to z_{0}} f(z)$ |
| :---: | :--- | :---: |
| 可去奇点 | 无负幂项 | 存在且为有限值 |
| $m$级极点 | 含有限个负幂项，关于 $(z-z_{0})^{-1}$ 的最高幂为 $(z-z_{0})^{-m}$ | $\infty$ |
| 本性奇点 | 含无穷多个负幂项 | 不存在且不为 $\infty$ |

### 函数的零点和极点的关系

#### 零点定义

不恒等于零的解析函数 $f(z)$ 如果能表示成

$$ f(z) = (z - z_{0})^{m} \varphi(z) $$

其中 $\varphi(z)$ 在 $z_{0}$ 解析且 $\varphi(z_{0}) \neq 0$，$m$ 为某一正整数，则 $z_{0}$ 称为 $f(z)$ 的 $m$ 级**零点**。

#### 零点判定

如果 $f(z)$ 在 $z_{0}$ 解析，则 $z_{0}$ 为 $f(z)$ 的 $m$ 级零点的充要条件是

$f^{(n)}(z_{0})=0$，$(n=0,1,2,\cdots m-1)$；$f^{(m)}(z_{0})\neq 0$。

#### 关系定理

如果 $z_0$ 是 $f(z)$ 的 $m$ 级极点，则 $z_0$ 是 $\dfrac{1}{f(z)}$ 的 $m$ 级零点，反之亦然。

!!! info
    这个定理给判断函数的极点提供了一个比较简便的方法。

## 复变函数的留数

### 留数的定义

如果 $z_{0}$ 为函数 $f(z)$ 的一个孤立奇点，则沿在 $z_{0}$ 的某个去心邻域 $0<|z-z_{0}|<R$ 内包含 $z_{0}$ 的任意一条简单闭曲线 $C$ 的积分 $\oint_{C} f(z)dz$ 的值除以 $2\pi i$ 后所得的数称为 $f(z)$ 在 $z_{0}$ 的留数，记作 $\operatorname{Res}[f(z),z_{0}]$。（即 $f(z)$ 在 $z_{0}$ 为中心的圆环域内的洛朗级数中负幂项 $c_{-1}(z-z_{0})^{-1}$ 的系数。）

### 利用留数求积分

#### 留数定理

函数 $f(z)$ 在区域 $D$ 内除有限个孤立奇点 $z_{1},z_{2},\cdots ,z_{n}$ 外处处解析，$C$ 是 $D$ 内包围诸奇点的一条正向简单闭曲线，则

$$ \oint_{C} f(z) \,\mathrm{d}z=2\pi i \sum_{k=1}^{n} \operatorname{Res}\left[f(z), z_k\right]. $$

说明：留数定理将沿封闭曲线 $C$ 积分转化为求被积函数在 $C$ 内各孤立奇点处的留数。

#### 留数的计算方法

1. 如果 $z_{0}$ 为 $f(z)$ 的可去奇点，则 $\operatorname{Res}\left[f(z),z_{0}\right]=0$。

2. 如果 $z_{0}$ 为 $f(z)$ 的本性奇点，则需将 $f(z)$ 展开成洛朗级数求 $c_{-1}$。

3. 如果 $z_{0}$ 为 $f(z)$ 的极点，则有如下计算规则：

   1. 如果 $z_{0}$ 为 $f(z)$ 的一级极点，则
        $$
        \operatorname{Res}\left[f(z),z_{0}\right]=\lim _{z\rightarrow z_{0}}\left(z-z_{0}\right) f(z).
        $$
   2. 如果 $z_{0}$ 为 $f(z)$ 的 $m$ 级极点，则
        $$
        \operatorname{Res}\left[f(z),z_{0}\right]=\frac{1}{(m-1)!}\lim_{z\to z_{0}}\frac{\mathrm{d}^{m-1}}{\mathrm{d}z^{m-1}}\left[(z-z_{0})^{m}f(z)\right].
        $$
   3. 设 $f(z)=\dfrac{P(z)}{Q(z)}$，$P(z)$ 及 $Q(z)$ 在 $z_{0}$ 都解析，如果 $P(z_{0})\neq 0$，$Q(z_{0})=0$，$Q^{\prime}(z_{0})\neq 0$，则 $z_{0}$ 为 $f(z)$ 的一级极点，且有
        $$
        \operatorname{Res}[f(z),z_{0}]=\dfrac{P(z_{0})}{Q^{\prime}(z_{0})}.
        $$

#### 简单闭曲线上的复积分计算方法

1. 若闭曲线**内部无奇点**，积分为 $0$。
2. 若闭曲线内部**有一个奇点**，考虑使用柯西积分公式或者高阶导数公式。
3. 若闭曲线内部**有多个奇点**，用复合闭路定理转化为上一个情况。
4. 用**留数定理**计算。

## 留数在定积分计算上的应用

### 形如 $\int_0^{2\pi}R(\cos \theta, \sin \theta)\,\mathrm{d}\theta$ 的积分

思路：$\boxed{\text{定积分}} \rightarrow \boxed{\text{复变函数沿着某条封闭路线的积分}}$

令 $z=e^{i\theta}$，则
$$
z=e^{i\theta} \longrightarrow \,\mathrm{d}z=ie^{i\theta}\,\mathrm{d}\theta \longrightarrow \,\mathrm{d}\theta=\frac{\,\mathrm{d}z}{iz},\\
\sin \theta = \frac{1}{2i}(e^{i\theta}-e^{-i\theta})=\frac{z^2-1}{2iz},
\\[1.5ex]
\cos \theta = \frac{1}{2}(e^{i\theta}+e^{-i\theta})=\frac{z^2+1}{2z}.
$$
当 $\theta$ 历经 $[0,2\pi]$，$z$ 沿着单位圆周 $\left|z\right|=1$ 正方向绕行一周。

$$
\begin{aligned}
    & \int _{0}^{2\pi} R (\cos\theta, \sin\theta)\,\mathrm{d}\theta\\
    =& \oint _{|z| = 1} R \left( \frac{z^2+1}{2z},\frac{z^2-1}{2iz} \right) \,\frac{\mathrm{d}z}{iz}\\
    =& \oint _{|z| = 1} f(z) \,\mathrm{d}z\\
    =& 2\pi i \sum _{k=1}^{n} \operatorname{Res}[f(z),z_k].
\end{aligned}
$$

这里 $f(z) = \dfrac{1}{iz} R\left( \dfrac{z^2+1}{2z}, \dfrac{z^2-1}{2iz} \right)$ 是 $z$ 的有理函数，且在单位圆周上分母不为零，满足留数定理的条件。$z_k$ 是包围在单位圆周内的各个孤立奇点。

### 形如 $\int_{-\infty}^{+\infty}R(x)\,\mathrm{d}x$ 的积分

若有理函数 $R(x)$ 的分母至少比分子高两次，并且分母在实轴上无孤立奇点。

一般设
$$
R(z)=\frac{z^n+a_1z^{n-1}+\cdots+a_n}{z^m+b_1z^{m-1}+\cdots+b_m},\quad m-n \ge 2
$$

!!!info
    这里是单纯的把实变函数的 $x$ 换成了复变函数的 $z$，不涉及任何变形，相当于照抄 $R(x)$ 的形式写出了 $R(z)$。这样一来 $R(z)$ 在实轴上的表现就和 $R(x)$ 是一致的。

先讨论 $\int_{-R}^R R(x)dx$，最后令 $R\to \infty$ 即可。

取 $R$ 适当大，这样 $R(z)$ 所有在上半平面内的极点 $z_k$ 都包在这个积分路线内。

补一条线 $C_R$ 也就是以原点为中心，$R$ 为半径的在上半平面的半圆周。

$C_R$ 和 $[-R,R]$ 一起构成了封闭曲线 $C$，$R(z)$ 在 $C$ 及其内部除去有限孤立奇点之外处处解析。

于是根据留数定理，
$$
\int _{-R}^{R} R(x)\,\mathrm{d}x + \int _{C_R} R(z)\,\mathrm{d}z = 2\pi i \sum \operatorname{Res}[R(z),z_k], \\
\begin{aligned}
    \left|R(z)\right| &= \frac{1}{|z|^{m-n}}\frac{\left|1 + a_1z^{-1} + \cdots + a_nz^{-n}\right|}{\left|1 + b_1z^{-1} + \cdots + b_mz^{-m}\right|}\\
    &\le \frac{1}{|z|^{m-n}}\frac{1 + \left|a_1z^{-1} + \cdots + a_nz^{-n}\right|}{1 - \left|b_1z^{-1} + \cdots + b_mz^{-m}\right|}
\end{aligned}
$$

下面我们的目的是试图证明这个 $\int _{C_R} R(z)\,\mathrm{d}z$ 只要 $z$ 充分大就趋于 $0$，如果成功就可以简化计算。观察到前面那一项 $\dfrac{1}{|z|^{m-n}}$ 是趋于 $0$ 的，那如果后面的那一项能被一个常数压住而不要发散到无穷就可以证明了。

所以我们进行了上面的放缩操作，目的是利用 $|z|$ 足够大的时候 $z$ 的任何负数次幂在 $1$ 面前都可以忽略不计。
随便找一个 $0 < p < 1$，比如 $\dfrac{1}{2}$（当然老师的课件上是 $\frac{1}{10}$，其实随便），当 $|z|$ 充分大的时候，$\left|a_1z^{-1} + \cdots + a_nz^{-n}\right|$ 和 $\left|b_1z^{-1} + \cdots + b_mz^{-m}\right|$ 是肯定可以小于 $p$ 的。再考虑 $m-n > 2$，那一定有
$$
|R(z)| < \frac{1}{|z|^2} \cdot \frac{1+p}{1-p} = \frac{3}{|z|^2},
$$

注意这里的 $3$ 是那个 $\dfrac{1+p}{1-p}$ 算出来的，不是魔法数字。然后喜闻乐见的放缩：
$$
\left|\int_{C_R} R(z)\,\mathrm{d}z \right| \le \int _{C_R} |R(z)|\,\mathrm{d}s \le \frac{3}{R^2} \pi R = \frac{3\pi}{R}.
$$

这样一搞，这个常数是多少根本不重要，只要是个常数，就可以保证 $R \to \infty$ 的时候整个式子趋于 $0$。

于是就得到：
$$
\boxed{
    \int_{-\infty}^{+\infty}R(x)\,\mathrm{d}x=2\pi i \sum \operatorname{Res}[R(z),z_k]
}
$$

### 形如 $\int_{-\infty}^{+\infty}R(x)e^{aix}\,\mathrm{d}x,(a>0)$ 的积分

积分存在要求：
$R(x)$ 是 $x$ 的有理函数，且分母的次数至少比分子的次数高一次，而且 $R(x)$ 在**实轴上无孤立奇点**。

和前面一样的是补一条很大的 $C_R$，构成封闭曲线 $C$ 包裹住上半平面的所有极点。

对于 $|z|$ 充分大，而且 $m-n \ge 1$，就会有 $|R(z) < \dfrac{2}{|z|}$。

$$
\left| \int _{C_R} R(z)e^{aiz}\,\mathrm{d}z \right| \le \int _{C_R} |R(z)| \left|e^{aiz}\right| \,\mathrm{d}s < \frac{2}{R} \int _{C_R} \left|e^{ai(x+iy)}\right| \,\mathrm{d}s
$$

令 $x=R\cos \theta,y=R\sin\theta$，则
$$
\,\mathrm{d}s=|\,\mathrm{d}z|=\left|\,\mathrm{d}(Re^{i\theta})\right|=R\,\mathrm{d}\theta,\\
z=R(\cos\theta+i\sin\theta),\quad 0 < \theta < \pi.\\
$$

$$
\begin{aligned}
    \frac{2}{R} \int _{C_R} \left| e^{ai(x+iy)} \right| \,\mathrm{d}s
    &= \frac{2}{R} \int _{C_R} \left| e^{axi} \right|  \left| e^{-ay} \right| \,\mathrm{d}s
    \\
    &= 2 \int _{0}^{\pi} e^{-aR\sin\theta} \,\mathrm{d}\theta
    \\
    &= 4 \int _{0}^{\frac{\pi}{2}} e^{-aR\sin\theta}  \,\mathrm{d}\theta
    \\
    &\le 4 \int _{0}^{\frac{\pi}{2}} e^{-aR(\frac{2\theta}{\pi})} \,\mathrm{d}\theta
    \\
    &= \frac{2 \pi}{aR} (1-e^{-aR}).
\end{aligned}
$$

当 $R \to \infty$，$1-e^{-aR} \to 0$。从而
$$
\int_{C_R} R(z)e^{aiz} \,\mathrm{d}z \to 0.
$$

由留数定理：
$$
\int_{-R}^{+R}R(x)e^{aix}\,\mathrm{d}x + \int_{C_R} R(z)e^{aiz} \,\mathrm{d}z = 2 \pi i \sum \operatorname{Res}[R(z)e^{aiz},z_k].
$$

$R\rightarrow +\infty:$

$$
\int_{-\infty}^{+\infty}R(x)e^{aix}dx = 2\pi i\sum Res[R(z)e^{aiz},z_k] $$
也可以由 $\boxed{e^{iax}=\cos ax + i\sin ax}$ 得到下面的形式：
$$
\int_{-\infty}^{+\infty}R(x)\cos ax\,dx + i\int_{-\infty}^{+\infty}R(x)\sin ax\,dx = 2\pi i\sum Res[R(z)e^{aiz},z_k]
$$

# Laplace 变换

## Laplace 变换概念

### Laplace 变换定义

!!!tip
    这里的虚数单位使用字母 $j$ 代替字母 $i$ 表示，这是因为 Laplace 变换主要服务于工程。工程中字母 $i$ 容易有很多其他含义，所以用 $j$。

设 $f(t)$ 是 $[0,+\infty)$ 上的实/复函数，若对于参数 $s = \beta + j \omega,F(s) = \int _{0}^{+\infty}f(t)e^{-st}\,\mathrm{d}t$ 在 $s$ 平面的某一区域内收敛，则称其为 $f(t)$ 的 Laplace 变换，记为
$$
\mathcal{L}[f(t)] = F(s) = \int _{0}^{+\infty}f(t)e^{-st}\,\mathrm{d}t
$$

这时候 $f(t)$ 就是 $F(s)$ 的 Laplace 逆变换：
$$
f(t) = \mathcal{L}^{-1}[F(s)]
$$

$F(s)$ 称为像函数，$f(t)$ 称为原像函数。

### Laplace 变换的存在定理

若函数f(t)满足：

1. 在 $t \ge 0$ 的任一有限区间上分段连续；

2. 当 $t \to +\infty$ 时，$f(t)$ 的增长速度不超过某一指数函数，即存在常数 $M>0$ 及 $c\ge 0$，使得

$$
|f(t)|\le Me^{ct},0\le t<+\infty.
$$

则 $f(t)$ 的拉氏变换
$$
F(s)=\int_{0}^{+\infty}f(t)e^{-st}dt
$$
在半平面 $\operatorname{Re}(s)>c$ 上一定存在，并且在 $ \operatorname{Re}(s)>c $ 的半平面内，$F(s)$ 为解析函数。

### 常见函数的Laplace变换

1. 单位阶跃函数
    $$
    \mathcal{L}[u(t)] = \frac{1}{s} \quad (\operatorname{Re}(s) > 0)
    $$
2. 指数函数
    $$
    \mathcal{L}[e^{kt}] = \frac{1}{s - k} \quad (\operatorname{Re}(s) > k)
    $$
3. 正弦函数
    $$
    \mathcal{L}[\sin kt] = \frac{k}{s^{2} + k^{2}} \quad (\operatorname{Re}(s) > 0)
    $$
4. 余弦函数
    $$
    \mathcal{L}[\cos kt] = \frac{s}{s^{2} + k^{2}} \quad (\operatorname{Re}(s) > 0)
    $$
5. 幂函数
    $$
    \mathcal{L}[t^{m}] = \frac{m!}{s^{m+1}} \quad m \in Z^{+}, (\operatorname{Re}(s) > 0)
    $$
6. 单位脉冲函数 $\delta(t)$
    $$
    H(t)=
    \begin{cases}
        1, & t=0\\
        0, & t \ne 0
    \end{cases}
    \\[1ex]
    \delta(t)=H'(t).
    $$

    !!! note $\delta(t)$ 的性质
        $$
        \int _{-\infty}^{+\infty} \delta(t) \,\mathrm{d}t = 1. \quad \int _{-\infty}^{+\infty} \delta(t)f(t) \mathrm{d}t = f(0)
        \\[1ex]
        \int _{-\infty}^{+\infty} \delta(t-t_0)f(t) \,\mathrm{d}t = f(t_0)
        \\[1ex]
        \mathcal{L}[\delta(t)]=\int _{0^{-}}^{+\infty}\delta(t)e^{-st} \,\mathrm{d}t=\int _{-\infty}^{+\infty} \delta(t)e^{-st} \,\mathrm{d}t = 1
        \\[1ex]
        \mathcal{L}[\delta(t)]=1.
        $$
7. 周期函数 $f(t)=f(t+T)$
    $$
    \begin{aligned}
        \mathcal{L}[f(t)]
        &= \int _0^T f(t)e^{-st}\,\mathrm{d}t + \cdots + \int _{kT}^{(k+1)T} f(t)e^{-st}\,\mathrm{d}t + \cdots
        \\[1ex]
        &= \int _0^T f(t)e^{-st}\,\mathrm{d}t + \cdots + e^{-skT} \int _0^T f(t)e^{-st}\,\mathrm{d}t + \cdots
        \\[1ex]
        &= \boxed{\frac{1}{1-e^{-sT}} \int _0^T f(t)e^{-st}\,\mathrm{d}t,\quad \operatorname{Re}(s) > 0}
    \end{aligned}
    $$

## Laplace 变换性质

### 线性性质

$\mathcal{L}[f_{i}(t)]=F_{i}(s)\,(i=1,2)$，则
$$
\mathcal{L}[a_{1} f_{1}(t)+a_{2} f_{2}(t)]=a_{1} F_{1}(s)+a_{2} F_{2}(s),
\\[1ex]
\mathcal{L}^{-1}[b_{1} F_{1}(s)+b_{2} F_{2}(s)]=b_{1} f_{1}(t)+b_{2} f_{2}(t).
$$

### 微分性质

$\mathcal{L}[f(t)]=F(s)，(\operatorname{Re}s > c)$，则
$$
\begin{aligned}
    \mathcal{L}[f'(t)] &= sF(s)-f(0)
    \\[1ex]
    \mathcal{L} \left[ f^{(n)}(t) \right] &=s^n F(s) - s^{n-1} f(0) - s^{n-2} f'(0) - \cdots - f^{(n-1)}(0)
\end{aligned}
$$
其中 $(n=1,2,\cdots；\operatorname{Re}s > c)$。

特别地，当 $f(0) = f'(0) = \cdots = f^{(n)}(0) = 0$ 时，
$$
\mathcal{L}\left[ f^{(n)}(t) \right]=s^n F(s)
$$

!!!note 像函数微分性质
    $$
    \begin{aligned}
        \mathcal{L}[(-t)f(t)]&=F^{\prime}(s)
        \\[1ex]
        \mathcal{L}^{-1}[F^{\prime}(s)]&=(-t)f(t)\quad(\operatorname{Re} s>c).
        \\[1ex]
        \mathcal{L}\left[(-t)^{n} f(t)\right]&=F^{(n)}(s),
        \\[1ex]
        \mathcal{L}^{-1}\left[F^{(n)}(s)\right]&=(-t)^{n}f(t).
    \end{aligned}
    $$

### 积分性质

$\mathcal{L}[f(t)]=F(s)，(\operatorname{Re}s > c)$，则
$$
\mathcal{L}\left[\int_{0}^{t} f(t) d t\right]=\frac{F(s)}{s}\quad\left(\operatorname{Re} s>\max (0, c)\right)
\\[1ex]
\mathcal{L}\left[\underbrace{\int_{0}^{t} \mathrm{d} t \int_{0}^{t} \mathrm{d} t \cdots \int_{0}^{t} f(t) \,\mathrm{d} t}_{n \text{次}}\right]=\frac{1}{s^{n}} F(s)
$$

!!!note 像函数积分性质
    已知 $\mathcal{L}[f(t)] = F(s)$，则有：
    $$
    \begin{align*}
    \int_{s}^{\infty} F(s)  \mathrm{d} s &= \int_{s}^{\infty} \left[ \int_{0}^{+\infty} f(t) \mathrm{e}^{-\mu t}  \mathrm{d} t \right] \mathrm{d} \mu \\
    &= \int_{0}^{+\infty} f(t) \left[ \int_{s}^{\infty} \mathrm{e}^{-\mu t}  \mathrm{d} \mu \right] \mathrm{d} t \\
    &= \int_{0}^{+\infty} f(t) \left( \left. \frac{-1}{t} \mathrm{e}^{-\mu t} \right|_{s}^{\infty} \right) \mathrm{d} t \\
    &= \int_{0}^{+\infty} \frac{f(t)}{t} \mathrm{e}^{-s t}  \mathrm{d} t \\
    &= \mathcal{L} \left[ \frac{f(t)}{t} \right]
    \end{align*}
    $$
    **结论：**
    $$
    \mathcal{L} \left[ \frac{f(t)}{t} \right] = \int_{s}^{\infty} F(s)  \mathrm{d} s
    $$
    更一般地，有：
    $$
    \mathcal{L} \left[ \frac{f(t)}{t^{n}} \right] = \underbrace{ \int_{s}^{\infty}  \mathrm{d} s \int_{s}^{\infty}  \mathrm{d} s \cdots \int_{s}^{\infty} F(s)  \mathrm{d} s }_{n \text{ 次}}
    $$

### 平移性（延迟性）

$\mathcal{L}[f(t)]=F(s)(t<0, f(t)=0)$，则
$$
\mathcal{L}[f(t-\tau)]=e^{-s\tau}\mathcal{L}[f(t)]=e^{-s\tau}F(s)\quad(\text{Re }s>c)
$$

函数 $f(t-\tau)$ 与 $f(t)$ 相比，$f(t)$ 从 $t=0$ 开始有非零数值，而 $f(t-\tau)$ 是从 $t=\tau$ 开始才有非零数值，即延迟了一个时间 $\tau$。从它的图象讲，$f(t-\tau)$ 是由 $f(t)$ 沿 $t$ 轴向右平移 $\tau$ 而得，其 Laplace 变换也多一个因子 $e^{-s\tau}$。

### 位移性

$\mathcal{L}[f(t)]=F(s)\,(\operatorname{Re}s > c)$，则
$$
\mathcal{L}\left[e^{\alpha t}f(t)\right] = F(s - \alpha),\quad (\operatorname{Re}(s - \alpha) > c)
\\[1ex]
\mathcal{L}^{-1}[F(s-\alpha)] = e^{\alpha t}f(t)
$$

## Laplace 逆变换

### Laplace 反演积分

已知像函数 $F(s)$ 求原像函数 $f(t)$：
$$
f(t)=\frac{1}{2\pi j} \int _{\beta - j\omega}^{\beta + j\omega} F(s)e^{st}\,\mathrm{d}s,\quad t > 0.
$$
这个积分被称为 Laplace 反演积分。

### Laplace 逆变换的计算

#### 用留数计算

#### 用 Laplace 逆变换的性质计算

$$
\begin{aligned}
\mathcal{L}^{-1}\left[b_{1} F_{1}(s)+b_{2} F_{2}(s)\right] &= b_{1} f_{1}(t)+b_{2} f_{2}(t)
\\[1ex]
\mathcal{L}^{-1}\left[F^{(n)}(s)\right] &= (-t)^{n} f(t)
\\[1ex]
\mathcal{L}^{-1}\left[\frac{F(s)}{s}\right] &= \int_{0}^{t} f(t)dt
\\[1ex]
\mathcal{L}^{-1}\left[\int_{s}^{\infty} F(s)\mathrm{d} s\right] &= \frac{f(t)}{t}
\\[1ex]
\mathcal{L}^{-1}\left[e^{-s\tau} F(s)\right] &= f(t-\tau)
\\[1ex]
\mathcal{L}^{-1}\left[F(s-\alpha)\right] &= e^{\alpha t}f(t)
\end{aligned}
$$

## 卷积

### 卷积概念

两个函数的卷积是指

$$
f_{1}(t) * f_{2}(t) = \int_{-\infty}^{+\infty} f_{1}(\tau) f_{2}(t-\tau)  \mathrm{d} \tau
$$

如果 $ f_{1}(t) $ 与 $ f_{2}(t) $ 都满足条件：当 $ t < 0 $ 时，$ f_{1}(t) = f_{2}(t) = 0 $ ，则上式可以写成：

$$
\begin{aligned}
f_{1}(t) * f_{2}(t) &= \int_{-\infty}^{0} f_{1}(\tau) f_{2}(t-\tau) \,\mathrm{d} \tau
\\
&\qquad +\int_{0}^{t} f_{1}(\tau) f_{2}(t-\tau)  \mathrm{d} \tau
\\
&\qquad + \int_{t}^{+\infty} f_{1}(\tau) f_{2}(t-\tau) \,\mathrm{d} \tau
\\
&= \int_{0}^{t} f_{1}(\tau) f_{2}(t-\tau) \,\mathrm{d} \tau .
\end{aligned}
$$

### 卷积性质

1. 交换律
    $$
    f_1(t) * f_2(t) = f_2(t) * f_1(t)
    $$
2. 分配律
    $$
    f_1(t)*(f_2(t)+f_3(t)) = f_1(t) * f_2(t) + f_1(t) * f_3(t)
    $$
3. 结合律
    $$
    (f_1(t) * f_2(t)) * f_3(t) = f_1(t) * (f_2(t) * f_3(t))
    $$

### 卷积定理

设 $ f_1(t), f_2(t) $ 满足 Laplace 变换存在定理条件，且 $ \mathcal{L}[f_1(t)] = F_1(s) $，$ \mathcal{L}[f_2(t)] = F_2(s) $，则

$$
\mathcal{L}[f_1(t) * f_2(t)] = \mathcal{L}[f_1(t)] \cdot \mathcal{L}[f_2(t)] = F_1(s) \cdot F_2(s)
$$

（或：$ \mathcal{L}^{-1}[F_1(s) \cdot F_2(s)] = f_1(t) * f_2(t) $）

**推广**：$ \mathcal{L}[f_k(t)] = F_k(s) $，$ k = 1, 2, \cdots, n $，则

$$
\mathcal{L}[f_1(t) *\cdots* f_n(t)] = F_1(s) \cdots F_n(s)
$$

或

$$
\mathcal{L}^{-1}[F_1(s) \cdots F_n(s)] = f_1(t) *\cdots* f_n(t)
$$

## Laplace 变换应用

应用拉氏变换解线性微(积)分方程(组)。

### 微分方程的 Laplace 变换解法

$$
\begin{aligned}
    \boxed{\text{微分方程}}
    & \xrightarrow{\text{取拉氏变换}}
    \boxed{\text{像函数的代数方程}}
    \\[2ex]
    & \xrightarrow{\text{解代数方程}}
    \boxed{\text{像函数}}
    \\[2ex]
    & \xrightarrow{\text{取 Laplace 逆变换}}
    \boxed{\text{原像函数是微分方程的解}}
\end{aligned}
$$
