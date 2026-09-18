# 文字与公式的原创示例

以下为说明表达规则而新写的示例，不是范文引文或用户已取得的结果。说明用中文，论文正文示例用英文，各例的假设仅在该例中适用。前四例用于新稿起草或明确获准的相应重写；纯润色不据此新增公式、改变证明顺序、替换常数或拆并段落。

## 例一：交叉项用估计链说明

已知实 Hilbert 空间中的向量 $u,v$，需要估计交叉项，并用 $-a\|u\|^2$ 吸收其中一部分，其中 $a>0$ 已给定。

不够具体的写法：这个交叉项可以用标准不等式处理，再选一个较小参数，就能被负项吸收。

论文正文可以写成：

By the Cauchy–Schwarz and Young inequalities, for any $\varepsilon>0$,

\[
2|\langle u,v\rangle|
\le 2\|u\|\|v\|
\le \varepsilon\|u\|^2+\varepsilon^{-1}\|v\|^2.
\]

Choosing $0<\varepsilon<a$ gives

\[
-a\|u\|^2+2\langle u,v\rangle
\le -(a-\varepsilon)\|u\|^2+\varepsilon^{-1}\|v\|^2.
\]

这里清楚交代了吸收哪一项及留下的代价。若后文还要处理 $\|v\|^2$，必须继续给出依据，不能据此直接宣布整个系统稳定。

## 例二：只用一次的组合直接展开

假定 $a,b,c$ 已有定义且 $c>0$，后文只需检查一次条件

\[
a+\frac{b^2}{4c}<0.
\]

此时直接写上述条件，不再定义一个 $\Theta:=a+b^2/(4c)$ 并称它为“综合稳定指标”。单纯增加名字既没有复用收益，也可能暗示尚未建立的稳定性判据。

若同一复杂组合在后续至少三个实际步骤中被调用，且确实使推导清楚，可以在首次需要时记为一个无冲突的符号。次数不足但确实显著改善可读性时允许例外；本例的短式没有这种必要。不要为了使用新符号而重复内容。纯润色仍保留稿件原有记号。

## 例三：从能量回到状态估计

假定对所有 $t\ge0$，已有可微函数 $V(t)$ 和状态 $x(t)$ 满足

\[
c_1\|x(t)\|^2\le V(t)\le c_2\|x(t)\|^2,
\qquad \dot V(t)\le-\alpha V(t),
\]

其中 $c_1,c_2,\alpha>0$ 是独立于时间和初值的常数。

论文正文可以写成：

The differential inequality yields

\[
\frac{d}{dt}\bigl(e^{\alpha t}V(t)\bigr)
=e^{\alpha t}\bigl(\dot V(t)+\alpha V(t)\bigr)\le0.
\]

Integrating this inequality and using the bounds on $V$, we obtain

\[
\|x(t)\|^2
\le c_1^{-1}V(t)
\le c_1^{-1}e^{-\alpha t}V(0)
\le \frac{c_2}{c_1}e^{-\alpha t}\|x(0)\|^2.
\]

This establishes the claimed exponential estimate.

没有必要给只在求导时出现的 $e^{\alpha t}V(t)$ 另起一个名称。若要陈述范数而非范数平方的衰减率，取平方根后速率为 $\alpha/2$，不能仍写成 $\alpha$。

## 例四：“充分大”需要量化依据

假定 $a>0$，不同估计给出的常数 $C_1,C_2\ge0$ 已固定且不依赖正整数 $N$。需要证明 $-aN^2+C_1N+C_2<0$ 可实现。

论文正文可以写成：

Choose a positive integer $N$ such that

\[
N\ge\max\left\{1,\frac{4C_1}{a},\sqrt{\frac{4C_2}{a}}\right\}.
\]

Then $C_1N\le aN^2/4$ and $C_2\le aN^2/4$, and hence

\[
-aN^2+C_1N+C_2
\le-aN^2+\frac a4N^2+\frac a4N^2
=-\frac a2N^2<0.
\]

两个常数各自可追踪，不用同名的可变 C 代替它们。这里给出了参数选择和关键估计，不必再为只用一次的阈值另起符号。若实际问题中 $C_1$ 或 $C_2$ 依赖于 $N$，必须分析该依赖，不能照抄结论。

## 例五：证明审查具体指出缺什么

原稿写“由上述估计可得均方指数稳定”，但前文只有 $\mathbb E[x(t)]\to0$。

应指出：现有估计控制的是状态的期望，尚未给出 $\mathbb E\|x(t)\|^2$ 的衰减界。需要相应的二阶矩估计才能得到所述结论。不要为了使语言顺畅，直接把前式改写成二阶矩不等式。

这类问题属于数学依据不足，不能当作普通措辞问题静默修补。润色时将它作为中文注释单列，不新增二阶矩公式或改写原结论。若原稿已经具备完整论证，则只改善英文连接句，不另写泛泛解释。

## 例六：只改英文的润色边界

原稿（一个段落）：

By using the Cauchy–Schwarz inequality, it can be obtained that $|\langle u,v\rangle|\le\|u\|\|v\|$. This estimate will be used in the following analysis.

润色后（仍为一个段落，公式完全相同）：

The Cauchy–Schwarz inequality gives $|\langle u,v\rangle|\le\|u\|\|v\|$. We use this estimate in the subsequent analysis.

这次修改只压缩英文措辞。不把行内式移动到独立公式，不补 Young 不等式，不改变证明次序。只有用户另行明确要求相应重写，才进行这些改动。
