# 电磁场与电磁波笔记
# 目录
>   * [1.矢量与场论](#1)
>      * [1.1正交坐标系与矢量](#11)
>      * [1.2梯度与散度](#12)
## <w id=1> 1.矢量与场论</h2>

>* [1.1正交坐标系与矢量](#11)
>* [1.2梯度与散度](#12)
### <w id=11>1.1正交坐标系与矢量</h3>

#### 矢量
>1. **表示**： 用 <font color=#66CCFF> $\vec{A}=A_x\hat{a_x}+A_y\hat{a_y}>+A_y\hat{a_y}$</font> 来表示
>2. **叉乘**
>$\vec{A}\times\vec{B}= \begin{array}{|ccccc|}
>   \hat{a}_x & \hat{a}_y & \hat{a}_z\\
>   \hat{A}_x & \hat{A}_y & \hat{A}_z\\
>   \hat{B}_x & \hat{B}_y & \hat{B}_z
>  \end{array} $ 
> 方向是右手<font color=#ff0000>$\vec{A}$扫向$\vec{B}$</font>
>3. **运算规律**: **<font color=#ff0000>反交轮换平方差</font>**
>   <img src="pic/叉乘关系.png" style="zoom:50%">  
>4. **点乘**：<font color=#66ccff>满足分配律和交换律</font>  
#### 正交曲线坐标系
>1. **单位矢量**：曲线切向量指向增加一侧
>2. **弧微分和拉梅系数**
><font color=#66d>拉梅系数:</font> <font color=#ff0000>$H_i=±\sqrt {(\frac{\partial{x}}{\partial{q_i}})^2+(\frac{\partial{y}}{\partial{q_i}})^2+(\frac{\partial{z}}{\partial{q_i}})^2}$</font>
>则 <font color=#ff0000>$ds_i=H_idq_i$</font> 面积元体积元看着办
>注意：<font color=#66ccff>ds_i理解为i变量引起的线长度变化</font>
>3. **坐标系弧微分**
>* <font color=#66ccff>柱坐标</font>
$dl_r=dr$
$dl_\phi=rd_\phi$
$dl_r=dz$
>* <font color=#66ccff>球坐标系</font>
$
    \begin{cases}
        dl_R=dR &\\
        dl_\theta=Rd\theta\\
        dl_R=Rsin(\theta)d\phi
    \end{cases}
$
>4. **矢量**：  
>       * 矢量函数：某点矢量与该点位置的关系,
>       <font color=#ff0000>矢量是由该点为起点出来的一个向量</font>，不一定是单位的
>       * 单位矢量，就是一个表征方向的模长为1的矢量
>       * 有点像<font color=#ff0000>$(\vec{x},\vec{y},\vec{z})和(x,y,z)$</font> 的关系
>       * 常矢量&变矢量指的是方向，<font color=#ff0000>在绝对空间里面会不会变化</font>
>       比如不同的点$a_x$都是x的一个绝对方向，但是$a_\theta$就不一定了

### <w id=12>1.2梯度与散度</h3>

####  标量场的梯度
>1. **场**：空间每点都对应物理量的一个确定值，则称在此空间确定了该量的一个场。
>2. **方向导数**<font color=#ff0000>$\frac{\partial{u}}{\partial{l}}|_{M_0}=\frac{\partial{u}}{\partial{x}}cos(\alpha)+\frac{\partial{u}}{\partial{y}}cos(\beta)+\frac{\partial{u}}{\partial{z}}cos(\gamma)$</font>
>算偏导-->算余弦
>3. **梯度**：最大的方向导数记为<font color=#66ccff>gradu</font>
>    * $\vec{G}=\hat{a_x}\frac{\partial{u}}{\partial{x}}+\hat{a_y}\frac{\partial{u}}{\partial{y}}+\hat{a_z}\frac{\partial{u}}{\partial{z}}$
<font color=#ff0000>$\vec{l}与\vec{g}$方向相同</font>的时候方向导数最大,模最大为$gradu=|\vec{G}|$
>    * 哈密瓜算子 $
     \nabla=\vec{G}=\hat{a_x}\frac{\partial{}}{\partial{x}}+\hat{a_y}\frac{\partial{}}{\partial{y}}+\hat{a_z}\frac{\partial{}}{\partial{z}}$
>    * $gradu=\nabla u$ <font color=#ff0000>其他坐标系注意微分变换就好</font> 
>    底下的东西用弧微分变换公式，因为本来是对弧微分求导数的
>    * <font color=#66ccff>因地制宜建立合理的坐标系</font>

####  标量场的散度

>1. **辨析矢量场，矢量线**   <font color=#66ccff>
>    * 矢量：空间里面的矢量，有方向，有大小
>    * 矢量场：一整个空间，每个坐标都有一个有方向的矢量
>    * 矢量线：一条和经过的每个点的矢量都相切的有向线段 
>2. </font> **绘制矢量线**
>    1. 先求出矢量的空间分布函数
>    2. 利用dl和空间分布函数同向的关系得到三个分量成比例转换为x，y，z的关系即可
>3. **矢量场的通量**
>    * 计算公式，其中cosθ是和法向量夹角，结果是个标量
>     <img src="pic/矢量的通量.png" style="zoom:50%">  
>4. **散度**
>    * <font color=#ff0000>$div\vec{A}=\int^{}\displaystyle\lim_{x\to0}\frac{\int_s \vec{A}\cdot d\vec{S}}{\Delta V}$</font>
>    * 定义为改通量源的能量密度，>0正源，<0负源，=0无源
>    * 用泰勒级数可以推出的一个散度公式 
>    * $div\vec{A}=\nabla\vec A$要注意和梯度辨析开来
>
>









