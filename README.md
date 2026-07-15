# 🧹 DiskCleaner — C盘垃圾清理工具 | C Drive Junk Cleaner

> 一键扫描并清除 Windows C 盘中的临时文件、缓存与系统垃圾，释放磁盘空间。
> One-click scan and clean junk files from Windows C drive.

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-Windows%2010%2F11-lightgrey.svg)]()

---

## 📖 简介 | About

**DiskCleaner** 是一款轻量级的 Windows C 盘垃圾清理工具，纯 C++17 编写，静态编译为单文件 exe，无需任何依赖。

A lightweight Windows C drive junk cleaner written in pure C++17, statically compiled as a single-file exe with zero dependencies.

---

## 🌍 支持的语言 | Supported Languages (50)

启动时输入语言代码即可切换 | Enter language code at startup to switch:

| 代码 | 语言 |
|------|------|
| en | English |
| zh | 简体中文 |
| zh-TW | 繁體中文 |
| ja | 日本語 |
| ko | 한국어 |
| vi | Tiếng Việt |
| th | ไทย |
| hi | हिन्दी |
| bn | বাংলা |
| id | Bahasa Indonesia |
| ms | Bahasa Melayu |
| tl | Filipino |
| ur | اردو |
| ta | தமிழ் |
| te | తెలుగు |
| mr | मराठी |
| gu | ગુજરાતી |
| kn | ಕನ್ನಡ |
| pa | ਪੰਜਾਬੀ |
| es | Español |
| fr | Français |
| de | Deutsch |
| it | Italiano |
| pt | Português |
| ru | Русский |
| pl | Polski |
| nl | Nederlands |
| sv | Svenska |
| no | Norsk |
| da | Dansk |
| fi | Suomi |
| el | Ελληνικά |
| cs | Čeština |
| hu | Magyar |
| ro | Română |
| uk | Українська |
| tr | Türkçe |
| ca | Català |
| ar | العربية |
| he | עברית |
| fa | فارسی |
| sw | Kiswahili |
| eo | Esperanto |
| lt | Lietuvių |
| lv | Latviešu |
| sk | Slovenčina |
| sl | Slovenščina |
| bg | Български |
| sr | Српски |
| hr | Hrvatski |
| et | Eesti |

---

## 🤝 欢迎贡献翻译 | Contribute Translations

欢迎提交 PR 改进翻译或增加新语言！

We welcome PRs to improve translations or add new languages!

| 联系方式 | Contact |
|----------|---------|
| 微信 WeChat | **forever870422** |
| 邮箱 Email | **810372789@qq.com** |

---

## ⚠️ 免责声明 | Disclaimer

本工具免费提供，仅供个人清理 Windows 系统垃圾文件使用。
使用前请关闭重要程序并备份数据。
使用即视为同意：开发者对任何直接或间接损失不承担责任。

This tool is free for personal Windows cleanup use.
Close important programs and back up data before use.
By using this tool you agree: the developer is not liable for any damages.

---

## 🚀 快速开始 | Quick Start

1. 从 [Releases](https://github.com/huvubb/DiskCleaner/releases) 下载 `DiskCleaner.exe`
2. 双击运行 / **右键 → 以管理员身份运行**（完整清理）
3. 输入语言代码（如 zh、en、ja）
4. 阅读免责声明，输入 `YES` 开始扫描
5. 查看扫描报告，选择 [A]全部 / [S]选择 / [N]退出

---

## 🔧 本地编译 | Build

```bash
g++ -std=c++17 -O2 -static -fexec-charset=UTF-8 \
    -o DiskCleaner.exe DiskCleaner.cpp \
    -lshell32 -lole32
```

---

## 📝 License

MIT © 2026
