# 栖桌 Qizhuo

简约的 Windows 桌面工作台。这里分别提供 **Native Lite** 和 **完整版** 的 Windows x64 便携包。

## 下载

| 版本 | 下载 | 压缩包大小 |
| --- | --- | --- |
| Native Lite 0.4.14（预览版） | [下载 Lite](https://github.com/lysisiyi/qizhuo-desktop/releases/download/lite-v0.4.14/QizhuoLite-0.4.14-windows-x64.zip) · [版本说明](https://github.com/lysisiyi/qizhuo-desktop/releases/tag/lite-v0.4.14) | 0.75 MiB |
| 完整版 0.27.0 | [下载完整版](https://github.com/lysisiyi/qizhuo-desktop/releases/download/full-v0.27.0/Qizhuo-0.27.0-windows-x64.zip) · [版本说明](https://github.com/lysisiyi/qizhuo-desktop/releases/tag/full-v0.27.0) | 134.92 MiB |

请下载带有 windows-x64.zip 的程序包。GitHub 自动生成的 Source code 压缩包不是可执行软件包。

## Lite 最近更新

Lite 0.4.14 的分屏小箭头会在按钮下方展开玻璃快捷布局，点选即可排列窗口，无需打开分屏工作台；收起后释放临时玻璃面板。另包含窗口列表兼容、零间距排列及显示桌面后软件栏恢复修复。

## 两个版本怎么选

| 功能 | Native Lite | 完整版 |
| --- | --- | --- |
| 常用空间、每日成果、软件栏 | 支持 | 支持 |
| 原生桌面玻璃 | 支持 | 支持，并带降级方案 |
| 排列现有软件窗口 | 支持，含保存方案和自动启动 | 支持 |
| 内置网页分屏 | 不包含 | 支持 |
| 主题包和更多组件 | 基础场景 | 更完整的编辑与组件功能 |

Lite 使用原生 Windows 界面，适合以桌面卡片和软件窗口排列为主的使用方式。完整版使用 Electron，提供内置网页分屏和更多功能。

## 运行

- **Lite**：解压整个文件夹，双击 QizhuoLite.exe，点击“轻量预览：放到桌面”。无需额外安装 Node.js、Electron 或 WebView。
- **完整版**：解压整个文件夹，双击 Qizhuo.exe。保留旁边的 DLL、resources、locales 和许可证文件，不要只复制 exe。
- 从系统托盘或软件菜单退出。切换两版的桌面模式前，请先退出正在运行的版本。
- 程序包不包含用户记录，也不会自动注册开机启动。

数据分别存放在 %APPDATA%\QizhuoLite 和 %APPDATA%\qizhuo-desktop。备份、升级和导入前请保留原数据。

## 验证与限制

发布前已在当前 Windows 电脑测试 Lite 独立 exe 启动，以及完整版启动、网页分屏、原生桌面玻璃和返回窗口。不同 Windows 版本、显卡和多显示器组合仍需分别验证。

Lite 为预览版。玻璃效果依赖系统桌面合成与显卡驱动。窗口方案保存软件路径、标题、布局和明确填写的启动内容，不保存未保存文档或应用内部完整会话。

当前开发机桌面模式的 Lite 实测私有内存约 79 MiB、工作集约 95 MiB；这是一次运行样本，不是固定上限，不含外部软件、系统 DWM 和全部显存。完整版和网页分屏的内存随使用内容变化。

每个 Release 提供 SHA-256 校验文件。第三方许可证随程序包提供；Chromium 完整许可在完整版的 LICENSES.chromium.zip 中。
