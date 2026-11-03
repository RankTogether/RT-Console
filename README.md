# RT Console

设备管理与 MCAP 视频 / IMU 数据回放工具，支持 Ubuntu、Windows 和 Android。

本仓库提供公开说明与软件下载。当前版本为 **0.0.1.21 预发行**。

| 平台 | 下载 |
| --- | --- |
| Windows 10 / 11 x64 | [安装版](https://github.com/RankTogether/RT-Console/releases/download/v0.0.1.21/rt-console_0.0.1.21_windows-x64-setup.exe) · [便携版](https://github.com/RankTogether/RT-Console/releases/download/v0.0.1.21/rt-console_0.0.1.21_windows-x64-portable.zip) |
| Ubuntu 22.04+ x64 | [deb 安装包](https://github.com/RankTogether/RT-Console/releases/download/v0.0.1.21/rt-console_0.0.1.21_amd64.deb) · [便携版](https://github.com/RankTogether/RT-Console/releases/download/v0.0.1.21/rt-console_0.0.1.21_linux-x64.tar.gz) |
| Android 7.0+ arm64 | [内部测试 APK](https://github.com/RankTogether/RT-Console/releases/download/v0.0.1.21/rt-console_0.0.1.21_android-arm64-internal-debug.apk) |

[全部版本与 SHA256 校验文件](https://github.com/RankTogether/RT-Console/releases) · [安装说明](docs/installation.md) · [设备连接](docs/devices.md) · [数据回放](docs/playback.md) · [第三方声明](THIRD_PARTY_NOTICES.md)

- 在局域网中发现 RTCamera Hub、打开预览网页、配置 Wi-Fi，并独立定位设备。
- 在同一窗口中打开 MCAP，查看视频、IMU 曲线和纳秒时间；按录像内的布局选择相机。
- `.21` 修复 Windows 文件打开进度停在 100% 的问题。Windows 安装版和便携版通过有效文件、损坏文件及超过 4 GiB 偏移的稀疏文件界面检查，均正常退出。

Windows 安装包尚未代码签名；Android 为 internal-debug 签名。真实 Windows LAN / BLE、现场原大文件的性能与内存、物理 Android 手机回放仍待验证；macOS 暂缓。稀疏文件检查不代表现场原长录像的性能验收。

## 版本来源

[0.0.1.21 更新说明](releases/0.0.1.21.md) · [0.0.1.20 更新说明](releases/0.0.1.20.md)

公开标签固定本仓发布文档，GitHub 自动提供的 Source code ZIP / tar.gz 也仅含这些文档。应用构建来源由每版 `releases/*-source.json` 和原始发行附件中的 `source_revision` 追溯。应用源码及构建记录由团队在私有仓维护。

`.20` / `.21` 从原发布入口迁入，安装包及全部 15 个附件逐字节保留；安装身份与软件版本保持原样。
