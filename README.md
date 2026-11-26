# AI Excel 助手 (AI Excel Assistant) · 零公式智能表格清洗与工作流工具

<p align="center">
  <a href="https://gurskyaskamug7878-commits.github.io/excel-ai-assistant/"><strong>🌐 立即打开在线体验 (Live Demo)</strong></a> ·
  <a href="https://github.com/gurskyaskamug7878-commits/excel-ai-assistant/issues/new?template=feature-or-rule.yml"><strong>➕ 提交新清洗规则</strong></a> ·
  <a href="https://github.com/gurskyaskamug7878-commits/excel-ai-assistant/discussions"><strong>💬 加入用户讨论区</strong></a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/License-MIT-blue.svg" alt="License" />
  <img src="https://img.shields.io/badge/Privacy-100%25%20Local%20Browser-emerald.svg" alt="Privacy" />
  <img src="https://img.shields.io/badge/Engine-SheetJS%20%2B%20Safe%20Schema-indigo.svg" alt="Engine" />
  <img src="https://img.shields.io/github/stars/gurskyaskamug7878-commits/excel-ai-assistant?style=social" alt="GitHub Stars" />
</p>

---

## 🇨🇳 中文介绍

### 为什么做「AI Excel 助手」？
行政、HR、财务、运营与电商从业者每天都在被脏数据折磨：身份证号打开变成 `1.38E+10`、多表列名顺序不一致无法合并、VLOOKUP 总是报错、同名记录想保留销售额最大的一条……
**AI Excel 助手** 让不会复杂函数公式的普通职场人，通过**浏览器本地沙盒计算**与**受控 AI 安全工作流**，30 秒搞定高频数据处理：

* **🔒 100% 浏览器本地沙盒计算（隐私零泄露）**：所有 `.xlsx` / `.xls` / `.csv` 解析与清洗均在本地浏览器内存完成，业务明细绝不上传至任何第三方服务器。
* **🛡️ 长数字高保真锁定（杜绝科学计数法）**：读写全链路强制纯文本格式（`t: 's', z: '@'`），彻底解决 18 位身份证、11 位手机号导出后变成 `1.38E+10` 或尾数变 `000` 的痛点。
* **🩺 10 维度全表数据体检中心**：自动排查完全空行、全空列、重复记录、异常手机号、源头已损毁身份证警示、隐藏空格、日期格式混乱，支持**一键生成修复副本（绝不污染原表）**。
* **🤖 受控 AI 工作流（大白话 → JSON Schema → 用户确认 → 白名单执行）**：AI 绝不生成不可控的任意代码，仅映射为 7 个白名单原子算子，参数核对确认后执行。
* **✨ 7 大核心原子算子 + 历史撤销栈**：
  1. **进阶表格去重**：单列/多列联合去重，支持按数值列最大值/最小值保留。
  2. **多表纵向智能合并**：异序表头自动取并集对齐，附带「来源文件」列。
  3. **空行/空列一键清理**。
  4. **格式清洗与身份证提取**：清理首尾及中文内部多余空格、统一 `YYYY-MM-DD` 日期、自动提取 18 位身份证的**出生日期与性别**。
  5. **名称清洗（模糊去重）**：全角转半角、大小写差异智能提醒。
  6. **跨表匹配（VLOOKUP 平替）**：一键将 B 表迟到次数/绩效按姓名或工号匹配到 A 表。
  7. **分类汇总与可视化占比看板** + **10 步快照撤销/重做 (Undo/Redo)**。

### 🤝 如何参与贡献与反馈？
* **需要新的表格清洗规则或快捷指令？** 👉 [提交新规则 / 功能需求](https://github.com/gurskyaskamug7878-commits/excel-ai-assistant/issues/new?template=feature-or-rule.yml)
* **遇到特殊 Excel 格式解析异常？** 👉 [提交 Bug 反馈](https://github.com/gurskyaskamug7878-commits/excel-ai-assistant/issues/new?template=bug-report.yml)
* **分享你的办公提效用法？** 👉 [前往 GitHub Discussions 交流](https://github.com/gurskyaskamug7878-commits/excel-ai-assistant/discussions)
* 觉得好用请点亮右上角的 **⭐ Star**，这是开源项目持续迭代的最大动力！

---

## 🇬🇧 English Overview

**AI Excel Assistant** is a privacy-first, zero-backend spreadsheet cleaning and workflow automation web app built for non-technical office professionals.

### ✨ Key Features
* **100% Local Browser Sandbox**: Powered by SheetJS (`xlsx`). Your sensitive HR/financial spreadsheets never leave your device.
* **Long-Number String Protection**: Enforces text cell typing (`t: 's', z: '@'`), preventing 18-digit ID cards and 11-digit phone numbers from turning into scientific notation (`1.38E+10`).
* **10-Dimension Data Health Checkup**: Detects empty rows/columns, duplicates, malformed phone/ID numbers, hidden spaces, and inconsistent date formats, generating a clean copy without mutating original data.
* **Safe AI Tool-Calling Workflow**: Translates natural language into structured JSON Schemas, requiring user confirmation before executing whitelisted operators (`remove_duplicates`, `merge_files`, `clean_data`, `vlookup_match`, `summarize_data`, `clean_names`).
* **Bounded Undo/Redo History**: 10-step immutable snapshot stack for instant rollback.
