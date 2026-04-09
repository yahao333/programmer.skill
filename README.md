<div align="center">

# programmer.skill

> *"It's not a bug — it's an undocumented feature."*

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Python 3.9+](https://img.shields.io/badge/Python-3.9%2B-blue.svg)](https://python.org)
[![Claude Code](https://img.shields.io/badge/Claude%20Code-Skill-blueviolet)](https://claude.ai/code)
[![AgentSkills](https://img.shields.io/badge/AgentSkills-Standard-green)](https://agentskills.io)

<br>

Every programmer has their own debugging style, their go-to stack,
their quirky habits when writing code,
and the specific way they review pull requests.

**Preserve coding wisdom and style — welcome to cyber-immortality!**

<br>

Provide source materials (code snippets, code reviews, chat logs, docs)
plus your understanding of their programming style,
and get an **AI Skill that carries their developer essence**

[数据来源](#支持的数据来源) · [安装](#安装) · [使用](#使用) · [效果示例](#效果示例) · [详细安装说明](INSTALL.md)

[**English**](README_EN.md) · [**中文**](README_ZH.md)

</div>

---

## 支持的数据来源

| 来源 | 说明 |
|------|------|
| GitHub/GitLab 代码 | 代码风格分析 |
| Code Review 记录 | CR 习惯分析 |
| Slack/飞书消息 | 工作沟通风格 |
| 技术文档/博客 | 技术偏好 |
| 直接粘贴文字 | 手动输入 |

---

## 安装

```bash
git clone https://github.com/yahao333/programmer.skill ~/.claude/skills/programmer
```

## 使用

在 Claude Code 中输入：

```
/programmer
```

### 管理命令

| 命令 | 说明 |
|------|------|
| `/programmer` | 调用 Programmer Skill 创建器 |
| `/list-programmers` | 列出所有已创建的 Programmer Skill |
| `/delete-programmer {slug}` | 删除指定 Programmer Skill |

---

## 效果示例

> 输入：`Go后端，5年经验，喜欢简洁代码，CR严格但给建议很有建设性，说话直接，技术视野广`

**场景一：代码审查**

```
用户      ❯ 帮我看看这个接口

programmer.skill ❯ 这个函数太长了，拆一下。
                  命名语义不明，
                  error handling 在这儿不合理。
                  （认真看完了）
                  整体架构还行，
                  但这两个地方需要改。
```


**场景二：技术讨论**

```
用户      ❯ 我想用微服务重构

programmer.skill ❯ 先想清楚为什么。
                  微服务解决的是组织问题，不是技术问题。
                  你们团队多大？
                  有没有 SRE 能力？
                  没有的话，先别折腾。
```

---

<div align="center">

MIT License © [yahao333](https://github.com/yahao333)

</div>
