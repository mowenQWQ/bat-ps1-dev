# bat-ps1-dev

**39 章 bat / PowerShell 脚本开发专项经验库——编码陷阱、cmd 语法坑、PS 5.1/7 兼容、跨平台 pwsh、安全工具最佳实践。**

**A 39-chapter batch & PowerShell scripting vault — encoding traps, cmd syntax gotchas, PS 5.1/7 compatibility, cross-platform pwsh, and security-tool best practices.**

[中文](#中文) | [English](#english)

---

## 中文

### 这是什么

从「SilverFox 银狐木马专杀工具」的 .bat 启动器 + .ps1 引擎双层架构开发中总结的脚本专项经验库。适用于：制作 .bat 启动器、.ps1 引擎、跨平台（pwsh）脚本。

与 [win-dev-pitfalls](https://github.com/mowenQWQ/win-dev-pitfalls)（全量主线，另含 Win32 GUI / Flutter 桌面端）同源，本库聚焦 **bat / PowerShell 脚本层**，独立运营。

### 内容结构

| 章节 | 内容 |
|------|------|
| §0 | 持续更新协议 + **按症状快速索引** |
| §1-13 基础篇 | 编码与行尾（GBK/BOM/CRLF）、cmd 批处理陷阱、PowerShell 5.1/7 兼容（最深的坑）、跨平台 pwsh、检测/安全工具最佳实践、Linux 沙箱实测流程、交付检查清单 |
| §14-39 实战篇 | DLL 加载与主动防御 hook 连环案、WindowsApps 别名坑、双重 BOM 静默拒绝、提权参数传递双坑、拦截关机、开机启动管理（§39）等 |

### 推荐阅读路径

- **遇到具体症状** → §0.1 按症状快速索引直接定位
- **新人入门** → 先扫 §1-13 基础，再按需查 §14-39 实战
- **想学排障思维** → §14-19 的「猜错→证伪→真凶」链完整读一遍

### 特色：每条记录都是三段式

`问题 | 现象/报错 | 对策`，注明来源版本（如 "v2.15.15 实战"），并内建**脱敏核查清单**与**修改后自查清单**——这个库本身就是按"活文档"协议运营的，可直接复用该协议管理你自己的经验库。

### 安装

```bash
git clone https://github.com/mowenQWQ/bat-ps1-dev.git
cp bat-ps1-dev/SKILL.md /path/to/your/agent/skills/bat-ps1-dev/
```

适用于支持 Skill 格式的 AI 编码助手（Claude Code / CodeBuddy / OpenClaw 等），按 description 关键词自动触发；也可以直接当文档读。

### 更多技能库

| 仓库 | 简介 |
|------|------|
| [win-dev-pitfalls](https://github.com/mowenQWQ/win-dev-pitfalls) | Windows 开发踩坑全量主线（含 Win32 GUI / Flutter 桌面端） |
| [Web-Security-Test-Rules](https://github.com/mowenQWQ/Web-Security-Test-Rules) | 已授权网站安全测试规则库 |
| [unattended-task-pitfalls](https://github.com/mowenQWQ/unattended-task-pitfalls) | 无人值守自动任务加固经验库 |
| [agent-mistake-patterns](https://github.com/mowenQWQ/agent-mistake-patterns) | AI 智能体犯错模式库与自我纠错纪律 |
| [grounded-summaries-skill](https://github.com/mowenQWQ/grounded-summaries-skill) | 防止 AI 在总结任务中编造内容 |

---

## English

### What is this

A scripting-focused vault distilled from the .bat launcher + .ps1 engine dual-layer architecture of the **SilverFox trojan-detection tool**. For building .bat launchers, .ps1 engines, and cross-platform (pwsh) scripts.

Same origin as [win-dev-pitfalls](https://github.com/mowenQWQ/win-dev-pitfalls) (the full-line vault with Win32 GUI / Flutter desktop extras); this one focuses on the **batch / PowerShell scripting layer** and is maintained independently.

### Structure

| Section | Content |
|---------|---------|
| §0 | Living-document protocol + symptom-based quick index |
| §1-13 Fundamentals | Encoding & line endings (GBK/BOM/CRLF), cmd traps, PowerShell 5.1/7 compatibility, cross-platform pwsh, security-tool best practices, Linux sandbox testing, delivery checklists |
| §14-39 Battle-tested | DLL loading & AV-hook chains, WindowsApps alias traps, double-BOM silent rejection, elevation argument pitfalls, shutdown interception, Run-key autostart management (§39) |

### Signature format

Every record follows `problem | symptom/error | fix`, annotated with the originating version, plus built-in **sanitization checklists** and **post-edit self-review checklists** — the vault is run as a living document, and the protocol itself is reusable for your own knowledge base.

### Installation

```bash
git clone https://github.com/mowenQWQ/bat-ps1-dev.git
cp bat-ps1-dev/SKILL.md /path/to/your/agent/skills/bat-ps1-dev/
```

---

## License

MIT

---

## 🤖 AI 使用声明 / AI Usage Disclosure

本项目在开发与维护过程中使用了 AI 编程助手（Claude / Anthropic）辅助代码编写、文档整理与问题排查；核心决策、内容审核与最终发布由维护者完成。

This project was developed and maintained with the assistance of an AI coding assistant (Claude / Anthropic) for coding, documentation, and troubleshooting. Core decisions, content review, and final releases are made by the maintainer.
