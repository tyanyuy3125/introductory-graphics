Please note that all materials are written in Simplified Chinese, no English materials are provided.

# 近现代计算机图形学导引

建议查看 pdf 文件或者使用本地呈现器打开 markdown 文件。GitHub 对 LaTeX 的渲染支持过于古老了。

## 勘误
* “物理部分”辐亮度方程的左手边不含变量 $\omega_i$ 。
* “信号部分”零阶采样保持的冲激函数左手边应该为 $h(x,y)$ 。
* “信号部分” $\delta$ 函数定义中，右手边的 $x$ 均改为 $t$ 。
* 请注意，“几何部分”的“摄像机模型与透视”一节的末尾，宽高比到视口尺寸参数的转换采用了 OpenGL 的习惯，也就是纵向 FOV，这和之前的推导是不相符的。
* “几何部分”的“可编程渲染管线”一节中，我忽略了当前 WebGL 在使用 OpenGL ES 标准，因此一些旧的 GLSL 语法依然保留。

## 简介

Introductory Graphics is a two-day brief (4 hrs) lecture on computer graphics for first-year students of the Dept. of EE of Tsinghua University.

近现代计算机图形学导引是面向清华大学电子工程系大一年级的本科生开设的一门为其两天的讲座。本讲座分为“几何”“信号”和“物理”三个部分，主要涉及以下内容：

* 几何
    * 特殊欧几里得（Special Euclidean）变换
    * 齐次坐标系（homogeneous coordinates）
    * 网格（mesh）
    * OpenGL 可编程渲染管线（programmable pipeline）入门
    * 包围体积层次（BVH）入门
* 信号
    * 傅里叶分析（Fourier analysis）
    * 图像滤波器
    * 奈奎斯特-香农采样定理（Nyquist-Shannon Sampling Theorem）
    * 超级采样抗锯齿（SSAA）和多重采样抗锯齿（MSAA）技术
* 物理
    * 现代电磁场理论基础
    * 辐射度量学
    * 双向反射分布函数（Bidirectional Reflectance Distribution Function, BRDF）
    * 渲染方程（the rendering equation）
    * 路径追踪（path tracing）

由于时间较短（预计总共4学时），并且面向的是电子系的同学，所以本讲座材料有如下特色：

* 有比较明显的电子工程的特色——但这其实是好事。在传统的图形学讲义中往往不会涉及到完整的信号分析和电磁场理论的内容，这使得图形学的故事总是不够完整。在本讲座中，我们从最基础的数学和物理原理讲起，让整座大厦有坚实的基础。
* 大量的删减。被删减的比较重要内容有：Bezier和NURBS曲线；颜色等。

## 参考资料

* LearnOpenGL - © Joey de Vries
* 3D Computer Graphics: A Mathematical Introduction with OpenGL - © Samuel R. Buss
* Algebra I - © Michael Artin
* 《物理光学》 - 梁铨廷
* 《电磁场理论基础》 - 王蔷、李国定、龚克
* Antennas: For All Applications (3rd edition) - John D. Kraus, Ronald J. Marhefka

## 致谢

特别感谢清华大学电子工程系学生科协软件部（ @eesast ）对本外系势力提供的向电子系学生介绍图形学的机会。

## 授权信息

所有内容按照 CC BY-NC 4.0 授权。

Tianyu Huang @ School of Software, Tsinghua University
