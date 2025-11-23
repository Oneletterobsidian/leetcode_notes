# one# LeetCode Daily Submit Auto Push · LeetCode 每日提交自动推送 GitHub

> 自动化管理 LeetCode 题解（solutions），每天将本地更新的代码自动提交（commit）并推送（push）到 GitHub 仓库（repository）。

---

## 1. Project Overview · 项目概述

**English**

This repository is used to **organize my LeetCode solutions** and **automatically push** daily updates to GitHub.  
A small script plus a scheduler (cron / Windows Task Scheduler / GitHub Actions) will:

1. Detect changed solution files  
2. Create a git commit with a standard message  
3. Push the commit to the remote repository

**中文**

本仓库用于 **整理我的 LeetCode 题解**，并通过一个小脚本 + 定时任务（scheduler）实现：

1. 检测当天新增或修改的题解文件  
2. 自动生成标准的 Git 提交信息（commit message）  
3. 自动推送（push）到远程 GitHub 仓库  

---

## 2. Directory Structure · 目录结构

```text
.
├─ scripts/                    # 自动化脚本 scripts
│   ├─ auto_commit.py          # 自动提交脚本（Python 示例，可自定义）
│   └─ config.example.json     # 配置模板 config template
├─ solutions/                  # 题解代码 solutions
│   ├─ python/
│   │   ├─ 0001_two_sum.py
│   │   ├─ 0021_merge_two_sorted_lists.py
│   │   └─ ...
│   └─ cpp/
│       ├─ 0001_two_sum.cpp
│       └─ ...
└─ README.md
