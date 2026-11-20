# Codex 额度监控

在桌面或任务栏查看 Codex 的 5 小时与周额度、重置时间及重置卡。

**当前版本：0.28 · Windows x64 · 公开测试版 · 第三方桌面工具**

[下载便携版](https://github.com/Xucool/codex-quota-float-custom/releases/download/v0.28/CodexQuotaMonitor-0.28-Windows-x64-Portable.zip) · [下载安装版](https://github.com/Xucool/codex-quota-float-custom/releases/download/v0.28/CodexQuotaMonitor-0.28-Windows-x64-Setup.exe) · [SHA-256 校验](https://github.com/Xucool/codex-quota-float-custom/releases/download/v0.28/SHA256SUMS.txt) · [发布说明](docs/发布说明.md)

## 当前功能
- 两种显示模式：百分比悬停、任务栏固定显示。已移除简约卡片，旧配置自动迁移。
- 任务栏固定白字、10 号常规字体，背景近透明；整个文字区域可触发鼠标悬停。
- 打开弹窗由鼠标事件触发；每 100 毫秒的位置检查仅辅助判断收起。
- 显示 5 小时与周额度、重置时间、重置卡；保留宠物显示开关。
- 可启用跟随 Codex 桌面程序启停：最小化继续运行，完全退出 Codex 后约 6 秒关闭监控。
- 跟随助手需要轻量常驻。主程序在 Codex 未打开时不运行。

## 开始使用
便携版：完整解压，双击 **额度监控.exe**。
安装版：运行 Setup，为当前 Windows 用户安装，无需管理员权限。默认不自动启动，也不默认开启开机启动。
需要联动时，运行 **跟随Codex启动.exe**；安装版也可从开始菜单选择“跟随 Codex 启停”。在偏好设置中可以关闭联动。
两个入口属于同一软件，图标相同，不能只复制单个 EXE。升级前先退出旧版本。
安装包和便携包内容相同。GitHub 自动生成的 Source code ZIP 只包含公开文档，不能作为运行包。

需要官方 Codex、自己的 ChatGPT 登录状态和 .NET Framework 4.6.1+。仅 API Key 登录可能没有套餐额度。
详细使用方法见 [使用说明](docs/使用说明.md)。

## 验证范围
透明白字的早期修复已由维护者在本机确认。当前字号、悬停和窗口层级补丁已通过相关自检，但未完成整套桌面交互实测。
跟随启动已通过六种状态逻辑检查并能识别当前 Codex 桌面进程，尚未通过完整的关闭、重开及 Windows 重启验证。
本次安装包未执行安装和卸载实测。Windows 11、ARM、第二台机器和不同任务栏美化环境未验证。
程序未签名，不需要关闭系统安全功能。版本限制和验证详情见 [发布说明](docs/发布说明.md)。

## 隐私
使用本机官方 Codex 的登录状态读取额度，不要求在软件中输入密码或复制 Token。重置卡的“使用”操作会发出真实请求，可能消耗卡片。
发布包不包含维护者的账号凭据、个人配置或账户日志。不要在反馈中上传此类信息。

## 来源、授权与反馈
基于 [Leon-z7/codex-quota-float](https://github.com/Leon-z7/codex-quota-float)，维护账号 [Xucool](https://github.com/Xucool)。
维护者此前已确认获得修改与再分发授权。本仓库继续只公开文档、演示图片及编译成品，不公开改版源码；原项目和第三方依赖许可仍适用。
Electron 与 Chromium 的许可随运行包保留。本软件不是 OpenAI 官方产品。
[反馈问题](https://github.com/Xucool/codex-quota-float-custom/issues)时请提供 Windows 版本、软件版本和错误提示。
