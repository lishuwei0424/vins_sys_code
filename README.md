![img](file:///image.jpg)
**第七次作业**

![img](file:///C:\Users\lishuwei\AppData\Local\Temp\msohtmlclip1\01\clip_image002.jpg)

**解:**

**分为两部分：仿真数据准备和开源的vins****系统**

**1.****数据准备**

**工具采用的是vio_data_simulation-master**

**a.Param.h****参数的设定为**

![img](file:///C:\Users\lishuwei\AppData\Local\Temp\msohtmlclip1\01\clip_image004.jpg)

外参：

​     ![img](file:///C:\Users\lishuwei\AppData\Local\Temp\msohtmlclip1\01\clip_image006.jpg)

 

**b.****文件格式**

**文件如**

![img](file:///C:\Users\lishuwei\AppData\Local\Temp\msohtmlclip1\01\clip_image008.jpg)

1）imu_pose.txt 与imu_pose_noise.txt: （imu数据）

每一行：时间戳，陀螺仪向量，加速度计向量

2）image_filename.txt（图像名文件）

每一行：时间戳，一帧图像名字

3）cam_pose.txt(图像实际的姿态)

每一行：x,y,z

**c.****最后系统的配置文件为：**

myslam_config.yaml

![img](file:///C:\Users\lishuwei\AppData\Local\Temp\msohtmlclip1\01\clip_image010.jpg)

![img](file:///C:\Users\lishuwei\AppData\Local\Temp\msohtmlclip1\01\clip_image012.jpg)

​       

**2.****开源vins**

**a.imu****数据输入**

 

![img](file:///C:\Users\lishuwei\AppData\Local\Temp\msohtmlclip1\01\clip_image014.jpg)

**b.****图像数据输入**

![img](file:///C:\Users\lishuwei\AppData\Local\Temp\msohtmlclip1\01\clip_image016.jpg)

![img](file:///C:\Users\lishuwei\AppData\Local\Temp\msohtmlclip1\01\clip_image018.jpg)

 

**c.****真实数据的显示（groudturth****）**

![img](file:///C:\Users\lishuwei\AppData\Local\Temp\msohtmlclip1\01\clip_image020.jpg)

 

d．可视化处理

![img](file:///C:\Users\lishuwei\AppData\Local\Temp\msohtmlclip1\01\clip_image022.jpg)

 

**有噪声的数据运行结果如图（dift****）：**

![img](file:///C:\Users\lishuwei\AppData\Local\Temp\msohtmlclip1\01\clip_image024.jpg)

 

 

 

**无噪声的数据运行结果如图：**

![img](file:///C:\Users\lishuwei\AppData\Local\Temp\msohtmlclip1\01\clip_image026.jpg)

 

 