# TB321FU_PixelOS_16_Komodo修改来自[Mystic-GSI](https://sourceforge.net/projects/mystic-gsi-updates/),原机型为Pixel 9 Pro XL(代号Komodo)

Bug: 

1. 自动亮度(依旧懒得修,反正这个机器自动亮度也很难用)
2. 系统自带的人脸识别可以添加,无法使用(毕竟依赖Tensor处理器,用不了一点)

我修改了什么:

1. 已签名；可直接启动，无需关闭 vbmeta 验证
2. 原GSI开机后为Selinux宽容,我修复了这点,现在开机10s后自动设置为Selinux严格
3. 修复`build.prop`,可被直接识别为正确的机型,默认关闭ADB等调试用的功能
4. 精简了一部分不常用的预装Google软件

ROM特性:

1. 环境几乎就是PixelOS原系统,几乎接近原厂系统,不存在权限漏洞
2. 配合Magisk模块,可以通过Play认证!
3. 配合Magisk模块,可以通过市面上几乎所有的Root检测器!
4. 接近Pixel原机体验的震动!
5. 接近Pixel原机体验的软件系统,非常流畅!
6. 全局165HZ
7. 安卓16最新特性,包括9:1分屏,新的UI,圈定即搜等.
8. 可以直接搜到6Ghz Wifi
9. 可以开无线热点(为什么官方系统阉割了这个功能?不理解) 

工作的硬件:

1. 几乎所有! 除了自动亮度,包括:
2. **CPU / GPU**
3. **蓝牙 / Wi-Fi**
4. **高刷新率**（165Hz 自适应）
5. **扬声器**
6. **前后相机**
7. **自动旋转**
8. **X 轴线性马达**
9. **USB-C 接口**（两个接口均可全速正常工作）

如何刷入:

1. 刷入最新的官方系统
2. 重启到fastbootd
3. 像一个正常GSI一样刷入
4. 刷入KernelSU(可选)
5. 享受它!

```
fastboot flash system "Pixel-komodo-16_ext4_raw_Signed_V5.img"
```


