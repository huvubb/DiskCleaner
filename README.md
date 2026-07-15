# 🧹 DiskCleaner — C盘垃圾清理工具

> 一键扫描并清除 Windows C 盘中的临时文件、缓存与系统垃圾，释放磁盘空间。

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-Windows%2010%2F11-lightgrey.svg)]()

---

## 📖 简介

**DiskCleaner** 是一款轻量级的 Windows C 盘垃圾清理工具，纯 C++17 编写，静态编译为单文件 exe，无需任何依赖，双击即可运行。

### 清理范围

| 类型 | 路径 | 需管理员 |
|------|------|:---:|
| 用户临时文件 | `%USERPROFILE%\AppData\Local\Temp` | |
| Chrome 缓存 | `Local\Google\Chrome\User Data\Default\Cache` | |
| Chrome Code Cache | `Local\Google\Chrome\User Data\Default\Code Cache` | |
| Edge 缓存 | `Local\Microsoft\Edge\User Data\Default\Cache` | |
| Edge Code Cache | `Local\Microsoft\Edge\User Data\Default\Code Cache` | |
| Firefox 缓存 | `Local\Mozilla\Firefox\Profiles` | |
| 缩略图缓存 | `Local\Microsoft\Windows\Explorer` | |
| Windows 临时文件 | `C:\Windows\Temp` | ✓ |
| 回收站 | `C:\$Recycle.Bin` | ✓ |
| 预读取文件 | `C:\Windows\Prefetch` | ✓ |
| Windows 更新缓存 | `C:\Windows\SoftwareDistribution\Download` | ✓ |
| Windows 错误报告 | `C:\ProgramData\Microsoft\Windows\WER` | ✓ |
| Windows 日志 | `C:\Windows\Logs` | ✓ |

---

## 🔄 使用流程

```
免责声明 → 输入 YES 开始
    ↓
扫描垃圾 → 显示每项大小 + 总计 + 评级
    ↓
报告汇总 → 输入 Y 确认清理 / N 退出
    ↓
执行清理 → 逐项清理 + 汇总报告
```

### 垃圾量评级

| 评级 | 范围 |
|------|------|
| 轻度 | < 500 MB |
| 中等 | 500 MB ~ 2 GB |
| 较多 | 2 GB ~ 5 GB |
| 大量 | 5 GB ~ 10 GB |
| 严重 | > 10 GB |

---

## ⚠️ 免责声明

```
本软件不提供任何形式的明示或暗示担保。
使用即视为您同意自行承担所有风险。
开发者对因使用本软件而导致的任何数据丢失、系统损坏或其他损失概不负责。
```

---

## 🚀 快速开始

1. 从 [Releases](https://github.com/huvubb/DiskCleaner/releases) 下载 `DiskCleaner.exe`
2. 双击运行（普通用户）或 **右键 → 以管理员身份运行**（完整清理）
3. 阅读免责声明，输入 `YES` 开始扫描
4. 查看扫描报告，输入 `Y` 确认清理

---

## 🔧 本地编译

```bash
g++ -std=c++17 -O2 -static -fexec-charset=UTF-8 \
    -o DiskCleaner.exe DiskCleaner.cpp \
    -lshell32 -lole32
```

要求：MinGW-w64 (g++)、Windows SDK

---

## 📁 项目结构

```
DiskCleaner/
├── DiskCleaner.cpp    # 源代码
├── DiskCleaner.exe    # 可执行文件（静态编译）
└── README.md
```

---

## 📝 License

MIT © 2026
