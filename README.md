# YFLY

​	列位好，我是耀风居士（很久之前起的，本来是叫“要疯”，后面疯着疯着再加了个居士，美化了下就是现在的名字，哈哈哈哈），这是我的第一个作品，希望认识更多的同道中人，一起讨论学习，“掀起一波浪花”。

​	本人是飞控的爱好者，初级业余飞控开发者，本作品也是第一次软硬件完全开发，难免有多多少少的美观性，合理性，逻辑性的问题，如有问题，还望各位道友不吝赐教。

  项目演示视频（必看！小弟很用心剪的，哈哈哈哈）：
  【【自制】F405飞控(开发记录)】https://www.bilibili.com/video/BV1bE2cYkEQF?vd_source=94e46f229dcdb63fc73a8a9f4ef7f09a

​	<img src=".\picture\整机2.jpg" style="zoom:15%;" />




# 参数

- 主控：STM32F405RGT6
- IMU：MPU9250（加速度计/陀螺仪/磁力计）
- 气压计：SPL06
- GPS：M8N（内置HMC5883L磁力计）
- 黑匣子：TF卡
- 光流接口：支持正点原子光流模块
- 扩展接口：SPI x 1 ; UART x 2
- 解码：PPM/SBUS编码
- 数传：单纯的串口（本人使用的是无线仿真器，有仿真和串口功能）
- 支持地面站：匿名地面站/QGC

<img src=".\picture\板子.png" style="zoom:60%;" />

【晶振旁跳线的由来】因为图快，用了AD的自动布线，但是没想到被坑了，晶振的地线没有连，而且DRC检测还没有检测出来！！（手动捂脸）

# 调参

支持匿名地面站进行PID调参

<img src=".\picture\PID.png" style="zoom:50%;" />

# 开源

目前只开源硬件部分，后续关注的人多的话，再开源软件部分代码。

# 后续开发

- 添加图传功能
- 开发数传模块
- 开发自动巡航功能
- 完全支持QGC地面站
- 开发飞控Linux大脑，准备适配计算机视觉导航
- 美化布局，手动布线
- 整理代码，优化效率
