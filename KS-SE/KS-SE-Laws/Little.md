# 里特定律 （Little's Law）
```md
Little's Law 是排队论里面的理论，只要现实问题中有排队的结构就可以考虑应用Little's Law。
这里说的排队不一定要满足任何像先进先出或者先进后出的规则，
队伍还不一定需要有顺序，关键是有一个系统（或者叫成空间也行）能容纳个体，个体有进有出就行。
```
```md
Little's law 是一个数学定理，只要满足前提条件 L = λW 就一定是对的，因为每一步都是通过严格数学推理的。
```
* L = λW
```md
一个排队系统在稳定状态下，在系统里面的个体的数量的平均值 L，等于平均个体到达率λ （单位是 个每单位时间）乘以个体的平均逗留时间W。
```
```md
1. 稳定状态
    可以直观理解成系统的状态在均值上或者说在某个时间点开始不怎么变了，
    每段时间的平均个体数目不会忽大忽小，每段时间的到达率的平均值不会忽高忽低，平均逗留时间不会忽长忽短。
2. 平均是长期时间上的平均
    个体总数平均值就是一段时间里面个体的总数除以这段时间长度。

稳定状态保证平均值的存在。各种工业系统一般都处于稳定状态的。
```

## 使用条件
```md
1. 开始和结束的时候系统是空的。
2. 个体不会凭空消失。
```
## 应用
```md
1. 产品排队进库存。排队论在库存管理里头的应用。
2. 顾客到百货商场买商品。百货商场是系统，顾客是个体。
3. 网民进入google网站，然后点链接离开。google这个网站是系统，网名是个体。
4. 我们回复email。邮箱是系统，邮件是个体，收到邮件表示邮件进入，我们回了邮件表示邮件离开。
5. 孕妇住院。医院是系统，孕妇是个体，准备要生的时候进入医院。生完休息护理完毕离开。
6. 中介卖楼。中介是系统，要卖楼的单子进入系统，楼被买掉了或者不卖了单子离开。
```
### IT
* 性能压力测试，开始时，压力压不上去
```md
N = X * E[T] ，N就是你的压力器线程数＊IODepth，X 是 IOPS ，E[T]是平均处理时间 
压不上去两个原因 1. N太小 2. E[T]太大
```