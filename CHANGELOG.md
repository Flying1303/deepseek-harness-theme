# 更新日志 / Changelog

## v1.0.1 · 2026-11-10

- 修复已发送消息气泡四周露出方角的问题。磨砂样式现在直接作用在消息气泡上，沿用 Harness 自带的圆角。
- Fixed square corners showing around sent messages. The frosted styling now applies to the message bubble itself and follows Harness's native corner radius.

- DSH 插件管理中的显示名称统一为 `deepseek-harness-theme`，与 GitHub 仓库名一致。
- The plugin now displays as `deepseek-harness-theme` in the DSH plugin manager, matching the GitHub repository name.
- Windows 一键安装工具现提供独立的简体中文和英文 ZIP。英文版包含英文安装提示、错误信息和使用说明，两版内置同一个插件。
- The Windows one-click installer is now available in separate Simplified Chinese and English ZIPs. The English edition includes localized prompts, errors, and instructions. Both editions bundle the same plugin.


## v1.0 · 2026-11-09

- 首次公开发布。包含桌面端适配、浅色与深色主题、粒子鲸鱼居中，以及窗口缩放优化。拖动窗口时保留上一帧，待尺寸稳定后再重建背景画布，以减少闪烁。
- Initial public release with desktop adaptation, light and dark themes, a centered particle whale, and smoother resizing. The background keeps its last rendered frame during resizing and rebuilds the canvas once the window size settles to reduce flicker.
