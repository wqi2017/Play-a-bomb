本程序是微信小游戏弹一弹的辅助。

平台：win10       visual studio 2013     opencv3.0.0

首先用adb工具对手机屏幕进行截图，然后读取该截图，用Opencv处理找到最上面的方块的中心，再使用adb模拟屏幕点击该中心。

缺点：没有考虑到子弹撞击的反弹，没有对方块内的数字进行识别，无法确定每次发弹的时间间隔

![image](https://github.com/wqi2017/-/blob/master/%E5%BC%B9%E4%B8%80%E5%BC%B9_%E7%8E%8B%E7%90%A6/%E5%BC%B9%E4%B8%80%E5%BC%B9_%E7%8E%8B%E7%90%A6/%E7%AC%AC%E4%B8%80%E6%AC%A1%E6%88%90%E7%BB%A9.png)

7-11:更新
    1.确定发弹间隔
    方法：根据屏幕中是否存在子弹确定是否点击屏幕
    2.更新为linux平台,使用cmake编译
    3.增加问题：自动点击加速未成功
