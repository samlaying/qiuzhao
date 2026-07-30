# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What This Is

An Obsidian vault serving as a personal interview preparation knowledge base for Chinese tech autumn recruitment (秋招). The owner is preparing for PM and operations roles (策略PM, 数据PM, 商业化PM, 用户/内容/产品运营). All content is in Chinese.

## Vault Structure & Conventions

- **Root entry folders** define navigation: `00-开始这里.md` is the home page, followed by `100-基础资料/`, the role folders `110-` through `170-`, `180-公司专项与转岗/`, and `200-面试材料/`.
- **Numbered folders** define storage lifecycle: `10-` raw material, `20-` personal facts/projects, `30-` general knowledge, `40-` question answers, `50-` role preparation, `60-` interview events, `70-` training/evaluation, `80-` indexes, `90-` archive.
- **100+ folders** follow a uniform layout: `能力要求.md` (core competency), optional `公司投递.md` (application tracker)
- Product sense and AI product materials are copied into each role’s `03-通用知识/` folder.

## Obsidian Bidirectional Links (双链)

Files cross-reference each other with `[[wikilink]]` syntax. Key link patterns:
- Interview questions are stored inside each applicable role’s `04-题库回答/` folder.
- Role folders → interview questions and reference materials
- Daily practice drills → specific roles or AIGC topics

When creating new files, add bidirectional link annotations so they surface from both directions.

## Templates

Templates live under `00-系统/` and the relevant knowledge sections. Use the existing practice templates for product analysis, Fermi estimates, and competitor analysis.

When adding a new role, create a `1XX-角色名/` folder and follow the template.

## File Naming

- Resume content: `录音-*`, `项目介绍-*`, `逐字稿-*`
- AIGC strategy: numeric prefix for ordering, descriptive Chinese name
- Interview questions: one file per question, placed in the appropriate `面试题库/` subfolder (`业务理解/`, `能力考察/`, `案例分析/`, `开放题/`)
- Mock materials: prefixed `Mock*`

## Editing Guidelines

- Write all new content in Chinese
- Keep markdown formatting compatible with Obsidian (no Hugo/Jekyll frontmatter beyond what Obsidian generates)
- Maintain the numbering scheme when inserting new files into existing sections
- Use tables for structured data (competency matrices, estimation formulas, drill schedules)
- Interview answers should follow the pattern: **conclusion first → framework → quantified evidence**

## Git

The `.obsidian/` config directory and `.DS_Store` are gitignored. Only markdown content is tracked.
