# SEU PhD Thesis Reference Skill

用于审查和受控修订东南大学博士学位论文中的参考文献、正文引用与顺序编号。

本 Skill 采用平台无关的 `SKILL.md` 指令，可供任何能够读取 Skill 文件、访问用户文档并输出报告或修改副本的 AI Agent 使用。

## 功能

| 模块 | 内容 |
|---|---|
| 引用真实性 | 禁止虚构文献；新增文献必须可核验并直接支撑正文陈述 |
| 引用映射 | 建立正文引用、文末条目和首次出现位置映射 |
| 编号管理 | 按首次出现顺序编号；同一文献复用唯一编号 |
| 数量控制 | 单处引用默认不超过 3 篇；禁止机械凑数和引用堆砌 |
| 受控修订 | 先审计、再修改、最后全文复核；不覆盖源文件 |
| 格式支持 | DOCX、Markdown、TXT、LaTeX 审计；PDF 默认只审计 |
| 最终报告 | 修改摘要、变更清单、风险、无法处理项和最终自检 |

## 安装

将整个仓库放入目标 Agent 支持的 Skill 目录，或让 Agent 直接读取本仓库中的 `SKILL.md`。

```bash
git clone https://github.com/miaozw97-ship-it/seu-phd-thesis.git
```

不同 Agent 的 Skill 安装目录和加载方式不同，请遵循对应平台的说明。

## 使用要求

- 提供完整论文或明确章节，并包含正文引用与参考文献表。
- 新增文献时，提供可核验的文献库、BibTeX/RIS、论文 PDF、DOI/数据库记录，或允许联网核验。
- 提供东南大学当前模板或学院规范时，Agent 才能确认校级格式细节。

## 测试

测试场景位于 [`references/test-cases.md`](references/test-cases.md)。

## 作者

Aim1ya
