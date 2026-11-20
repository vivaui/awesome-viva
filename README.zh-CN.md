# Awesome Viva

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> 一份关于 [Viva](https://github.com/vivaui/viva) 的精选列表：应用、工具与资源。Viva 是一个 Go 优先、GPU 原生的桌面框架。

Viva 在 macOS、Windows 和 Linux 上直接绘制原生窗口与 GPU 表面，不使用
WebView，不捆绑浏览器引擎，也没有附加运行时。应用用 Go 编写，组件以源码分发，
发布产物只包含它实际用到的代码。

[English](README.md) | 简体中文

## 目录

- [应用](#应用)
- [官方资源](#官方资源)
- [框架包](#框架包)
- [工具](#工具)
- [学习](#学习)
- [社区](#社区)
- [贡献](#贡献)
- [许可证](#许可证)

## 应用

用 Viva 构建、源码公开的应用。

- [Motty](https://github.com/t8y2/motty) - 把终端、SFTP、端口转发、远程桌面和 AI 助手放进同一个原生窗口的 SSH 工作台。`macOS` `Windows` `Linux` · Apache-2.0
- [Peck](https://github.com/eryajf/Peck) - macOS 菜单栏助手：检查隔离标记与签名状态，等你确认后再打开被系统拦下的应用。`macOS` · Apache-2.0
- [听澜（Tinglan）](https://github.com/talongao/tinglan) - 非官方、实验性的华为音乐客户端，带原生音乐库、歌词、12 款主题和可悬浮的播放器。`macOS` · AGPL-3.0
- [Viff](https://github.com/1lck/viff) - 轻量的原生 Git 客户端，支持按行暂存、并排 diff 和分页历史。`macOS` `Windows` · MIT
- [GoIM](https://github.com/Ezreal-byte/GoIM) - 支持自动发现同一局域网内的设备，可单聊、群聊和共享文件。`macOS` `Windows` `Linux` · MIT

## 官方资源

- [Viva](https://github.com/vivaui/viva) - 框架与运行时：面向 macOS、Windows 和 Linux 的 Go 模块。
- [官网](https://vivaui.dev/zh/) - 指南、API 参考和带实时预览的组件目录，也有[英文版](https://vivaui.dev/en/)。
- [文档](https://vivaui.dev/zh/docs/) - 从第一个窗口到打包发布的全部指南。
- [API 参考](https://vivaui.dev/zh/api/) - 按包组织的公开 Go API。
- [组件目录](https://vivaui.dev/zh/components/) - 以源码分发的组件配方，附实时预览。
- [案例](https://vivaui.dev/zh/showcase/) - 用 Viva 构建的应用，含截图与链接。
- [版本发布](https://github.com/vivaui/viva/releases) - 发布说明、源码标签和预编译的 `viva` 命令压缩包。

## 框架包

- [app](https://pkg.go.dev/github.com/vivaui/viva/app) - 窗口生命周期、状态栏项、密钥存储、拖放和平台服务。
- [ui](https://pkg.go.dev/github.com/vivaui/viva/ui) - 保留式场景、绘制原语、输入、焦点与无障碍。
- [flex](https://pkg.go.dev/github.com/vivaui/viva/flex) - 用 Go 声明、按 CSS flexbox 规则排版的布局。
- [components](https://pkg.go.dev/github.com/vivaui/viva/components) - 参考 shadcn 的组件配方，一个组件一个普通 Go 文件。
- [text](https://pkg.go.dev/github.com/vivaui/viva/text) - 文本整形与编辑契约。
- [markdown](https://pkg.go.dev/github.com/vivaui/viva/markdown) - 原生渲染助手回复和发布说明所用的 Markdown。
- [headless](https://pkg.go.dev/github.com/vivaui/viva/headless) - 不打开窗口，运行应用真实的绘制、输入与焦点路径。

## 工具

- [viva 命令](https://github.com/vivaui/viva/tree/main/cmd/viva) - 构建、打包、初始化项目和热重载应用；这些代码都不会链接进发布产物。
- [Homebrew tap](https://github.com/vivaui/homebrew-tap) - 在 macOS 和 Linux 上 `brew install vivaui/tap/viva`。
- [Scoop 清单](https://github.com/vivaui/homebrew-tap) - 同一个仓库也放 Windows 清单：`scoop bucket add vivaui ...`。
- [无头测试](https://vivaui.dev/zh/docs/testing/) - `vivahead` 构建标签，以及从不打开窗口的测试驱动。
- [编码助手技能](https://github.com/vivaui/viva/tree/main/docs/skills/building-with-viva) - 一份教会 Agent 编程模型与无头工作流的技能文件。

## 学习

- [快速开始](https://vivaui.dev/zh/docs/getting-started/) - 安装命令、初始化项目、打开窗口。
- [编程模型](https://vivaui.dev/zh/docs/programming-model/) - 状态、失效与重绘。
- [声明式布局](https://vivaui.dev/zh/docs/declarative-layout/) - 用值而不是坐标搭建页面。
- [绘制与布局](https://vivaui.dev/zh/docs/drawing-and-layout/) - 绘制路径，以及布局在其中的位置。
- [输入处理](https://vivaui.dev/zh/docs/handling-input/) - 指针、键盘与焦点。
- [文本输入](https://vivaui.dev/zh/docs/text-input/) - 原生编辑、选择与输入法。
- [主题](https://vivaui.dev/zh/docs/theming/) - 颜色、字体与密度。
- [构建与打包](https://vivaui.dev/zh/docs/build-and-package/) - 从 `viva build` 到签名后的应用包。
- [测试](https://vivaui.dev/zh/docs/testing/) - 在 `go test` 里无头驱动 UI。
- [性能](https://vivaui.dev/zh/docs/performance/) - 预算指标以及它们的测量方式。
- [平台](https://vivaui.dev/zh/docs/platforms/) - 各个后端目前支持的能力。
- [系统集成](https://vivaui.dev/zh/docs/system-integration/) - 状态栏项、密钥、文件拖放与文件管理器。

## 社区

- [Discussions](https://github.com/vivaui/viva/discussions) - 提问、想法和作品分享。
- [Issues](https://github.com/vivaui/viva/issues) - Bug 报告与功能请求。
- [贡献指南](https://github.com/vivaui/viva/blob/main/CONTRIBUTING.md) - 框架改动如何评审。
- [行为准则](https://github.com/vivaui/viva/blob/main/CODE_OF_CONDUCT.md)

## 贡献

发现缺项？欢迎补充。

这份列表遵循 [Awesome](https://awesome.re) 的惯例。要添加一个应用，请在同一次
pull request 里同时修改 `README.md` 与 `README.zh-CN.md`，并满足：

- 应用用自己的 UI 使用 Viva，而不是只把网页包在一个窗口里；
- 每个项目只占一条，保持现有顺序；
- 提供公开源码仓库、构建或安装说明、明确的许可证，以及仍在维护的迹象；
- 用一句话说明应用做什么、给谁用。

完整检查清单见 [CONTRIBUTING.md](CONTRIBUTING.md)。

## 许可证

[![CC0](https://licensebuttons.net/p/zero/1.0/80x15.png)](https://creativecommons.org/publicdomain/zero/1.0/)

列表本身以 CC0 1.0 发布。应用名称、代码与图像归各自项目所有。
