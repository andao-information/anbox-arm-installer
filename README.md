# anbox-arm-installer
[Anbox](https://www.anbox.io/) 基于容器，可以在 Linux 上运行 Android 应用。为在 x86 设备上运行针对 arm 指令集构建的应用，需要安装指令翻译层 [libhoudini](https://github.com/Rprop/libhoudini/) 。

关于脚本的详细说明参见
~~https://geeks-r-us.de/2017/08/26/android-apps-auf-dem-linux-desktop/~~
https://geeks-r-us.de/2018/09/04/anbox-update-overlay/ (德语)

此脚本去除了安装 Google Play 的内容，其他部分未作改动。使用 Anbox 170 测试正常工作。

## 用法

安装 Anbox

```
sudo add-apt-repository ppa:morphis/anbox-support
sudo apt update
sudo apt install anbox-modules-dkms
sudo modprobe ashmem_linux
sudo modprobe binder_linux
sudo snap install --edge --devmode anbox
```

启动 anbox ，确认可以正常运行。关闭 Anbox 后运行此脚本

```sudo arm-installer.sh```

## 捐赠

可通过以下方式支持原脚本作者

If you find this piece of software useful and or want to support it's development think of buying me a coffee https://www.buymeacoffee.com/YdV7B1rex
