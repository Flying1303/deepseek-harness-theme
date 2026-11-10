# 更新日志 / Changelog

发布日期时区为 **(UTC+08:00) 北京，重庆，香港特别行政区，乌鲁木齐**。

Release dates use **(UTC+08:00) Beijing, Chongqing, Hong Kong SAR, Urumqi**.

## v1.0.1 · 2026-11-10

- 修复已发送消息气泡四周露出方角的问题。磨砂样式现在直接作用在消息气泡上，沿用 Harness 自带的圆角。
- Fixed square corners showing around sent messages. The frosted styling now applies to the message bubble itself and follows Harness's native corner radius.

- DSH 插件的显示名称和包标识统一为 `deepseek-harness-theme`，与 GitHub 仓库名一致。一键安装会迁移旧标识 `dsh-client-ui-deepseek-bg`。
- The display name and package identifier now both match the GitHub repository name, `deepseek-harness-theme`. The one-click installer migrates installations using the old identifier.
- Windows 一键安装工具现提供独立的简体中文（-CN）和英文（-EN）ZIP。英文版包含英文安装提示、错误信息和使用说明，两版内置同一个插件。
- The Windows one-click installer is now available in separate Simplified Chinese (-CN) and English (-EN) ZIPs. The English edition includes localized prompts, errors, and instructions. Both editions bundle the same plugin.


## v1.0 · 2026-11-10

- 首次公开发布。包含桌面端适配、浅色与深色主题、粒子鲸鱼居中，以及窗口缩放优化。拖动窗口时保留上一帧，待尺寸稳定后再重建背景画布，以减少闪烁。
- Initial public release with desktop adaptation, light and dark themes, a centered particle whale, and smoother resizing. The background keeps its last rendered frame during resizing and rebuilds the canvas once the window size settles to reduce flicker.
