---
name: programmer
description: "Distill a programmer's coding style, problem-solving approach, and tech wisdom into an AI Skill. | 蒸馏程序员的编码风格、问题解决方式和技术智慧到一个 AI Skill 中。"
argument-hint: "[programmer-name-or-slug]"
version: "1.0.0"
user-invocable: true
allowed-tools: Read, Write, Edit, Bash
---

# 程序员.skill 创建器（Claude Code 版）

## 触发条件

当用户说以下任意内容时启动：
- `/programmer`
- "帮我创建一个程序员 skill"
- "我想蒸馏程序员"
- "新建程序员"
- "给我做一个程序员的 skill"

---

## 主流程：创建新程序员 Skill

### Step 1：基础信息录入

问 3 个问题：

1. **称呼**（必填）：你平时怎么称呼他/她？如「大佬」「同事」「师兄」
2. **基本信息**（一句话）：技术栈、年限、性格特点、代码风格
   - 示例：`10年经验后端，Python/Go，喜欢写简洁优雅的代码，急性子`
3. **特别技术风格**（可选）：他/她最标志性的代码习惯、架构思路或口头禅

### Step 2：原材料导入

询问用户提供原材料：

```
原材料怎么提供？

  [A] 代码片段
      GitHub、GitLab、代码片段

  [B] Code Review 记录
      他/她的 CR 意见、评论风格

  [C] 技术文档/博客
      他/她写的技术文档、博客文章

  [D] 聊天记录
      技术讨论、问题解答记录

  [E] 直接粘贴
      复制文字粘贴进来

可以混用，也可以跳过（仅凭手动信息生成）。
```

### Step 3：分析生成

将收集到的材料按三条线分析：

**线路 A（代码风格）**：
- 命名规范：变量、函数、类的命名风格
- 代码结构：模块化程度、函数长度、注释风格
- 代码审美：简洁 vs 详细，函数式 vs 面向对象

**线路 B（问题解决）**：
- 调试风格：print 大法 vs debug vs 日志
- 解决问题方式：先查文档 vs 先问人 vs 直接动手
- 技术好奇心：追新 vs 稳定、深度 vs 广度

**线路 C（沟通特点）**：
- CR 风格：严厉 vs 温和、具体 vs 抽象
- 技术表达：能通俗易懂解释 vs 满嘴技术术语
- 教学风格：给答案 vs 给思路

### Step 4：确认并写入

向用户展示摘要，确认后写入文件到 `./programmers/{slug}/`。

---

## 进化模式

用户追加新材料时，分析增量内容并 merge 到对应部分。

用户纠正时说「他不会这样」「她应该是」，更新对应内容。

---
---

# Programmer.skill Creator (Claude Code Edition)

## Trigger Conditions

Activate when the user says:
- `/programmer`
- "Help me create a programmer skill"
- "I want to distill my programmer"
- "New programmer"

---

## Main Flow: Create a New Programmer Skill

### Step 1: Basic Info (3 questions)

1. **Name/Nickname** (required): What do you call them? e.g., "Boss", "Colleague", "Senior"
2. **Basic Info** (one sentence): Tech stack, years of experience, personality, coding style
   - Example: `10-year backend developer, Python/Go, loves writing clean elegant code, impatient`
3. **Special Tech Style** (optional): Their most iconic coding habit, architecture approach, or catchphrase

### Step 2: Source Materials

```
How would you like to provide materials?

  [A] Code snippets
      GitHub, GitLab, code fragments

  [B] Code Review records
      Their CR comments, review style

  [C] Technical docs/blogs
      Technical documents, blog posts they wrote

  [D] Chat records
      Technical discussions, problem-solving records

  [E] Paste text
      Copy-paste directly
```

### Step 3: Analyze & Generate

Analyze collected materials along three tracks:

**Track A (Coding Style)**:
- Naming conventions: Variable, function, class naming style
- Code structure: Modularity, function length, comment style
- Code aesthetics: Concise vs detailed, functional vs OOP

**Track B (Problem Solving)**:
- Debugging style: print vs debug vs logs
- Problem approach: Read docs first vs ask first vs dive in
- Tech curiosity: Cutting-edge vs stable, deep vs broad

**Track C (Communication)**:
- CR style: Strict vs gentle, specific vs abstract
- Technical expression: Can explain simply vs full of jargon
- Teaching style: Gives answers vs gives direction

### Step 4: Confirm & Write

Show summary to user, write files to `./programmers/{slug}/` after confirmation.

---

## Evolution Mode

When user adds new materials, analyze delta and merge into relevant sections.

When user corrects with "they wouldn't do that" / "they should be", update content.
