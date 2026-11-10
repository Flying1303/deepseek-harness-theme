# DeepSeek Harness 官网风格皮肤 v1.0

简体中文 | [English](./README.en.md)

浅色和深色均支持动态流光、星座网格、居中的粒子鲸鱼与磨砂界面。跟随 Harness 的外观设置。插件包无外部依赖，不需要另外下载素材。

v1.0 将画布重建延后到窗口尺寸稳定时，减少拖动窗口时闪烁。

## 来源与致谢

- 原版 Web 皮肤由 B 站 UP 主 [@爱玩蛛的少年](https://space.bilibili.com/564770445) 分享。感谢原作者！[原版演示与下载入口](https://www.bilibili.com/video/BV1fVbi63ETW/)
- 视觉来源为 [DeepSeek Harness 官方产品页](https://www.deepseek.com/harness/)。官方 Web UI 的启动方式见 [DeepSeek Harness 官方仓库](https://github.com/deepseek-ai/deepseek-harness#run)。
- 此仓库提供社区适配版，包含桌面端支持、浅色主题、会话区居中和缩放重绘修复。原皮肤包的清单标注 MIT。

## 官方桌面端

1. 将 [dsh-client-ui-deepseek-bg-1.0.0.tgz](./dsh-client-ui-deepseek-bg-1.0.0.tgz) 下载到本地。无需解压。
2. 打开 DeepSeek Harness，进入左侧「插件 → 添加插件」，粘贴该文件的完整路径，例如 `C:\Users\你的用户名\Downloads\dsh-client-ui-deepseek-bg-1.0.0.tgz`。
3. 安装后点击「立即启用」。如果界面提示重启，完全退出再打开应用。
4. 进入「设置 → 通用设置 → 外观」，选择浅色、深色或跟随系统。

已装过同名皮肤时，先在插件页卸载旧版，再安装新版。恢复原版时，在插件页关闭或卸载 `dsh-client-ui-deepseek-bg`，然后重新打开客户端。

### Windows 桌面端命令行安装

先启动过一次桌面端以初始化配置，随后完全退出桌面端。PowerShell 示例，将两个路径替换为实际路径：

```powershell
& 'H:\Programs\DeepSeek Harness\resources\runtime\cli\bin\dsh.cmd' plugin --profile desktop add 'C:\Users\你的用户名\Downloads\dsh-client-ui-deepseek-bg-1.0.0.tgz'
```

安装完成后重新打开 DeepSeek Harness。命令行用的是桌面安装目录自带的 dsh。

## Harness Web

在有 Web 插件管理器的版本上，可使用相同的本地包路径安装并启用。若 Web Host 部署在另一台机器上，路径必须在 Host 那台机器上可访问。也可在 Host 上使用该 Web 安装的 CLI：

```sh
dsh plugin --profile web add /absolute/path/dsh-client-ui-deepseek-bg-1.0.0.tgz
```

重启 Web Host 并刷新页面。

## 兼容范围

Windows 官方桌面版 0.2.2-rc.1 已用于开发和安装验证。同系列 Web、macOS 或 Linux 客户端需支持 DSH bundle、Web 客户端插件和 WebGL2。其他版本和第三方客户端需实测，布局改动较大的版本可能缺少部分磨砂效果。仅支持 DeepSeek Harness 的插件系统。
