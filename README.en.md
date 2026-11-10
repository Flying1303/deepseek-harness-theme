# DeepSeek Harness Website-Inspired Theme v1.0

[简体中文](./README.md) | English

A community theme for DeepSeek Harness with animated aurora, an interactive constellation grid, a centered particle whale, and frosted glass surfaces. The theme follows Harness's light and dark appearance settings. All assets are bundled.

Version 1.0 keeps the last rendered background frame while the window is being resized and redraws it once the window size settles.

## Credits and upstream

- **Original Web theme** [爱玩蛛的少年](https://space.bilibili.com/564770445) (Bilibili UID 564770445)
- **Desktop and dual-theme adaptation** [Flying1303](https://github.com/Flying1303)

- Thanks to Bilibili creator [@爱玩蛛的少年](https://space.bilibili.com/564770445) for sharing the original Web theme. [Original demo and download links](https://www.bilibili.com/video/BV1fVbi63ETW/)
- The visual design is inspired by the original DeepSeek Harness launch page. See the [current official product page](https://www.deepseek.com/harness/) and the [startup guide](https://github.com/deepseek-ai/deepseek-harness#run) for current information.
- This community adaptation adds desktop support, a light theme, conversation-area centering, and the resize fix. The original theme's package manifest declares MIT.

## Install on DeepSeek Harness Desktop

1. Download [dsh-client-ui-deepseek-bg-1.0.0.tgz](./dsh-client-ui-deepseek-bg-1.0.0.tgz). Keep the archive intact.
2. Open Harness and go to **Plugins → Add plugin**. Paste the absolute path to the downloaded file.
3. Install it and select **Enable now**. If prompted, quit and reopen Harness.
4. Choose **Light**, **Dark**, or **System** under **Settings → General → Appearance**.

If an older copy of this plugin is installed, uninstall it before installing the new one. To restore the default appearance, disable or uninstall `dsh-client-ui-deepseek-bg` and reopen Harness.

### Windows command-line installation

Launch Harness Desktop once to initialize its profile, then quit it completely. Replace both paths in the example with the paths on your computer.

```powershell
& 'C:\Path\To\DeepSeek Harness\resources\runtime\cli\bin\dsh.cmd' plugin --profile desktop add 'C:\Path\To\dsh-client-ui-deepseek-bg-1.0.0.tgz'
```

Reopen DeepSeek Harness after installation.

## Install on Harness Web

Use **Plugins → Add plugin** with the absolute archive path on the machine running the Web host. You can also install it using the host's CLI.

```sh
dsh plugin --profile web add /absolute/path/dsh-client-ui-deepseek-bg-1.0.0.tgz
```

Restart the Web host and refresh the page.

## Compatibility

Offline installation and removal were verified with the official Windows Desktop 0.2.2-rc.1 CLI. Web, macOS, Linux, and third-party clients require DSH bundle support, Web client plugins, and WebGL2. Those environments have yet to be individually tested. Clients with different layouts may render some glass effects differently.
