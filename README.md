# drawio-template-pack

An OpenCode skill package for building thesis-friendly `draw.io` diagrams with a consistent black-and-white visual system, reusable `.drawio` templates, and template-selection guidance.

## Why this repo

This repository packages a complete `draw.io` workflow for OpenCode:

- a reusable skill definition in `SKILL.md`
- a style guide in `Drawio图风格模板.md`
- 8 starter `.drawio` templates with editable placeholders
- automatic template-routing rules for common diagram requests

It is designed for users who want to create new diagrams quickly while keeping a stable academic/technical diagram style.

## Highlights

- Unified thesis-style black-and-white diagram language
- Ready-to-edit templates instead of empty canvases
- Built-in guidance for element semantics and layout rules
- Automatic mapping from user intent to the nearest template type
- Suitable for architecture, function, ER, use-case, state, sequence, and page-structure diagrams

## Included templates

| Template | Use case |
| --- | --- |
| `templates/总体架构图模板.drawio` | System architecture, layered design, deployment structure |
| `templates/功能结构图模板.drawio` | Top-down function trees and module decomposition |
| `templates/功能模块划分图模板.drawio` | Role-based or responsibility-based functional grouping |
| `templates/数据库E-R图模板.drawio` | Chen-style entity-relationship modeling |
| `templates/用例图模板.drawio` | Actor-to-function relationships |
| `templates/状态流转图模板.drawio` | State transitions and lifecycle diagrams |
| `templates/业务时序图模板.drawio` | Multi-participant interaction over time |
| `templates/页面结构图模板.drawio` | Page hierarchy and information architecture |

## Repository structure

```text
drawio-template-pack/
├─ SKILL.md
├─ Drawio图风格模板.md
├─ LICENSE
├─ README.md
└─ templates/
   ├─ 总体架构图模板.drawio
   ├─ 功能结构图模板.drawio
   ├─ 功能模块划分图模板.drawio
   ├─ 数据库E-R图模板.drawio
   ├─ 用例图模板.drawio
   ├─ 状态流转图模板.drawio
   ├─ 业务时序图模板.drawio
   └─ 页面结构图模板.drawio
```

## Quick start

1. Copy this directory into your OpenCode skills directory.
2. Invoke the skill as `drawio-template-pack`.
3. Let the skill choose the right template, or open one manually from `templates/`.
4. Replace placeholder text, duplicate same-type nodes when needed, and keep the built-in style rules.

## How template routing works

- `分层 / 架构 / 部署` -> `总体架构图模板`
- `功能树 / 模块拆分` -> `功能结构图模板`
- `角色职责 / 分栏功能` -> `功能模块划分图模板`
- `实体 / 属性 / 关系` -> `数据库E-R图模板`
- `角色与系统功能关系` -> `用例图模板`
- `状态变化 / 生命周期` -> `状态流转图模板`
- `请求响应 / 交互顺序` -> `业务时序图模板`
- `页面树 / 信息架构` -> `页面结构图模板`

Detailed rules and element semantics are documented in `Drawio图风格模板.md`.

## Best for

- thesis figures and academic system design chapters
- teams that want one consistent `draw.io` style
- rapidly turning natural-language requests into usable diagram starters
- standardizing existing diagrams into a cleaner visual grammar

## License

MIT
