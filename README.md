# SM4_Multhread

1、代码原理：有关SM4代码的阐述如下图所示，在这里不对函数的定义做过多介绍，只在软件加速方面进行更多补充。

![image](https://user-images.githubusercontent.com/108848022/181264435-284228cc-90e8-4f40-91af-c6f1d3d81d84.png)

![image](https://user-images.githubusercontent.com/108848022/181264692-5f02c42a-d76f-4ecf-ae9b-b30a16182f88.png)

![image](https://user-images.githubusercontent.com/108848022/181264726-86299d73-2740-4213-b8a4-1bb3c6b59ae9.png)


2、在本任务中介绍有关利用多线程加速SM4算法，函数截图如下图所示：

![image](https://user-images.githubusercontent.com/108848022/181265331-78850334-a017-4371-bec8-f69470bec41c.png)

3、有关多线程加速SM4算法的原理解释：

![image](https://user-images.githubusercontent.com/108848022/181265330-d5c02b83-dc22-4f34-a6dc-dd7aaa438ead.png)

4、有关main函数的代码复现：

![image](https://user-images.githubusercontent.com/108848022/181265516-bce123f8-b93f-45eb-b094-141b0583a16b.png)

在main函数中，我们计算原始SM4算法和多线程下SM4算法的时间来判断多线程软件加速方法的加速比，有关不同数据量下加速比的对比情况如下图所示：

![image](https://user-images.githubusercontent.com/108848022/181266284-38bb8a27-dba9-43b1-b74f-de077c9b53f7.png)

可以明显看出随着数据量级越来越大，显然在多线程下计算SM4算法的速率明显更快，且加速比始终保持在一个较高的区间内，说明多线程能够很大程度上在软件层面加速SM4运算速度。
