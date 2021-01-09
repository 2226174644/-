# calculator
QT编写 一元稀疏多项式计算器-数据结构课设

1.任务陈述
一元稀疏多项式在计算器中被表示为一个整数序列，其中ci，ei，分别是第i项的系数和指数，序列按指数降序排序。系统用于计算多项式加减，在输入多项式A和B后，能做到求和，求差，输出结果。

2.任务目标
实现如下目标：
一：显示计算器的界面模块
二：根据用户的输入的数据创建多项式
三：设计多项式加、减操作供用户选择。
四：根据用户选择的操作输出结果。
五：将上述四个模块对应至一个主函数。

3.实现功能：
一元稀疏多项式简单计算器的基本功能是：
（1）1.需要用户输入多项式A和B。
（2）2.需要用户选择加、减操作。
（3）3.实现对应功能，输出结果。
（4）可清空输入框中的数据

4.算法思想：
输入字符串形式的多项式A和B.
Build()函数先检测字符串合法性，合法则将字符形式的多项式转换为char类型数组。用检索每一项的系数和指数新建节点并加入尾节点。检索完毕后进行合并和排序。
选择加减操作后进入计算程序。与建立多项式类似，把A和B多项式存入新链表C,继续合并和排序。最后进行格式化输出。
（合并算法：从单链表中的第一项开始，将其与之后的每一项进行指数对比，若指数相等，则进行系数相加，并从单链表中删除所加项。第一项遍历完所有项后重新开始从第二项开始遍历，依此类推直至结束。）
