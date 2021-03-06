# ICP 点云配准算法
## 一、环境
PCL 1.8.1

## 二、效果

`pc_registration.exe`可以实现键盘控制每次ICP迭代，按空格执行下一次迭代，按q退出。

<p align="center"><img src="./result/result.png" width=50% height=50%></p>

<h6 align="center">运行结果</h6>



ICP point-to-point算法对点云密度差不不大时配准效果较好(和初始点选择有关)，而当点云密度差距较大时不能很好的配准，容易卡在一个鞍点或局部极小点上。因此ICP算法有许多改良版本，包括point-to-plane、plane-to-plane、generalized-ICP算法等，ICP算法更详细的介绍见[./docs](./docs/ICP.ipynb)

## 三、安装

```
git clone git@github.com:GCaptainNemo/ICP-registration-PCL.git 
cd ICP-registration-PCL/Project1
mkdir build
cd build && cmake ..
```

## 三、参考资料

[1] [csdn-ICP原理与PCL代码实现](https://blog.csdn.net/qq_29462849/article/details/85080518)

[2] [github-ICP点云配准](https://github.com/seven-linglx/icp)

 







