# 安装 RT Console

RT Console 使用同一安装身份覆盖升级，Ubuntu 菜单只保留一个 **RT Console**。数据回放采用新版头环俯视图，从右起相机 0、1、2、5、4、3，点击热点切换单路；历史文件沿用自己的布局快照。相机 / IMU 编号及平台边界见 [回放指南](playback.md)。`.21` 的 Ubuntu / Windows / Android 安装包及校验文件已发布。

从 [Releases](https://github.com/RankTogether/RT-Console/releases) 下载对应平台的软件和校验文件。公开附件无需登录。

- Ubuntu：`sudo apt install --allow-downgrades ./rt-console_0.0.1.21_amd64.deb`，退出旧程序后从应用菜单打开 **RT Console**，或运行 `rtcamera-finder`。卸载：`sudo apt remove rtcamera-finder`。
- Windows：运行 `rt-console_0.0.1.21_windows-x64-setup.exe`，按当前用户安装，无需管理员权限；也可完整解压 Windows 便携 ZIP，运行其中的 `rtcamera_finder.exe`。卸载使用系统“已安装的应用”。
- Android：安装 `rt-console_0.0.1.21_android-arm64-internal-debug.apk`，Android 7.0+ arm64；这是内部测试签名，云机证书可能与本地候选不同，覆盖失败时先卸载原候选。
- Ubuntu 便携版：完整解压 `linux-x64.tar.gz`，运行包内 `rtcamera_finder`。保留同目录 `lib/`、`data/`；系统仍需 GTK、Avahi、iproute2、xdg-utils。

从旧 0.4.12 切换到 `0.0.1.x` 属于编号重编，Ubuntu 安装命令显式允许降级；Android 内部升级编号持续递增。

安装依赖可能需要互联网，程序运行和局域网搜索无需互联网。Windows 内部测试包暂未代码签名，系统可能提示发布者未知；只使用本仓发布的包并核对 SHA256。安装器不自动修改防火墙规则。


请同时下载对应平台 SHA256SUMS 文件核对安装包。Windows 可用 `Get-FileHash 文件名 -Algorithm SHA256`，Linux 可用 `sha256sum -c 校验文件名`。
