# Repository Guidelines

## Project Structure & Module Organization

This repository is an Obsidian vault for Chinese autumn-recruitment interview preparation. Organize content by lifecycle:

- `00-系统/`: directory rules, templates, metadata schema, workflow, and archive rules.
- `10-原始材料/`: unprocessed interview notes, job descriptions, transcripts, screenshots, and articles.
- Each root role folder (`110-` through `170-`) contains `01-岗位准备/`, `02-个人项目/`, `03-通用知识/`, `04-题库回答/`, `05-面经录音/`, `06-面试复盘/`, and `07-训练记录/`.
- `10-原始材料/`, `60-面试事件/`, `70-训练评测/`, and `90-归档/` are backend/source areas, not primary navigation entries.

Keep new source material in `10-原始材料/`; do not place it directly in compiled knowledge areas. Folders describe lifecycle, not every way a note may be found.

## Classification & Retrieval

The primary user journey is **根目录 → 岗位文件夹 → 目标内容**. Keep this path within two clicks whenever possible. `00-开始这里.md` lists the numbered root entries; do not make users browse backend folders first.

Use separate dimensions so one note can be found from multiple directions:

- **Lifecycle/folder:** raw input → personal facts or general knowledge → question answers → role preparation → interview event → evaluation → archive.
- **Role family:** keep product roles (for example `策略PM`, `数据PM`, `商业化PM`, `AI/Agent产品`) and operations roles (for example `用户运营`, `内容运营`, `产品运营`, `策略运营`) as the first navigation grouping. A company or job posting belongs beneath the relevant role family, not above it.
- **Type:** `raw`, `project`, `knowledge`, `question`, `job_package`, `interview`, or `evaluation`.
- **Facets:** record `related_roles`, `related_projects`, company, interview round, topic, status, and evidence level in frontmatter when applicable.
- **Navigation:** every role entry should link to the same compact set of destinations: `能力要求`, `岗位/公司准备`, `题库回答`, `项目素材`, `面试复盘`, and `训练记录`. Link one note from multiple MOCs instead of duplicating it.

Classify in this order: source/confidence, reusable output, related roles/projects/topics, then readiness. Use nested tags such as `#type/question`, `#role/策略PM`, `#topic/Agent评测`, and `#status/review` only when frontmatter or an existing MOC cannot express the facet. Follow names in `00-系统/03-元数据Schema.md`.

For fast lookup, start from a numbered role folder, then filter by destination or topic. Examples: `path:"110-产品-策略PM/04-题库回答"`, `path:"140-运营-用户运营/05-面经录音"`, or `Agent 评测`. Shared content is copied into each relevant role by design. Do not rely on filenames alone.

When adding a role, create a numbered root folder and its `00-岗位总览.md`, then copy the seven standard content sections from an existing role. Keep role pages shallow; do not create extra subfolders unless they represent a stable retrieval need.

## Build, Test, and Development Commands

There is no software build or automated test suite. The normal workflow is to add material to `10-原始材料/` and run the repository’s `process-inbox` workflow when available. Review classification, generated links, MOCs, and indexes in Obsidian afterward. Use `git diff --check` to catch whitespace errors and `git status` to review changed files.

## Coding Style & Naming Conventions

Write new content in Chinese Markdown, using UTF-8 and Obsidian-compatible `[[wikilink]]` references. Preserve the numbered directory scheme and use descriptive names such as `项目介绍-*.md`, `逐字稿-*.md`, `能力要求.md`, and `Mock*.md`. Use tables for structured comparisons, matrices, and schedules. Put conclusions before frameworks and quantified evidence in interview answers.

## Testing Guidelines

Validate changes manually in Obsidian: check that wikilinks resolve, headings and tables render correctly, and generated indexes point to the intended notes. Never overwrite original source text; verify that facts and numbers remain unchanged.

## Commit & Pull Request Guidelines

Use concise Chinese imperative-style commit subjects that describe the content change, for example `新增字节面经整理` or `修复索引链接`. Keep commits focused. Pull requests should explain the affected vault sections, identify any new or moved notes, mention link/index validation, and include screenshots when rendering or navigation changes are relevant.

## Content Safety Rules

Preserve provenance for every compiled note. Do not delete originals, turn inferences into quoted interview statements, or mix role-specific preparation into general knowledge. Low-confidence material belongs in the pending-review queue; archive old content instead of deleting it.
