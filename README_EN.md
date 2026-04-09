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

[Supported Sources](#supported-data-sources) · [Install](#install) · [Usage](#usage) · [Demo](#demo) · [Detailed Install](INSTALL.md)

[**English**](README_EN.md) · [**中文**](README_ZH.md)

</div>

---

## Supported Data Sources

| Source | Description |
|--------|-------------|
| GitHub/GitLab code | Code style analysis |
| Code Review records | CR habit analysis |
| Slack/Feishu messages | Work communication style |
| Tech docs/blogs | Technology preferences |
| Paste text directly | Manual input |

---

## Install

```bash
git clone https://github.com/yahao333/programmer.skill ~/.claude/skills/programmer
```

---

## Usage

In Claude Code, type:

```
/programmer
```

### Commands

| Command | Description |
|---------|-------------|
| `/programmer` | Invoke full Skill |
| `/programmer-code` | Code review mode |
| `/programmer-debug` | Debug mode |
| `/programmer-explain` | Tech explanation mode |

---

## Demo

> Input: `Go backend, 5 years experience, loves clean code, strict CR but gives constructive advice, direct speech, broad tech vision`

**Scenario 1: Code Review**

```
User            ❯ Help me review this API

programmer.skill ❯ This function is too long, split it.
                  Naming is unclear.
                  Error handling here is unreasonable.
                  (finishes reading)
                  Overall architecture is fine,
                  but these two places need changes.
```

**Scenario 2: Tech Discussion**

```
User            ❯ I want to refactor with microservices

programmer.skill ❯ First figure out why.
                  Microservices solve org problems, not tech problems.
                  How big is your team?
                  Do you have SRE capability?
                  If not, don't bother yet.
```

---

<div align="center">

MIT License © [yahao333](https://github.com/yahao333)

</div>
