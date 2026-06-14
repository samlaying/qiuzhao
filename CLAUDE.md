# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What This Is

An Obsidian vault serving as a personal interview preparation knowledge base for Chinese tech autumn recruitment (秋招). The owner is preparing for PM and operations roles (策略PM, 数据PM, 商业化PM, 用户/内容/产品运营). All content is in Chinese.

## Vault Structure & Conventions

- **Numbered prefixes** define sections: `00-` (resume), `01-` (methodology), `02-` (AIGC strategy), `03-` (interview), `04-` (product sense), `100+` (per-role prep)
- **100+ folders** follow a uniform layout: `能力要求.md` (core competency), optional `公司投递.md` (application tracker)
- `04-产品Sense/` has sub-structure: `面试题库/` (categorized by topic), `日常练习/` (drills)
- `02-AIGC策略/` files are numbered (`00-`, `01-`, `10-`, etc.) — the gap marks a logical grouping (core capabilities vs. company-specific prep)

## Obsidian Bidirectional Links (双链)

Files cross-reference each other with `[[wikilink]]` syntax. Key link patterns:
- Interview questions → applicable roles: `适用：[[100-策略PM]]、[[103-用户运营]]`
- Role folders → interview questions and reference materials
- Daily practice drills → specific roles or AIGC topics

When creating new files, add bidirectional link annotations so they surface from both directions.

## Templates

Templates live in `04-产品Sense/`:
- `岗位-模板.md` — scaffold for new role folders
- `练习-模板-产品分析.md`, `练习-模板-费米估算.md`, `练习-模板-竞品分析.md` — practice exercise formats

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
