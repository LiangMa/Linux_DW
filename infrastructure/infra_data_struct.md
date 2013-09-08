#Linux kernel Infrastructure Data Structure     

##List
###特性描述
Linux 中最常用最基本的数据结构， 双向循环链表。 不同于通常的链表实现， Linux 中的 双向循环列表 没有包含节点结构， 而是把 链表的核心结构抽象出来，然后利用 gcc扩展 [containerof](#contianerof) 编译时计算出所在数据结构的偏移量，从而轻易获得整个链表节点的地址
   
     
    
>  **双向循环链表:**      

![alt text](./pics/Linux_List.png "双向循环链表")    



----------   


###API介绍
###实现剖析
###例子


##HList
在Hash table 中使用到的链表结构， 改进自List， 更加节省空间
###特性描述
###API介绍
###例子
```c
#include <linux/list.h>
```
###实现剖析

##KFifo
###特性描述
###API介绍
###例子
###实现剖析

##Read Copy Update 简介
##RCUList
###特性描述
###API介绍
###例子
###实现剖析

##KObject
主要是针对核心的内核数据结构做引用计数， 有强引用和弱引用之分
###特性描述
###API介绍
###例子
###实现剖析


#附录
##GCC Extension 

###ContianerOf 
###TypeOf

##Sparse Checking Tools 


