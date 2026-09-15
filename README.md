# Antify Feedback

[English](README_EN.md)

[官方网站](https://antifyapp.com/zh) · [下载 Antify](https://r2.antifyapp.com/releases/latest/Antify.dmg) · [使用指南](https://antifyapp.com/zh/guides) · [更新记录](https://antifyapp.com/zh/changelog) · [隐私说明](https://antifyapp.com/zh/privacy)

Antify 是一款 macOS 应用级透明代理工具。它通过系统扩展处理你指定 App 的网络连接，无需开启 macOS 系统代理，也无需在代理工具中启用 TUN 模式。

这个仓库是 Antify 的公开反馈入口，用于报告问题、提出功能建议和讨论使用体验。仓库中不包含 Antify 的应用源码。

<img src="assets/antify-rules.png" alt="Antify 应用规则界面" width="1200" />

## Antify 能做什么

- 为不同 App 分别设置 `Proxy`、`Direct` 或 `Block`。
- 配置 SOCKS5、HTTP 和 HTTPS 代理，并在使用前测试连接延迟。
- 用多个 `Configuration` 保存不同的规则组合，并按 Wi-Fi 名称自动切换。
- 通过 `Connections`、`Activity` 和 `Discovery` 查看连接与规则匹配情况。
- 为命令行工具、脚本和可执行文件创建路径规则。

代理服务器需要由你自行准备，Antify 不提供代理服务。

## 系统要求

- macOS 14.0 或更高版本。
- 首次使用时需要安装并授权 Antify 系统扩展。
- 至少准备一个可用的 SOCKS5、HTTP 或 HTTPS 代理服务器。

## 下载与上手

你可以直接[下载最新版本](https://r2.antifyapp.com/releases/latest/Antify.dmg)，也可以通过 Homebrew 安装。

```bash
brew tap cyberlesterr/antify
brew install --cask antify
```

第一次使用可以从[安装系统扩展](https://antifyapp.com/zh/guides/first-installation)开始，再按[完整使用指南](https://antifyapp.com/zh/guides)添加代理和应用规则。

## 遇到问题先看这里

| 你遇到的情况 | 指南 |
|---|---|
| 扩展装不上，或卡在授权 | [安装 Antify 与系统扩展](https://antifyapp.com/zh/guides/first-installation) |
| 代理填好了但连不上 | [添加并测试代理服务器](https://antifyapp.com/zh/guides/configure-proxy) |
| 想让某个 App 走代理、直连或断网 | [为不同 App 设置代理、直连或阻止](https://antifyapp.com/zh/guides/per-app-routing) |
| 终端或 IDE 启动的命令不走代理 | [让终端和 IDE 启动的命令走指定代理](https://antifyapp.com/zh/guides/dev-tools-proxy) |
| 要给命令行工具、脚本加规则 | [为 CLI、脚本和包创建路径规则](https://antifyapp.com/zh/guides/command-line-rules) |
| 不确定规则有没有生效 | [理解「连接」、「探索」和「活动」](https://antifyapp.com/zh/guides/connections-and-activity) |

## 提交反馈

提交前请先搜索[已有 Issues](../../issues)，看看是否已经有人报告过同一问题。

- [报告 Bug](../../issues/new?template=bug_report.md)
- [提出功能建议](../../issues/new?template=feature_request.md)

一份容易定位的 Bug 报告通常包括以下信息。

- Antify 版本和 macOS 版本
- 代理类型，以及是否启用了认证
- 可以重复出现问题的操作步骤
- 预期结果和实际结果
- 相关截图或日志

提出功能建议时，请说明你遇到的实际问题、希望 Antify 怎样工作，以及目前使用的替代方案。

你可以在 `Settings > General > Diagnostics > Collect Logs…` 中采集诊断信息。GitHub Issues 是公开页面，上传前请检查截图和日志，移除代理密码、令牌及其他不希望公开的信息。

## 中文交流群

欢迎加入交流群，与其他用户讨论使用方法和分享反馈。二维码失效时，可以通过 GitHub Issues 联系我们。

<table>
  <tr>
    <td><img width="280" height="500" alt="Antify 中文交流群二维码" src="https://github.com/user-attachments/assets/dee70719-5edf-4626-97e9-e846125b073e" /></td>
  </tr>
</table>
