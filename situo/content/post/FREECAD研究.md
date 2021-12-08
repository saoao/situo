# FREECAD研究

## 编译准备

1. 从码云下载最新的源码镜像，地址：https://gitee.com/tinysik/FreeCAD.git

2. freecad第三库依赖库较多，官方提供libpack压缩包供编译使用，下载地址：

   文件名：FreeCADLibs_12.1.4_x64_VC15.7z

   链接：https://pan.baidu.com/s/1xyCGNyMtwtnEYZo3bgE40Q 
   提取码：st88

3. 下载cmake，本地教程使用3.14.3版本，可以使用更高版本。

4. 下载vs2017，地址：ed2k://|file|mu_visual_studio_professional_2017_version_15.3_x86_x64_11100064.exe|1069960|900673A59F0798822207F72FAA0DA6A9|/

## 开始编译

cmake配置：

![image-20200802143844596](C:\Users\Zhejun\AppData\Roaming\Typora\typora-user-images\image-20200802143844596.png)

注意勾选上图红框中的选项，以便程序运行时找到相关的dll。

![image-20200802144149179](C:\Users\Zhejun\AppData\Roaming\Typora\typora-user-images\image-20200802144149179.png)

使用qt5编译，libpack下自带的是qt5.12.1。

![image-20200802145021738](C:\Users\Zhejun\AppData\Roaming\Typora\typora-user-images\image-20200802145021738.png)

![image-20200802145224944](C:\Users\Zhejun\AppData\Roaming\Typora\typora-user-images\image-20200802145224944.png)

值填写pyside2 platforms的实际地址。例如：***D:\DEV\OpenSource\FreeCADLibs_12.1.4_x64_VC15***\bin\Lib\site-packages\PySide2\plugins\platforms，加粗的部分为实际的libpack安装路径。

![image-20200802144735265](C:\Users\Zhejun\AppData\Roaming\Typora\typora-user-images\image-20200802144735265.png)

设置"FreeCADMain"为启动项目。

等待编译完成。













