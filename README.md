# SEU PhD Thesis — Hermes Agent Skill

东南大学博士学位论文写作与参考文献处理 Skill，用于 [Hermes Agent](https://github.com/NousResearch/hermes-agent)。

## 功能

| 模块 | 内容 |
|------|------|
| 论文写作 | 绪论结构、实验章主线、讨论深度、结论聚焦、用词规范 |
| 参考文献管理 | 数量基准 (字数/300)、选择原则、插入范围 (12 项禁区)、引用格式 (顺序编码制) |
| 引用密度控制 | 单处 ≤3 篇、禁止 `[1-3][4-6]` 规避、自然融入文本 |
| 文献列表格式 | GB/T 7714 顺序编码制、6 种文献类型格式示例 |
| 融合去重 | 7 步工作流：映射 → 真实性 → 融合 → 去重 → 统一编号 → 删孤儿 → 修复 |
| 送审前检查 | 12 项检查报告 |

## 安装

```bash
# 克隆到 Hermes skills 目录
git clone https://github.com/<your-username>/seu-phd-thesis.git \
  "$HOME/AppData/Local/hermes/skills/research/seu-phd-thesis"

# 或者复制 SKILL.md 到已有目录
cp SKILL.md "$HOME/AppData/Local/hermes/skills/research/seu-phd-thesis/"
```

安装后启动新的 Hermes 会话即可自动加载。

## 触发关键词

东南大学博士论文, 学位论文写作, 参考文献插入, 引用格式检查, 送审前检查, 博士大论文, SEU thesis, 顺序编码制, GB/T 7714, 引用去重, 参考文献审校, 最终检查报告

## 依赖 Skill

本 skill 在操作工作流中会委托以下 skill：

- `nature-writing` — 章节起草/结构规划
- `nature-polishing` — 语言润色
- `nature-citation` — Nature/CNS 期刊引用
- `thesis-citation-audit` — DOCX 引用提取/交叉验证/去重/上标格式化 (python-docx)
- `document-editing` — Word 程序化编辑

## 作者

Aim1ya
