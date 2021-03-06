##  Introduction

- Principle of Locality (局部性原理，区域性原则)
  - Programs access a small proportion of their address space at any time 程序可随时访问其地址空间的一小部分
  - Temporal locality [计] 时间局部性
    - Items accessed recently are likely to be accessed again soon 最近访问的项目可能很快就会再次访问
    - e.g., instructions in a loop, induction variables
  - Spatial locality [计] 空间局部性
    - Items near those accessed recently are likely to be accessed soon 最近访问过的项目附近的项目可能很快就会被访问
    - E.g., sequential instruction access, array data 例如，顺序指令访问，数组数据
  
![](img/2020-11-23-22-15-21.png)


- **Temporal locality** 时间局部性: The locality principle stating that if a data location is referenced then it will tend to be referenced again soon.

- **Spatial locality** 空间局部性: The locality principle stating that if a data location is referenced, data locations with nearby addresses will tend to be referenced soon.

![](img/2020-11-23-23-01-42.png)  

---

- **Memory hierarchy** 分级存储器体系: A structure that uses multiple levels of memories; as the distance from the processor increases, the size of the memories and the access time both increase.


- **Block (or line)**: The minimum unit of information that can be either present or not present in a cache.


![](img/2020-11-23-23-19-48.png)

![](img/2020-11-23-23-22-52.png)

![](img/2020-11-23-23-22-11.png)

![](img/2020-11-23-23-23-54.png)

![](img/2020-11-23-23-25-24.png)

![](img/2020-11-24-02-49-34.png)

![](img/2020-11-24-02-53-12.png)

---

![](img/2020-11-24-02-50-53.png)

![](img/2020-11-25-14-00-13.png)

![](img/2020-11-25-14-03-47.png)

---

- **Hit rate** [计] 命中率: The fraction of memory accesses found in a level of the memory hierarchy.
- **Miss rate**  : The fraction of memory accesses not found in a level of the memory hierarchy.

- **Hit time**: The time required to access a level of the memory hierarchy, including the time needed to determine 
  whether the access is a hit or a miss.
  - Hit time is the time to access the upper level of the memory hierarchy, which includes the time needed to determine 
    whether the access is a hit or a miss (that is, the time needed to look through the books on the desk). 

- **Miss penalty** 缺失损失): The time required to fetch a block into a level of the memory hierarchy from the lower 
  level, including the time to access the block, transmit it from one level to the other, insert it in the level that 
  experienced the miss, and then pass the block to the requestor.
  - The miss penalty is the time to replace a block in the upper level with the corresponding block from the lower 
    level, plus the time to deliver this block to the processor (or the time to get another book from the shelves and 
    place it on the desk).

![](img/2020-11-25-14-16-26.png)

![](img/2020-11-25-17-51-41.png)

![](img/2020-11-25-18-04-49.png)








