- [1. 前言](#1-前言)
  - [1.1 算法（Algorithms）和数据结构（Data Structure）](#11-算法algorithms和数据结构data-structure)
  - [1.2 什么是好的算法？](#12-什么是好的算法)
  - [1.3 算法分析](#13-算法分析)
    - [1.3.1 实验分析（Experimental Analysis）](#131-实验分析experimental-analysis)
    - [1.3.2 理论分析](#132-理论分析)
      - [1.3.2.1 伪代码（Pseudo-code）](#1321-伪代码pseudo-code)
      - [1.3.2.2 随机访问机器（Random Access  Machine）](#1322-随机访问机器random-access--machine)
      - [1.3.2.3 时间复杂度（Time omplexity）](#1323-时间复杂度time-omplexity)
      - [1.3.2.4 渐进符号（Asymptotic notation）](#1324-渐进符号asymptotic-notation)
        - [1.3.2.4.1 大O符号（Big-Oh Notation）](#13241-大o符号big-oh-notation)
        - [1.3.2.4.2 大Ω符号（Big-Omega Notation）](#13242-大ω符号big-omega-notation)
        - [1.3.2.4.3 大Θ符号（Big-Theta Notation）](#13243-大θ符号big-theta-notation)
    - [1.3.2.5 空间复杂度（Space Complexity）](#1325-空间复杂度space-complexity)
- [2. 数据结构](#2-数据结构)
  - [2.1 Stacks（栈）](#21-stacks栈)
    - [2.1.1 相关方法](#211-相关方法)
    - [2.1.2 应用](#212-应用)
      - [2.1.2.1 翻转数组](#2121-翻转数组)
      - [2.1.2.2 后缀表达式/反向波兰表达式（Postfix notation， Reverse Polish notation）](#2122-后缀表达式反向波兰表达式postfix-notation-reverse-polish-notation)
      - [2.1.2.3 迷宫问题等搜索问题](#2123-迷宫问题等搜索问题)
  - [2.2 队列（Queues）](#22-队列queues)
    - [2.2.1 相关方法](#221-相关方法)
    - [2.2.2 实践](#222-实践)
      - [2.2.2.1 循环队列（Circular Queue）](#2221-循环队列circular-queue)
      - [2.2.2.2 多线程编程（Multithreading）](#2222-多线程编程multithreading)
  - [2.3 列表（List）](#23-列表list)
    - [2.3.1 相关方法](#231-相关方法)
    - [2.3.2 实践](#232-实践)
      - [2.3.2.1 单链表（Singly-linked list）](#2321-单链表singly-linked-list)
      - [2.3.2.2 双链表（Doubly-linked list）](#2322-双链表doubly-linked-list)
  - [2.4 根树（Rooted Tree）](#24-根树rooted-tree)
    - [2.4.1 相关术语（Terminology）](#241-相关术语terminology)
    - [2.4.2 二叉树（Binary Trees）](#242-二叉树binary-trees)
    - [2.4.3 相关方法](#243-相关方法)
      - [2.4.3.1 访问方法](#2431-访问方法)
      - [2.4.3.2 查询方法](#2432-查询方法)
      - [2.4.3.3 通用方法](#2433-通用方法)
    - [2.4.4 实践](#244-实践)
      - [2.4.4.1 节点的深度](#2441-节点的深度)
      - [2.4.4.2 树的高度](#2442-树的高度)
      - [2.4.4.3 树遍历（Tree Traversal）](#2443-树遍历tree-traversal)
        - [2.4.4.3.1 前序遍历（Preorder traversal）](#24431-前序遍历preorder-traversal)
        - [2.4.4.3.2 后序遍历（Postorder traversal）](#24432-后序遍历postorder-traversal)
        - [2.4.4.3.3 中序遍历（Inorder traversal）](#24433-中序遍历inorder-traversal)
      - [2.4.4.4 算术表达式](#2444-算术表达式)

# 1. 前言
这门课程是之前INT102的进阶，它介绍算法分析的基础概念并且介绍算法的复杂度分析。

## 1.1 算法（Algorithms）和数据结构（Data Structure）
1.数据结构是一种系统化地组织和访问数据的方式。通过合理地组织数据，可以提高数据的存储效率、访问速度和操作便利性。常见的数据结构包括数组、链表、栈、队列、树、图等。
2.算法是在有限时间内完成某项任务的一系列步骤。算法是解决问题的具体方法，通过一系列逻辑步骤实现特定的功能或目标。不同的算法有不同的效率和适用场景。
例如：1.导航到某个地方需要使用算法来规划从起点到终点的最佳路径。
2.通过算法将音频或视频文件从一种格式转换为另一种格式。
3.通过算法来控制太阳能板，从而最大化太阳能的利用效率。
4.通过算法将二维或三维模型渲染成图像或视频。
5.用于求解方程的根（即解）的算法。
6.用于减少文件大小的压缩算法。
7.用于寻找最优解或近似最优解的优化算法。
8.用于将图形或图像数据转换为最终视觉效果的算法。
我们在学习数据结构的时候我们也会经常提到算法，因为程序是算法和程序的结合体，两者相辅相成。每种数据结构有其对应的算法，它们也有各自的使用场景。
比如数组有不同的排序算法，比如快速排序（Quick Sort）、归并排序（Merge Sort）、冒泡排序（Bubble Sort）等。搜索方法有二分查找（Binary Search），它们有不同的使用场景。
再比如树有不同的遍历算法，图有不同的遍历算法。

## 1.2 什么是好的算法？
因为算法和数据结构相辅相成，所以好的算法也需要依赖高效的数据结构。在当前讨论组，我们说的“好”是运行速度快的，这将在课程中进一步阐述。

## 1.3 算法分析
我们使用算法分析来评价一个算法的效率。
算法分析是对计算机程序性能和资源使用的理论研究。主要关注点是算法的运行时间（时间复杂度）以及对数据结构的操作。次要关注点是算法的空间（或“内存”）使用（空间复杂度）。
本课程专注于算法及其相关数据结构的数学设计与分析，并使用相关的数学工具来实现这一目标。

我们关注运行时间或内存需求与输入规模之间的依赖关系。
输入规模的定义取决于具体问题的背景。例如：
在图算法中，输入规模通常用顶点数（V）和边数（E）表示。
在字符串处理中，输入规模通常用字符串的长度表示。
在数值计算中，输入规模可以用数字的位数表示。

### 1.3.1 实验分析（Experimental Analysis）
为了分析算法，我们有时通过实验分析来分析算法，通过实际运行算法来测量其性能，而不是仅仅依赖于理论分析。这种方法可以帮助我们了解算法在实际数据上的表现，尤其是在理论分析难以准确预测的情况下。但进行实验性分析需要合理选择样本输入，并进行适当数量的测试，以便我们能够对分析结果有统计上的信心。

由于运行时间取决于输入的规模和具体实例，以及使用的算法和运行的环境。其中输入的规模不难理解，对于具体实例会因为输入的具体实例不同，即使规模相同，也可能导致运行时间不同。例如对于冒泡排序来说，已排序的数组的时间复杂度是$O(n)$，对于完全随机的数组的时间复杂度是$O(n^2)$。
一般来说，算法或数据结构方法的运行时间会随着输入规模的增加而增加。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/ca9a2826811548d8b97ad5b79d1a7e8a.png)
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/ff138d7969764b4f9f33e8439330bcd2.png)
因此对于实验分析来说有以下几点需要注意：
1.实验是在有限的测试输入集上进行的。
2.所有测试必须在相同的硬件和软件环境下进行。
3.需要实现并运行算法。

### 1.3.2 理论分析
理论分析与实验分析相比有以下优势：
1.可以考虑所有可能的输入。
2.可以在不依赖硬件/软件环境的情况下，比较两个（或更多）算法的效率。
3.涉及研究算法的高级描述——伪代码（pseudo-code）。

当我们以这种方式分析算法时，我们的目标是为每个算法关联一个函数$f(n)$，其中$f(n)$表征了运行时间，这是基于输入大小$n$的某种度量。
这种$f(n)$函数的典型有：$n$，$log n$，$n^2$，$nlogn$，$2^n$...
用这种方式我们可以将算法运行的时间表示出来，因为算法$A$的运行时间与$n$成正比，因此$f(n)=kn$，其中$k$是一个常数，每增加一个单位的输入规模，运行时间就增加$k$个单位。

为了完成理论分析需要四个要素：
1.描述算法的语言，即伪代码我们后面会再复习一遍。
2.算法执行的计算模型，常见的包括图灵机，以及后文复习的随机访问机器（RAM）。
3.衡量性能的度量标准，即时间复杂度和空间复杂度。
4.描述性能的方法， 我们可以使用Big-Oh符号等来描述，后文也会复习。

我们前面就说过一个算法会因为输入的具体实例不同而有不同的运行时间。因此有平均情况复杂度（Average-case complextiy)和最坏情况情况复杂度（Worst-case complextiy)
平均情况复杂度指的是在所有相同规模的输入中，算法运行时间的平均值。
最坏情况复杂度指的是在所有相同规模的输入中，算法运行时间的最大值。
平均情况复杂度反映了算法在大多数情况下的性能，而最坏情况复杂度则提供了算法在最不利情况下的性能保证。由于最坏情况复杂度对于确保系统稳定性和可靠性的重要性，我们通常更关注它。
对于平均情况分析通常需要我们基于给定的输入分布来计算预期的运行时间。
#### 1.3.2.1 伪代码（Pseudo-code）
伪代码是一种用于描述算法的高级语言。
它提供了更结构化的算法描述，允许我们对算法进行高级分析，以确定它们的运行时间（和内存需求）。
下面的例子用伪代码编写了一个找到一组数字中最小数字的代码。
```
Algorithm Minimum-Element(A)  
input: An array A sorting n≥1 integers  
output: minimum element min
min ← A[0]
for i ← 1 to n-1 do
 	if min > A[i] then  
		min ←A[i]
return min
```
其中我们也可以使用等号代替←，也可以使用大括号来代替if-then-end结构。

从上面的例子中我们也可以看出，伪代码不像传统的编程语言对语法格式有所要求，它是自然语言和高级编程语言（例如 Java、C 等）的混合体。伪代码的目的是提供一个通用的、与特定编程语言无关的算法或数据结构实现描述。
伪代码包括：表达式、声明、变量初始化和赋值、条件语句、循环、数组、方法调用等。
这门课中，不会正式定义一个严格的伪代码编写方法，但当需要使用它时，我们的目标是以一种方式描述算法，使一个称职的程序员能够将伪代码转换为程序代码，而不会误解算法。（换句话说这门功课不会要求写伪代码，但是需要能够理解伪代码描述的算法是哪种）。
伪代码忽略了底层的实现细节，它由一些列高级原始操作，包括赋值、调用方法、执行算术操作、比较、通过索引访问元素、引用、返回等。然后为了分析算法的运行时间，我们计算算法执行过程中执行的操作数量。

示例如下：对于如下伪代码我们可以计算算法中执行的原始操作有多少次。

```
 Algorithm arrayMax(A,n):
 input: array A
 output: maximum element currentMax
	currentMax ← A[0]
	for j ← 1 to n-1 do
		if currentMax<A[j]
			then currentMax ← A[j]
	returncurrentMax
```
对于第一行，我们通过索引读取数组里的值，然后再赋值，因此是$2$次。
第二行我们先赋值一次，然后我们会比较$n$次，$1<n$，所以是$n+1$次。
第三行我们通过索引读取数组里的值，然后再比较，因此是$2(n-1)$次。
第四行中如果我们的值每次要更新那就会运行$2(n-1)$次，索引读取和赋值，但是如果我们赋值的就是最大的值。
之后我们其实需要让j自增1，这一步是一次算术和一次赋值，因此是$2(n-1)$次。
最后返回值$1$次。
最好情况：$2+1+n+4(n-1)+1=5n$。
最坏情况：$2+1+n+6(n-1)+1=7n-2$。
由于数操作数没有一个标准，因此考试也不会考察该部分。

下面我们再看一个递归算法。
例如$T(n)=3, n=1;T(n) = T(n-1)+7, n ≥ 2$，我们可以将其递归关系转换为封闭形式$T(n)=7T(n-1)+3=7n-4$。
了解基本的递归算法后我们可以尝试一下斐波拉契数列，尝试写出它的伪代码。
示例如下。

```
Algorithm: fibonacci numbers  
Input: upper limit n
Output: The n-th term of Fibonacci  
int fib (int n){
if n <=2  
	return 1;
else
 	return fib(n-1)+fib(n-2);
}
```
我们之前就学过递归算法，虽然递归算法在某些情况下可能看起来更简单，但它们也可能引入一些问题。比如重复解决子问题，递归算法将大问题分解为小问题，而这些小问题可能在递归调用过程中被多次遇到。
如下图所示。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/d818a8a1f0ed47aeafc554a22660bf85.png)
计算第六项的时候计算了前面的第三项三次。所以如果输入值较大时，可能因为大量重复计算而导致栈空间迅速增加，最终超出计算机的内存限制。
我们可以使用动态规划（Dynamic Programming）方法避免每个子问题进行了多次计算。
动态规划的斐波拉契数列伪代码如下。

```
Algorithm: fibonacci numbers  
Input: upper limit Nmax
Int f(int Nmax)
{
f1 ←1;
f2 ←1;
for n←3:(Nmax-2){  
	fn← f2 + f1;
	f1 ←f2;  
	f2 ←fn;
	}
return fn;
}
```

#### 1.3.2.2 随机访问机器（Random Access  Machine）
随机访问机器是一种计算模型，通过简化计算机的操作来便于分析。
在RAM模型中，计算机由一个中央处理单元（CPU）和一个存储单元组（内存）组成。CPU负责执行计算和控制操作，而内存用于存储数据。其中内存单元是基本的存储单位，可以存储不同类型的数据，如整数、浮点数、字符或内存地址。这种灵活性使得RAM模型能够模拟各种计算机操作。
我们假设原始操作（如单个加法、乘法或比较）需要恒定的时间来执行，即无论操作数的大小如何，这些操作的执行时间都是相同的。虽然 RAM 模型假设所有基本操作都需要恒定时间，但实际上，不同操作的执行时间可能不同。例如，乘法通常比加法需要更多的时间来执行。这种假设简化了算法分析，但可能不完全反映真实计算机的性能。

#### 1.3.2.3 时间复杂度（Time omplexity）
时间复杂度关注的是算法运行时间随着输入规模趋近于无穷大时的变化趋势，而不是具体的运行时间。通常用下面我们说的渐进符号来表示其变化趋势。

#### 1.3.2.4 渐进符号（Asymptotic notation）
我们使用渐进符号描述算法运行时间或其他资源需求随着输入规模增长的变化趋势。因此我们可以实验渐进符号来比较两个算法的运行时间。在算法分析中，渐近符号用于简化分析过程。它估计执行的原始操作数量，但只考虑常数因子。这意味着我们关注的是算法运行时间的主导项，而不是常数乘数。
下图展示了对于不同算法运行时间对应的最大问题规模$（n）$。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/5069c185efe84515872a8e3d1805968d.png)
从长远角度来看，渐进较快的算法优于渐进较慢的算法。这里渐进更快指的是在后续的Big-Oh符号等渐进符号中，前者的增长速率低于后者。例如，一个具有$O(logn)$时间复杂度的算法比具有$O(n)$时间复杂度的算法“渐进更快”，因为对数函数的增长速率远低于线性函数。

我们现在复习以下函数的增长率。
对于多项式函数来说：
线性函数（Linear），增长率与输入规模$n$成正比，表示为$n$。
二次函数（Quadratic），增长率与输入规模$n$的平方成正比，表示为$n^2$。
三次函数（Cubic），增长率与输入规模$n$的立方成正比，表示为$n^3$。
我们现在使用对数-对数图来比较不同函数的增长率，因为它可以将指数增长或多项式增长的函数转换为直线。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/d169c84b41684bc2b5095e3bd04527b5.png)
在分析增长率时，我们通常关注算法的主导项（即最高次项），因为它们对算法在大规模输入下的性能影响最大。因此我们忽略常数因子（constant factors），例如$10n$和$100n$的常数不同，但都被认为是线性增长。我们还会忽略低阶项（Lower-Order Terms），例如$n^2+n$中的$n$就是低阶项。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/c9d8c7fed41542f2a2eb2e894a3b1fbb.png)
前面我们说过理论分析是找到描述算法运行时间与输入规模之间的关系，这个函数也就是这里用来表达算法的渐进行为，我们用渐进符号来描述这种渐进行为。

##### 1.3.2.4.1 大O符号（Big-Oh Notation）
大O符号（Big-Oh Notation）是描述算法运行时间或其他资源消耗上界的一种常用渐近符号。它让我们能够以一种标准化的方式表达算法在最坏情况下的性能。
其定义如下：
给定两个正函数$f(n)$和$g(n)$（它们都是在非负整数上定义的），我们说$f(n)$是$O(g(n))$，记作$f(n)∈O(g(n))$，如果存在常数$c$和$n_0$使得$f(n)≤c⋅g(n)$对所有$n≥n_0$成立。
例如：$2n+10$用大O符号描述为$O(n)$
过程如下：
$2n+10 ≤ cn$
$(c-2)n ≥ 10$
$n ≥ 10 / (c - 2)$
取$c=3，n_0=10$即可满足$2n+10≤3n$对所有$n≥10$，因此$2n+10$用大O符号描述为$O(n)$。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/edf8119512e247028a363793ad8b7e77.png)


我们前面说大O符号描述算法的运行时间或空间复杂度的上界，因此对于函数$n^2$其大O符号表示不是$O(n)$。
证明过程如下：
$n^2 ≤ cn$
$n ≤ c$
上述不等式不能被满足，因为$c$必须是一个常数。要使$n≤c$对所有$n$都成立，$c$必须大于或等于所有可能的$n$，这是不可能的，因为$n$可以无限增大。
或者说$n^2$的增长速度比$n$快，所以$O(n^2)$的运行时间会比$O(n)$慢。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/81cf59db8965462f9798b8fd60ed4c7a.png)
下图展示了多种函数的增长速度，从左到右速度不断增加。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/d9fa6e154e4e49f98231a458fdaa0ef8.png)
更多的例子如：
$7n-2$的大O符号是$O(n)$，$c=7，n_0=1$。
$3n^3+20n^2+5$的大O符号是$O(n^3)$，$c=4，n_0=21$。

我们对增长速度做出进一步解释，“$f(n)$是$O(g(n))$”的声明意味着$f(n)$的增长率至多与$g(n)$的增长率一样快。
通过大O符号，我们可以根据增长率对函数进行排序。
下图进一步展示了刚刚说的这两点。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/10785d52febe4279b46c22a5b95b913a.png)
外面的函数的增长速度小于等于$O$里面的函数。

对于我们的日常函数的大O符号如下：
1.常数:$O(1)$
2.对数函数:$O(logn)$
3.线性函数:$O(n)$
4.线性对数函数:$O(nlogn)$
5.二次函数:$O(n^2)$
6.三次函数:$O(n^3)$
7.多项式函数:$O(n^k)$
8.指数函数:$O(a^n0),a>1$
9.阶乘函数:$O(n!)$

如果$f(n)$是一个次数为$d$的多项式，那么$f(n)$是$O(n^d)$。我们只需要关注最高次项，忽略低次项和常数因子。
此外还有两点需要注意：
1.选择能最准确描述函数增长速度的最小可能的函数类别。
例如：对于$2n$的大O符号是$O(n)$而不是$O(n^2)$。
2.选择最简单的表达式来表示函数类别。
例如：对于$3n+5$的大O符号是$O(n)$而不是$O(3n)$。

因此更多例子如下：
1.$13 n^3 +7nlogn+3$的大O符号是$O(n^3)$
2.$3logn + loglogn$的大O符号是$O(logn)$因为$3logn + log logn ≤ 4 log n$当$n≥2$时。
3.$2^{70}$的大O符号是$O(1)$
对于第三个的证明如下：$2^{70}≤2^{70} * 1$，对于$n≥1$都成立。

我们使用渐进算法进行分析时，我们先确定算法在最坏情况下执行的原始操作（如比较、赋值等）的数量，并将这个数量表示为输入规模 n 的函数。然后使用大O符号来描述算法运行时间的上界。
我们以查找数组中最大元素的算法为例，前面我们数过这个算法的原始操作的次数为$7n-2$。因此我们就说这个算法的运行时间为$O(n)$。

```
Algorithm prefixAverage1(X,n)
	Input array X of n integers
	Output array A of prefix averages of X
	A ← new array of n integers
	for i ← 0 to n - 1 do
		s ← X[0]
		for j ← 1 to i do
			s ← s + X[j]
		A[i] ← s / (i+1)
	return A
```
由于这里使用了求和，所以根据求和公式，想要计算n个整数的和，通过求和公式$n(n + 1) / 2$，因此它的运行时间为$O(n^2)$。
或者我们看这里是由一个循环在另一个循环里面，因此是$O(n^2)$。

下面这个算法中并不是每次都要单独计算前$n$个数的和，而是直接每次在前一次和上加最新一项，因此这里的运行时间为$O(n)$。

```
Algorithm prefixAverage2(X,n)
	Input array X of n integers
	Output array A of prefix averages of X
	A ← new array of n integers
	s ← 0
	for i ← 0 to n - 1 do
		s ← s + X[i]
		A[i] ← s / (i + 1)
	return A
```
因此这里只有一次循环。

下面多给几个例子：

```
s ← 0
for i ← 1 to n do
    s ← s + i
```
时间复杂度为$O(n)$。

```
p ← 1
for i ← 1 to 2n do
    p ← p * i
```
时间复杂度为$O(n)$。

```
p ← 1
for i ← 1 to n^2 do
    p ← p * i
```
时间复杂度为$O(n^2)$。因为循环是从$1$到$n^2$。

```
s ← 0
for i ← 1 to 2n do
    for j ← 1 to i do
       s ← s + i
```
时间复杂度为$O(n^2)$。因为是嵌套循环。

##### 1.3.2.4.2 大Ω符号（Big-Omega Notation）
我们说$f(n)$是$Ω(g(n))$，如果存在实数常数$c$和$n_0$，使得所有$n≥n_0$，都有$f(n)≥cg(n)$。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/c165b498a68747228559e2205143c441.png)
##### 1.3.2.4.3 大Θ符号（Big-Theta Notation）
我们说$f(n)$是$Θ(g(n))$，如果$f(n)$既是$O(g(n))$又是$Ω(g(n))$。这意味着$f(n)$的增长速率与$g(n)$完全相同，即$f(n)$既不超过$g(n)$的某个常数倍的增长速率，也不低于$g(n)$的某个常数倍的增长速率。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/f7a4686491ab4c8c917962b7467ba8fb.png)
因此我们现在总结这三种渐进符号。
1.大O符号（Big-Oh）
如果$f(n)$是$O(g(n))$，这意味着$f(n)$的增长速率在渐近意义上小于或等于$g(n)$的增长速率。换句话说，随着输入规模$n$的增大，$f(n)$的增长不会超过$g(n)$的某个常数倍。
2.大Ω符号（Big-Omega）
如果$f(n)$是$Ω(g(n))$，这意味着$f(n)$的增长速率在渐近意义上大于或等于$g(n)$的增长速率。也就是说，随着输入规模$n$的增大，$f(n)$的增长至少和$g(n)$的某个常数倍一样快。
3.大Θ符号（Big-Theta）
如果$f(n)$是$Θ(g(n))$，这意味着$f(n)$的增长速率在渐近意义上等于$g(n)$的增长速率。换句话说，随着输入规模$n$的增大，$f(n)$的增长速率与$g(n)$的增长速率完全相同。

示例如下：
$3logn + log logn$的时间复杂度是$Ω(logn)$。因为$3logn + log logn ≥ 3 log n$当$n≥2$时。
前面我们也得到过$3logn + log logn$的时间复杂度是$O(logn)$。
因此我们可以得到$3logn + log logn$的时间复杂度是$Θ(logn)$。

### 1.3.2.5 空间复杂度（Space Complexity）
空间复杂度是衡量算法所需的存储空间量的一个指标。具体来说，它指的是在算法的任何时刻，在最坏情况下需要多少内存。
与时间复杂度类似，我们主要关注的是随着输入问题规模$N$的增长，空间需求如何增长，用大O符号来表示。
例子如下：

```java
int sum(int x, int y, int z) {  
int r = x + y + z;
 return r;
 }
```
这个算法需要三个单位的空间用于参数以及一个单位的空间用于局部变量，并且这个空间需求是固定的与输入规模$N$无关，因此它的空间复杂度是$O(1)$。

```java
int sum(int a[], int n) {  
int r = 0;
for (int i = 0; i < n; ++i) {  
	r += a[i];
	}
return r;
}
```
这个算法需要$N$个单位的空间用于数组a，以及n，r和i分别一个单位的空间，因此它的空间复杂度是$O(n)$。

# 2. 数据结构
我们现在讲数据结构。

首先我们重申一遍数据结构的重要性：
1.算法的执行依赖于数据（信息）。
2.算法计算的速度部分取决于对数据的高效使用。
3.数据结构是存储和访问信息的特定方法。
4.我们研究不同类型的数据结构，可以根据特定算法的需求寻找其合适的数据结构。
## 2.1 Stacks（栈）
栈是一种遵循“后进先出”（Last-in，First-Out，简称LIFO）的数据结构。这意味着最后被添加到栈中的元素将是第一个被移除的元素。
因此我们直接访问的元素只能是最后一个被插入的元素，即栈顶元素。
但是可以在任何时候向栈中添加元素，只要栈没有溢出（即没有达到其最大容量限制）。而新元素是被添加到栈的栈顶。
例如，Web 浏览器使用栈来存储最近访问的网页地址。当你点击浏览器的“后退”按钮时，浏览器从栈中弹出（Pop）最顶部的地址，即最后访问的网页，然后显示该网页。

### 2.1.1 相关方法
栈（Stacks）作为一种抽象数据类型（Abstract Data Type，简称 ADT），下面列出其支持的一些基本操作和方法。
1.push(Obj)：将对象 Obj 插入到栈的顶部。
2.pop()：移除（并返回）栈顶部的对象。如果栈为空，则该操作会触发错误或异常。
3.initialize()：初始化栈，通常将栈设置为一个空状态。
4.isEmpty()：返回 true 如果栈为空，否则返回 false。
5.isFull()：返回 true 如果栈已满，否则返回 false。

对于基础操作的push和pop的伪代码如下：

```
PUSH(Obj)
# Check to see if stack is full
if size() == N
	then indicate "stack-full" error occurred
else t ← t + 1
	S[t] ← Obj
```

```
POP()
# Check to see if stack is empty
if isEmpty()
	then indicate "stack empty" error occurred
else Obj ← S[t]
	S[t] ← null
	t ← t - 1
return Obj
```

具体push和pop操作过程如下图所示。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/76f59508df3c4fd69f157fc082cffc8e.png)
### 2.1.2 应用
栈在现代过程式编程语言（例如 C、C++、Java 等）的运行时环境中非常重要。这是因为这些语言通常使用栈来管理函数调用、局部变量和控制流语句（如循环和条件语句）。在函数调用时，每个函数的参数、返回地址和局部变量通常被压入（push）调用堆栈（call stack）中。当函数执行完毕后，这些信息被弹出（pop）堆栈，程序控制返回到调用函数。
此外，表达式求值、编译器优化和内存管理等许多底层操作也依赖于栈结构。
如果使用算式表达式使用的是后缀表达式（postfix notation，也称反向波兰表达式，Reverse Polish notation（RPN））则可以使用栈来计算。

#### 2.1.2.1 翻转数组
我们前面在别的课中也学习了如何讲数组里的值翻转一遍，现在我们使用栈来解决这个问题我们会发现，栈做这种事非常适合。

```
ReverseArray(Data: values[])
 	// Push the values from the array onto the stack.  
	Stack: stack = New Stack
 	For i = 0 To <length of values> - 1  
		stack.Push(values[i])
 	Next i
 	// Pop the items off the stack into the array.
 	For i = 0 To <length of values> - 1  
		values[i] = stack.Pop()
 	Next i
End ReverseArray
```
刚好我们从头开始读取数组里的每一项，由于FILO，我们最先放进的值就将最后一个被读出来因此就实现了数组的翻转。

#### 2.1.2.2 后缀表达式/反向波兰表达式（Postfix notation， Reverse Polish notation）
在后缀表达式中，操作数（如变量或数字）位于算术运算符之前，当遇到一个运算符时，它应用于之前遇到的两个操作数。例如，中缀表达式$x + y$在后缀表达式中写作$x y +$,中缀表达式$(x + y) * z$在后缀表达式中写作$x y + z *$,中缀表达式$x * (y + z)$在后缀表达式中写作$x  y z + *$，中缀表达式的$-x$的后缀表达式写作$x-1*$。
同理我们也可以用后缀表达式也可以转化为中缀表达式，后缀表达式的$xywz/-*$写成中缀表达式为$x*(y-w/z)$。

下图展示了如何用栈处理后缀表达式。
步骤如下：
1.遇到操作数就将其压入栈中。
2.遇到操作符就从栈中弹出所需的操作数，执行运算，并将结果压回栈中。
3.最终，栈顶元素即为表达式的结果。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/08a7eda9e81b483da16f3e4e9184b5e2.png)
第一个元素是$7$，所以压入栈中。
第二个元素是$5$，也压入栈中。
第三个元素是$3$，也压入栈中。
第四个元素是$+$，因此弹出两个操作数出来，执行计算为$5+3$，得到$8$后再压入栈中。
第五个元素是$*$，因此弹出两个操作数出来，执行计算为$7*8$，得到$56$后再压入栈中。
因此现在栈顶元素56就是表达式的结果。

后面两张图展示了更多例子。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/6731994fd9654949a17ea7cee0469f62.png)
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/e7d8b32145394e549d648de078c574b4.png)
如果对中缀转后缀之类的转换还不理解，可以看以下视频。
[中缀表达式转前缀/后缀表达式](https://www.bilibili.com/video/BV1aV4y1771G/?spm_id_from=333.1391.0.0&vd_source=3e562ebba9d60af0c036a8e95b29f3c1)

经过前面的学习我们现在可以总结以下后缀表达式的优点：
1.在后缀表达式中，没有运算符优先级的概念，因为运算符总是跟在它所操作的操作数之后。这意味着表达式中的运算符从左到右的顺序就是它们被执行的顺序。
2.后缀表达式实际上模仿了我们计算“通常”（即中缀）表达式的方式。在中缀表达式中，我们从左到右读取表达式，遇到运算符时，按照从左到右的顺序应用之前的两个操作数。
3.后缀表达式消除了使用括号的需要（前提是我们不会将减法运算符与负数中的“-”符号混淆），因为运算符的顺序已经由它们在表达式中的位置确定。因此，计算机在读取和处理数字时，正确的格式和处理非常重要。

#### 2.1.2.3 迷宫问题等搜索问题
考虑一只被困在迷宫中的老鼠，它试图找到通往出口的路径。迷宫通常可以用二维数组表示，其中每个单元格点可以是通道（通常用0表示）或墙（用1表示）。
如图所示。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/24baef1a76a24eb7b6c84e7cd1d2bead.png)
我们现在利用栈写一个程序来解决关于下面这个简单迷宫问题。

```
exitMaze()
initialize stack, exitCell, entryCell, currentCell = entryCell;  
while currentCell is not exitCell
	mark currentCell as visited;
	push onto the stack the unvisited neighbors of currentCell;
	If stack is empty
		failure;
	else pop off a cell from the stack and make it  currentCell;
success;
```
迷宫如下。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/ce377b7c833c4e0b97286ca8abca8478.png)
下图展示了用刚刚的代码解决这个问题的过程。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/92cbc99531984beebab5bfc6083e44ae.png)
m表示老鼠位置，老鼠刚开始位于（3，3），不是终点，因此将其标为来过的，然后将周围的未来过的地方压进栈，即（2，3）和（3，2）。
因此我们接下来推出一个新的位置作为当前老鼠的位置，因此老鼠当前位置是（3，2），不是终点，因此将其标为来过的，然后将周围的未来过的地方压进栈，即（2，2）和（3，1）。
我们接下来再推出一个新的位置作为当前老鼠的位置，因此老鼠当前位置是（3，1），不是终点，因此将其标为来过的，然后将周围的未来过的地方压进栈，即（2，1）。
我们接下来再推出一个新的位置作为当前老鼠的位置，因此老鼠当前位置是（2，1），不是终点，因此将其标为来过的，然后将周围的未来过的地方压进栈，即（2，2）。
我们接下来再推出一个新的位置作为当前老鼠的位置，因此老鼠当前位置是（2，2），不是终点，因此将其标为来过的，然后将周围的未来过的地方压进栈，即（2，3）。
我们接下来再推出一个新的位置作为当前老鼠的位置，因此老鼠当前位置是（2，3），不是终点，因此将其标为来过的，然后将周围的未来过的地方压进栈，即（1，3）和（2，4）。
我们接下来再推出一个新的位置作为当前老鼠的位置，因此老鼠当前位置是（2，4），是终点，可以逃出迷宫。
## 2.2 队列（Queues）
队列是一种遵循先进先出（First-In, First-Out）原则的数据结构，类似于我们在现实世界中使用的队列，如排队等候服务。
同样我们可以在任何适合再队列的尾部（rear）插入对象，这种操作通常称为入队（enqueue）。
但是只有队列首部（front）的元素可以被移除，这种操作通常称为出队（dequeue）。
元素从队列的尾部进入，从队列的前部被移除。
一个常见的队列应用示例是打印机任务队列。多个打印任务被发送到打印机，它们按照到达的顺序排队等候打印。

### 2.2.1 相关方法
队列（Queues）作为一种抽象数据类型（Abstract Data Type，简称 ADT），下面列出其支持的一些基本操作和方法。
1.enqueue(Obj)：这个方法用于在队列的尾部（rear）插入一个对象（Obj）
2.dequeue()：这个方法用于移除并返回队列首部（front）的对象。如果队列为空，则此操作会触发错误。
因此队列这种数据结构需要包含指向头部（head）和尾部（tail）的指针或引用，以便有效地执行入队（enqueue）和出队（dequeue）操作。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/cf8a7e5a1df441aabc112c92dff8c5f4.png)
头部指针指向第一个元素，因为我出队是要返回队列首部的对象。而尾部指针指向最后一个元素的后一个位置，因为我入队是要在尾部插入一个新的对象。

3.size()：返回队列中对象的数量。
4.isEmpty()：如果队列为空，则返回 true；否则返回 false。
5.isFull()：如果队列已满（达到其容量限制），则返回 true；否则返回 false。
6.front()：返回但不移除队列首部的对象。如果队列为空，则此操作会返回错误。可以用于查看队列前端的元素，而不改变队列的状态。

下图展示了一个队列的例子。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/a6657314a95b4e4bb45fa662ad4a2e10.png)
刚开始头部和尾部指针一致。将$3$入队后，插入的位置就是原来尾部指针的位置，插入后。头部指针指向$3$，而尾部指针指向最后一个元素（$3$）的下一个。
再将$7$入队后，尾部指针因此又向后移动一个。
再将$8$入队后，尾部指针因此又向后移动一个。
执行出队后，移除头部指针指向的元素，并返回该元素，即移除和返回$3$,在将头部指针向后移动一个。
将$1$入队，在尾部指针的位置插入$1$，再将指针向后移动一个。
执行出队后，移除头部指针指向的元素，并返回该元素，即移除和返回$7$,在将头部指针向后移动一个。
执行出队后，移除头部指针指向的元素，并返回该元素，即移除和返回$8$,在将头部指针向后移动一个。

### 2.2.2 实践
#### 2.2.2.1 循环队列（Circular Queue）
循环队列是一种队列的实现方式，它使用一个固定大小的数组来存储队列中的元素，并使用两个指针来分别追踪队列的前端和后端。当队列满时，新元素会覆盖最早进入队列的元素，从而实现循环利用数组空间。
如下图所示。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/9af045e2c3c7460a8a39d5e3d420b70e.png)

在循环队列中，当尾部指针到达数组末尾时，它会环绕到数组的开头，这就是“循环”一词的由来。其的优点便是有效地使用固定大小的数组空间，避免了因队列增长而需要的动态数组扩容。

#### 2.2.2.2 多线程编程（Multithreading）
我们在操作系统中学习了多线程编程的概念，队列最大的应用便是利用队列来实现线程间的CPU时间分配。
多线程编程是一种实现有限形式的并行性（parallelism）的方法，其允许多个任务或线程同时运行。
例如：计算机（或程序）可能使用多个线程，其中一个线程负责捕获鼠标点击，另一个线程可能负责在屏幕上绘制动画。
在设计使用多个线程的程序（或操作系统）时，我们必须确保单个线程不会独占CPU。
一种解决方案是使用队列来以轮询（round-robin）协议分配CPU时间给线程，即我们可以使用一个队列来保存线程集合。队列开头的线程被移除，分配一部分CPU时间，然后被放回队列的尾部。

## 2.3 列表（List）
列表是一种数据结构，由一系列项（items）组成，每个项存储在一个节点（node）中。每个节点包含一个数据字段（用于存储数据）和一个指向列表中下一个元素的指针。
与前面的数据结构的不同在于，数据可以通过在列表中的任意位置插入新节点并重新分配指针来插入到列表中，因此数据不仅可以随时插入，还可以在任意位置插入。
列表ADT支持引用（访问特定位置的元素）、更新（包括插入和删除操作）以及搜索方法。
列表ADT可以被实现为单链表或双链表（这一点在数据结构课上有详细说明）。
单链表（Singly-linked list）：每个节点包含数据字段和指向下一个节点的指针。
双链表（Doubly-linked list）：每个节点包含数据字段和两个指针，一个指向下一个节点，另一个指向前一个节点。

### 2.3.1 相关方法
1.first()：返回列表中第一个元素的位置。如果列表为空，则操作会触发错误。
2.last()：返回列表中最后一个元素的位置。如果列表为空，则操作会触发错误。
3.isFirst(p)：如果元素 p 是列表中的第一个元素，则返回 true，否则返回 false。
4.isLast(p)：如果元素 p 是列表中的最后一个元素，则返回 true，否则返回 false。
5.before(p)：返回列表中位置 p 之前的那个元素的位置。如果 p 是第一个元素，则操作会触发错误，因为第一个元素之前没有其他元素。
6.after(p)：返回列表中位置 p 之后的那个元素的位置。如果 p 是最后一个元素，则操作会触发错误，因为最后一个元素之后没有其他元素。
7.replaceElement(p,e)：将位置 p 处的元素替换为新元素 e。
8.swapElements(p,q)：交换位置 p 和 q 处的元素。
9.insertFirst(e)：在列表的开头插入新元素 e。
10.insertLast(e)：在列表的末尾插入新元素 e。
11.insertBefore(p,e)：在位置 p 之前插入新元素 e。
12.insertAfter(p,e)：在位置 p 之后插入新元素 e。
13.remove(p)：移除位置 p 处的元素。

### 2.3.2 实践
#### 2.3.2.1 单链表（Singly-linked list）
单链表是一种常见的数据结构，由一系列节点（nodes）组成，每个节点包含数据元素和指向列表中下一个节点的链接（next link）。每个节点中的链接指向列表中的下一个元素。如果一个元素是列表的最后一个元素，那么它的链接是 null，表示没有后续元素。
下图展示了一个节点的组成。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/db889fee26424da289162e0f405dd650.png)
下图展示了一个单链表。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/fb2fe6c212d441d6bea8f510a636e5ee.png)

#### 2.3.2.2 双链表（Doubly-linked list）
双链表与单链表的区别是多存储了一个链接，原来的链接叫做next链接，额外储存的是指向前一个元素的prev链接。
因此它为列表ADT提供了一种直观且高效的实现方式。
所以现在一个节点的组成如下：
元素（Element）：存储实际的数据。
前一个节点的链接：指向前一个节点的链接。
下一个节点的链接：指向下一个节点的链接。
下图展示了一个节点的组成。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/df31066c748a468ebf1150a131159217.png)
但是我们这里有两个特例，即头部和尾部的节点该怎么处理，我们可以直接将第一个节点的prev链接设置为null，最后一个节点的next链接设置为null。当然也可以采用下面的方案。
专门多两个特殊节点：
1.头节点（Header nodes）：通常位于列表的开始位置，用作列表的入口点。头节点可能不存储任何实际的数据元素，或者存储一个特殊值，用于标识列表的开始。
2.尾节点（Trailer nodes）：位于列表的末尾，用于标识列表的结束。尾节点的 next 链接通常设置为 null，表示没有更多的节点跟随其后。
因此一个双链表如下所示。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/44212b3747b14ff5872c2d3f606e29ea.png)

我们一般使用的都是双链表，所以我们接下来看一下双链表如何实现前面说的一些基本操作。
插入元素操作如下图所示，执行了insertAfter(1,e)。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/51c2f5252b1345abb0538ec194c1953d.png)
我们找到插入的位置后，然后创建一个新节点，然后其元素储存对应的值。然后prev链接指向前一个节点，next链接指向下一个节点。最后更新前一个节点的next链接和后一个节点的prev链接使它们指向新节点。

该操作的伪代码如下。
```
INSERTAFTER(p,e)
 //Create a new node v
v.element ←e
 //Link v to its predecessor
v.prev ← p
 //Link v to its successor
v.next ←p.next
 //Link p’s old successor to v
(p.next).prev ← v
 //Link p to its new successor v
p.next ←v
return v
```
下图是代码运行过程的解释，数字代表代码的行数。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/0bab5eb7dfb64117b23336c080e88f86.png)
注意这里的顺序不能先修改原来的链表的链接，否则我们会找不到下一个节点。

说完插入元素，我们说一下移除元素。
下图展示了执行remove(2)的结果。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/befd13e76a3b47c8abc9250246565d86.png)
首先找到第二个元素“Greece”然后调整前一个节点的next链接，直接指向“Greece”的下一个节点。然后“Greece”的下一个节点的prev链接指向“Greece”的前一个节点。最后释放或删除“Greece”节点所占用的内存。
同样，这里如果先删除“Greece”指向下一个节点的next链接会导致找不到“Greece”的下一个节点。

该操作的伪代码如下。
```
REMOVE(p)
 //Assign a temporary variable to hold returnvalue
t ←p.element
 //Unlink p from list
(p.prev).next ← p.next
(p.next).prev ← p.prev
 //invalidatep
p.prev ←null
p.next ←null
return t
```

下图是代码运行过程的解释，数字代表代码的行数。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/f70679978fdc4191b97ed8f80a8918ec.png)

## 2.4 根树（Rooted Tree）
根树 T 是一种树形数据结构，由一组节点组成，这些节点以父子关系（parent-child relationship）相互连接。
在根树 T 中，有一个特殊的节点 r，称为树的根（root）。根节点是树的起始点，s所以没有父节点。
树中的每个节点（除了根节点）都有一个父节点（parent node）。父节点指向其子节点，子节点指向其父节点。
下图展示了一个根树。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/f01bfbb4b3fe4a7aa4703b3fb988b6d5.png)
### 2.4.1 相关术语（Terminology）
1.父节点和子节点（Parent和Child）：如果节点 u 是节点 v 的父节点，那么 v 就是 u 的子节点。
2.兄弟节点（Siblings）：如果两个节点是同一个父节点的子节点，那么这两个节点互为兄弟节点。
3.叶节点（Leaf或External Node）：如果一个节点没有子节点（即没有孩子），那么这个节点就是叶子节点或外部节点。
4.内部节点（Internel Node）：如果一个节点有子节点（即至少有一个孩子），那么这个节点就是内部节点。
5.有序树（Ordered Tree）：如果树中每个内部节点的子节点都有一个定义良好的线性顺序（即每个内部节点都有一个明确的第一子节点、第二子节点等），那么这棵树就是有序的。有序树允许我们按特定顺序访问或遍历子节点，例如，先访问第一个子节点，再访问第二个子节点，依此类推。

### 2.4.2 二叉树（Binary Trees）
二叉树是一种特殊的有序树：它是一种有根的有序树。在二叉树中，每个节点最多有两个子节点，通常称为左子节点（left child）和右子节点（right child）。
完全二叉树（Proper Binary Tree）：如果二叉树中的每个内部节点都恰好有两个子节点，则称这棵二叉树为完全二叉树。

### 2.4.3 相关方法
#### 2.4.3.1 访问方法
1.root()：返回树的根节点。
2.parent(v)：返回节点 v 的父节点。
3.children(v)：返回指向节点 v 的子节点的链接。

#### 2.4.3.2 查询方法
1.isInternal(v)：测试节点 v 是否为内部节点（internal node）。
2.isExternal(v)：测试节点 v 是否为外部节点（external node）。
3.isRoot(v)：测试节点 v 是否为根节点。

#### 2.4.3.3 通用方法
1.size()：返回树中节点的数量。
2.elements():返回树中所有元素的列表。
3.positions()：返回所有元素地址的列表。
4.swapElements(u,v)：交换位置 u 和 v 处存储的元素。
5.replaceElements(v,e)：用元素 e 替换位置 v 处的元素。

### 2.4.4 实践
#### 2.4.4.1 节点的深度
节点的深度是指从根节点到该节点的路径长度，即从根节点开始，经过的边（或链接）的数量。下面利用伪代码展示利用递归如何计算节点的深度。

```
DEPTH(T,v)
if T.isRoot(v)
then return 0
else return 1 +DEPTH(T, T.parent(v))
```
如果节点 v 是树 T 的根节点（T.isRoot(v) 返回 true），则 v 的深度为 0。如果节点 v 不是根节点，那么它的深度是其父节点的深度加 1（return 1 + DEPTH(T, T.parent(v))）。这里 T.parent(v) 返回节点 v 的父节点，然后递归地计算父节点的深度。

#### 2.4.4.2 树的高度
树的高度等同于树中叶子节点的最大深度。下面的伪代码计算了以节点 v 为根的子树的高度。

```
HEIGHT(T,v)
if ISEXTERNAL(v)
	then return0
else
 	h = 0
	for each w ∈T.CHILDREN(v)
 		do
 			h = MAX(h,HEIGHT(T,w))
 	return 1 + h
```
检查节点 v 是否为叶子节点（即没有子节点的外部节点）。如果节点 v 是叶子节点（IS_EXTERNAL(v) 返回 true），则返回 0，因为叶子节点的高度为 0。然后初始化变量 h 为 0。这个变量将用于存储子树的最大高度。再用递归计算子树的高度遍历节点 v 的所有子节点 w，对每个子节点 w，递归地调用 HEIGHT(T, w) 来计算其高度，使用 MAX(h, HEIGHT(T, w)) 来更新 h，确保 h 存储的是目前为止找到的最大高度。最后返回 1 + h，因为树的高度是其子树中最大高度加 1（根节点的高度至少为 1）。

#### 2.4.4.3 树遍历（Tree Traversal）
树遍历是一种对树中所有节点按某种顺序进行访问并执行操作的过程。遍历的目标是确保每个节点都被访问一次，并且可以对每个节点执行特定的操作。
尽管遍历和搜索听起来相似，它们的目的和应用场景可能有所不同。
遍历：指按照某种系统化的顺序访问树中的所有节点，例如打印节点值、收集信息或执行某种操作。
搜索：指查找特定节点或值，例如在二叉搜索树中查找最小或最大值。

二叉树支持以下三种遍历方式：
1.前序遍历（Preorder Traversal）：
访问顺序：根节点 → 左子树 → 右子树。
2.后序遍历（Postorder Traversal）：
访问顺序：左子树 → 右子树 → 根节点。
3.中序遍历（Inorder Traversal）：
访问顺序：左子树 → 根节点 → 右子树。

##### 2.4.4.3.1 前序遍历（Preorder traversal）
在前序遍历中，节点会在其所有后代（descendant，也就是子节点）之前被访问。
其的伪代码如下。

```
Algorithm preOrder(v)
    visit(v)
    for each child w of v
       preOrder(w)
```

可以用于打印结构化文档，如下图所示。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/2df0e29e6b3a4b3e8d01ae065c88f2c3.png)
下图的树如果使用前序遍历。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/fb75d56d16aa4035aaa935932219a8fc.png)
那么遍历的顺序是：A，B，C，D，E，F，G，H，I，J，K.

##### 2.4.4.3.2 后序遍历（Postorder traversal）
在后序遍历中，节点在访问其所有后代（子节点）之后被访问。
其的伪代码如下：

```
Algorithm postOrder(v)
    for each child w of v
       postOrder(w)
    visit(v)
```
后序遍历的一个应用是计算文件目录及其子目录中文件所占用的空间，如下图所示。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/0a90e278996f47da9b0fb6a7af926983.png)
同样的图。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/fb75d56d16aa4035aaa935932219a8fc.png)
遍历的顺序是：D，E，C，F，B，I，J，H，K，G，A.

##### 2.4.4.3.3 中序遍历（Inorder traversal）
在中序遍历中，节点在访问其左子树之后，而在右子树之前被访问。即在左子树和右子树之间被访问。
其的伪代码如下：
```
Algorithm inOrder(v)
    if hasLeft(v)
        inOrder(left(v))
    visit(v)
    if hasRight(v)
        inOrder(right(v))
```
中序遍历的一个应用是绘制二叉树。通过中序遍历，我们可以确定节点的中序排名（inorder rank）和深度（depth）。在二叉搜索树（二叉搜索树和二叉树不同，其在二叉树的基础上将里面的每个节点以左节点小于该节点，右节点大于该节点的顺序排序）中，中序遍历可以生成有序序列。这是因为二叉搜索树的性质保证了左子树的所有节点值都小于根节点，右子树的所有节点值都大于根节点。因此，通过中序遍历，我们可以得到一个从小到大的有序序列。
如下图所示。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/fdcdbaafd3c54bcf8bb0285f6f1c7060.png)
同样的图。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/fb75d56d16aa4035aaa935932219a8fc.png)
遍历的顺序是：D，C，E，B，F，A，I，H，J，G，K.

#### 2.4.4.4 算术表达式
二叉树与算术表达式相关联，其中每个叶节点（external node）是一个变量或常量，每个内部节点（internal node）定义了其两个子节点上的算术运算。
如下图所示。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/75f5e3f42bdc409bbc521bc62a96602d.png)
我们用中序遍历的方式遍历该树就可以获得中缀表达式$(2*(a-1)+(3*b))$。
同理，下图给出了另一个例子。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/b8a48d0981bf4fbba31009f09be408b3.png)
中缀表达式为$((4+7)*6+(11-5)+3)*(8*(4+6)-3)$。

