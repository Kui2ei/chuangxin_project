# **卜凡臻202000460039独立完成**

# 最长36bit

**运行指导：**

这个python文件用编辑器打开，其中的参数a是我们需要碰撞的长度（单位是4bit），初始值设置的为5（20bit），运行即开始查找碰撞。

**项目说明：**

生日攻击，就是选取所要攻击的长度的一半来进行穷举攻击，代码比较简单。
一开始编写的代码较为简陋，内存利用率不高，如下图：

![This is an image](https://github.com/Bufanzhen/chuangxin_project/blob/main/SM3/the%20na%C3%AFve%20birthday%20attack%20with%20python/%E5%9B%BE%E7%89%87.png)
在跑7个十六进制数的时候，发生了内存过大的问题：

![图片](https://user-images.githubusercontent.com/71548447/181870162-9b4c5216-2787-4922-bd54-adcc5fa51691.png)

之后进行改进，采用边算边查，如果有碰撞就停止，可以减少内存使用，用时247.3s，成功找出了36bit的碰撞。如下图

![图片](https://user-images.githubusercontent.com/71548447/181870497-5d451dbf-cb56-421f-9eae-6cc335eaeee9.png)

