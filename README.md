<div align="center">

<img src="logo.png" width="120" alt="FileOrganizer Pro">

# FileOrganizer Pro

**苹果风格的 Windows 智能文件整理工具**

一键把杂乱的桌面、下载文件夹整理得井井有条 —— 全程本地处理，不上传任何文件

[![Version](https://img.shields.io/badge/version-1.2.0-0071E3?style=flat-square)](https://github.com/RHH-herry/FileOrganizer-Pro/releases/latest)
[![Channel](https://img.shields.io/badge/channel-stable-34C759?style=flat-square)](VERSION)
[![Platform](https://img.shields.io/badge/platform-Windows%2010%2F11%20x64-5856D6?style=flat-square)](#系统要求)
[![License](https://img.shields.io/badge/license-Proprietary-FF9500?style=flat-square)](LICENSE)
[![Downloads](https://img.shields.io/github/downloads/RHH-herry/FileOrganizer-Pro/total?style=flat-square&color=0071E3)](https://github.com/RHH-herry/FileOrganizer-Pro/releases)

**[⬇️ 立即下载](https://github.com/RHH-herry/FileOrganizer-Pro/releases/latest)** ·
**[🌐 产品官网](https://rhh-herry.github.io/FileOrganizer-Pro/)** ·
**[📋 更新日志](https://rhh-herry.github.io/FileOrganizer-Pro/changelog.html)** ·
**[🔒 隐私政策](https://rhh-herry.github.io/FileOrganizer-Pro/privacy-policy.html)**

<img src="images/banner.png" width="720" alt="FileOrganizer Pro 界面预览">

</div>

---

## 这个仓库是什么

这里是 **FileOrganizer Pro 的官方发布与下载仓库**，提供安装包、版本元数据、校验和、安全说明与产品官网。

> **⚠️ 本软件为闭源商业软件（Proprietary Software），源代码不公开。**
> 本仓库**不包含任何源代码**，请勿提交 Pull Request 修改代码。
> 详见 [开源范围声明](#开源范围声明) 与 [LICENSE](LICENSE)。

## 核心功能

| 功能 | 说明 |
|------|------|
| 🗂 **快速整理** | 按文件类型 / 修改日期 / 名称规则一键归类，支持预览后再执行 |
| ⚙️ **自定义规则引擎** | 自建匹配条件（扩展名、关键词、大小、时间范围）与目标路径，规则可保存复用 |
| ✏️ **批量重命名** | 序号、日期、查找替换、大小写转换、正则模式，实时预览重命名结果 |
| 🔍 **重复文件检测** | 基于内容哈希比对（非仅文件名），精准识别重复并批量清理 |
| 🧹 **智能清理** | 识别临时文件、空文件夹、无效快捷方式等可安全清理项 |
| ↩️ **撤销与历史** | 每次整理生成可回滚记录，误操作可一键还原 |
| 🎨 **6 套主题** | 苹果风液态玻璃界面，系统级真圆角窗口，深浅色自适应 |

<div align="center">
<img src="images/features.png" width="720" alt="功能总览">
</div>

## 安装

### 系统要求

| 项目 | 要求 |
|------|------|
| 操作系统 | Windows 10 (1809+) / Windows 11，**64 位** |
| 运行时 | **无需预装 .NET** —— 自包含发布已内置 .NET 10 运行时 |
| 磁盘空间 | 约 200 MB |
| 权限 | 普通用户权限即可；整理系统目录时需管理员权限 |

### 下载与安装

1. 前往 **[Releases 页面](https://github.com/RHH-herry/FileOrganizer-Pro/releases/latest)** 下载 `FileOrganizer_Pro_v1.2.0_Setup.exe`
2. 运行安装程序，按引导完成安装
3. 首次启动会显示欢迎向导，可选择主题与默认整理规则

> Windows SmartScreen 可能因安装包尚未积累足够下载量而提示"未知发布者"，
> 点击 **更多信息 → 仍要运行** 即可。建议安装前先用下方命令核验哈希。

### 完整性校验（推荐）

下载后请核验 SHA-256，确认文件未被篡改：

```powershell
Get-FileHash .\FileOrganizer_Pro_v1.2.0_Setup.exe -Algorithm SHA256
```

期望值（见 [`checksums.sha256`](checksums.sha256)）：

```
9AAF0E87E5E31CDFDD120568BA5785BF7E0D9628CFA0749CE54444FE7422E320  FileOrganizer_Pro_v1.2.0_Setup.exe
A532DE87B36620457D933B00B4EF3A69C1185E2193481B30E3D5BA0742213D4D  Uninstall.exe
```

哈希不一致 **请勿运行**，并通过 Issues 反馈。

## 隐私与安全

FileOrganizer Pro **100% 本地运行**：

- ✅ 不上传任何文件、路径或目录结构
- ✅ 不收集个人信息，无账号体系、无遥测、无广告 SDK
- ✅ 唯一的网络请求是**用户主动点击「检查更新」**时读取本仓库的 `update.json`
- ✅ 删除操作默认走**系统回收站**，可还原

完整说明见 [SECURITY.md](SECURITY.md) 与 [隐私政策](https://rhh-herry.github.io/FileOrganizer-Pro/privacy-policy.html)。

## 版本信息

| 项目 | 值 |
|------|-----|
| 版本号 | **1.2.0** |
| 发布通道 | `stable`（正式版） |
| 构建号 | `2026.08.08.001` |
| 序列号 | `FOP-1.2.0-20260808-001` |
| 发布日期 | 2026-08-08 |
| 目标框架 | `net10.0-windows`（win-x64，self-contained） |

机器可读元数据见 [`VERSION`](VERSION) 与 [`update.json`](update.json)。

## 开源范围声明

为避免误解，这里明确说明：

- **FileOrganizer Pro 是闭源专有软件**，全部源代码（界面层、视图模型、核心整理引擎、规则引擎、清理判定、批量重命名引擎、安装器）**均不公开**。
- 本公开仓库仅承担 **产品官网 + 分发下载 + 版本元数据 + 安全文档** 的职能。
- 因此，**本仓库无法也无意支持从源码构建**。这不是缺失，是设计。
- 软件本身免费供个人非商业使用，但"免费"不等于"开源"，请遵守 [LICENSE](LICENSE) 的使用限制。

如果你在找开源工具，作者的另外两个项目是完整开源（MIT）的：

- **[archive-toolbox](https://github.com/RHH-herry/archive-toolbox)** —— 本地 ZIP 压缩/解压/校验/分卷工具
- **[efficiency-toolbox](https://github.com/RHH-herry/efficiency-toolbox)** —— 40+ 离线效率小工具集

## 反馈与支持

| 类型 | 渠道 |
|------|------|
| Bug 报告 / 功能建议 | [提交 Issue](https://github.com/RHH-herry/FileOrganizer-Pro/issues/new/choose) |
| 安全漏洞 | 见 [SECURITY.md](SECURITY.md) 的负责任披露流程 |
| 商务与其他 | 3871822145@qq.com |

反馈 Bug 时请附上：软件版本号、Windows 版本、复现步骤、必要截图。

## 许可证

**专有许可（Proprietary）** —— 免费供个人非商业使用，禁止再分发、反向工程与商业用途。
完整条款见 [LICENSE](LICENSE)。

---

<div align="center">

**如果这个工具帮你省下了整理文件的时间，点个 ⭐ Star 支持一下**

Copyright © 2026 FileOrganizer Pro. 保留所有权利。

</div>
