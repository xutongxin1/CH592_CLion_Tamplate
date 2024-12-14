# 这是一个CH592的工程模板

如何使用：

1. 确保安装好了原厂的MRS，确保你的单片机原厂可以下载

   ![image-20241214180835173](http://github.xutongxin.me/https://raw.githubusercontent.com/xutongxin1/PictureBed/master/2024After/image-20241214180835173.png)

2. 解压CH592Lib.zip到该文件夹的上一级，这样可以使你的多个项目都共同引用这些简单的依赖

   ![image-20241214180726640](http://github.xutongxin.me/https://raw.githubusercontent.com/xutongxin1/PictureBed/master/2024After/image-20241214180726640.png)

   （注：CH592库不会自己更新，目前是2024.12.14的最新版但不保证未来是否会更新，如果官网更新请自行下载资源包进行替换更新）

3. 打开CLion加载cmake，和stm32一样，CLion中所选择的工具链不重要，你需要在环境位置增加环境变量

```
Path=C:\Path\MounRiver\MounRiver_Studio\toolchain\RISC-V Embedded GCC\bin\
```

4. Enjoy！



## Q&A：

### Q:都是592，592X和592F编译环境有区别吗？

A:似乎没有，我对比过在修改芯片型号后官方MRS的项目文件没有一点变化除了一个信息文件，考虑到库也一样可能确实就是没区别吧

如果不放心可以打开模板中的MRS修改芯片型号后再继续回到CLion编程，默认是592F