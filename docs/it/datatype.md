# 常见数据结构

## 链表
- 链表是一种物理存储单元上非连续、非顺序的存储结构，数据元素的逻辑顺序是通过链表中的指针链接次序实现的。链表由一系列结点（链表中每一个元素称为结点）组成，结点可以在运行时动态生成。每个结点包括两个部分：一个是存储数据元素的数据域，另一个是存储下一个结点地址的指针域。 相比于线性表顺序结构，操作复杂。由于不必须按顺序存储，链表在插入的时候可以达到O(1)的复杂度，比另一种线性表顺序表快得多，但是查找一个节点或者访问特定编号的节点则需要O(n)的时间，而线性表和顺序表相应的时间复杂度分别是O(logn)和O(1)。
!['linked'](/imgs/dataype/b-26.jpg)
## 数组
- 所谓数组，是有序的元素序列。
    - 若将有限个类型相同的变量的集合命名，那么这个名称为数组名。组成数组的各个变量称为数组的分量，也称为数组的元素，有时也称为下标变量。用于区分数组的各个元素的数字编号称为下标。数组是在程序设计中，为了处理方便， 把具有相同类型的若干元素按无序的形式组织起来的一种形式。 
    - 这些无序排列的同类数据元素的集合称为数组。
  数组是用于储存多个相同类型数据的集合。
- 链表操作快，读取慢
- 数组读取快，操作慢

## 栈
- 栈（stack）又名堆栈，它是一种运算受限的线性表。限定仅在表尾进行插入和删除操作的线性表。这一端被称为栈顶，相对地，把另一端称为栈底。向一个栈插入新元素又称作进栈、入栈或压栈，它是把新元素放到栈顶元素的上面，使之成为新的栈顶元素；从一个栈删除元素又称作出栈或退栈，它是把栈顶元素删除掉，使其相邻的元素成为新的栈顶元素。
- 后进先出，先进后出 **Last In First Out， LIFO**

## 队列
- 先进先出，后进后出 **First In First Out FIFO**


## 堆
- 堆是一种图的树形结构，被用于实现“优先队列”（priority queues）（树形结构的详细讲解
  在 4-2 节）。优先队列是一种数据结构，可以自由添加数据，但取出数据时要从最小值开始按顺
  序取出。在堆的树形结构中，各个顶点被称为“结点”（node），数据就存储在这些结点中。

## 二叉查找树
- 二叉查找树（又叫作二叉搜索树或二叉排序树）是一种数据结构，采用了图的树形结构。数据存储于二叉查找树的各个结点中。
- 每一个节点最多有两个子节点

## 红黑树
- 红黑树（Red Black Tree） 是一种自平衡二叉查找树，是在计算机科学中用到的一种数据结构，典型的用途是实现关联数组。
- 它是在1972年由Rudolf Bayer发明的，当时被称为平衡二叉B树（symmetric binary B-trees）。后来，在1978年被 Leo J. Guibas 和 Robert Sedgewick 修改为如今的“红黑树”。
  红黑树和AVL树类似，都是在进行插入和删除操作时通过特定操作保持二叉查找树的平衡，从而获得较高的查找性能。
- 它虽然是复杂的，但它的最坏情况运行时间也是非常良好的，并且在实践中是高效的： 它可以在O(log n)时间内做查找，插入和删除，这里的n 是树中元素的数目。
- 二叉树如果数组是递增形式，那么单边增长的形式
- 红黑树，结构着完整`完美二叉树`的方式调整