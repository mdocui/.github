### mdocUI

[![npm core](https://img.shields.io/npm/v/@mdocui/core?label=%40mdocui%2Fcore&color=blue)](https://www.npmjs.com/package/@mdocui/core)
[![npm react](https://img.shields.io/npm/v/@mdocui/react?label=%40mdocui%2Freact&color=blue)](https://www.npmjs.com/package/@mdocui/react)
[![npm cli](https://img.shields.io/npm/v/@mdocui/cli?label=%40mdocui%2Fcli&color=blue)](https://www.npmjs.com/package/@mdocui/cli)
[![GitHub stars](https://img.shields.io/github/stars/mdocui/mdocui?style=social)](https://github.com/mdocui/mdocui)

Generative UI for LLMs using Markdoc `{% %}` tag syntax inline with markdown prose.

LLMs write natural markdown **and** drop interactive components — charts, buttons, forms, tables — all in the same stream. No custom DSL, no JSON blocks, no JSX confusion.

```
The Q4 results show strong growth.

{% chart type="bar" labels=["Jan","Feb","Mar"] values=[120,150,180] /%}

Revenue grew **12%**. Want to dig deeper?

{% button action="continue" label="Show by region" /%}
```

#### Packages

| Package | Description |
|---------|-------------|
| [`@mdocui/core`](https://github.com/mdocui/mdocui/tree/main/packages/core) | Streaming parser, component registry, system prompt generator |
| [`@mdocui/react`](https://github.com/mdocui/mdocui/tree/main/packages/react) | React renderer, 24 theme-neutral components, `useRenderer` hook |
| [`@mdocui/cli`](https://github.com/mdocui/mdocui/tree/main/packages/cli) | Scaffold, generate system prompts, preview |

#### Get started

```bash
pnpm add @mdocui/core @mdocui/react
```

#### For AI coding agents

Install the mdocUI skill in Claude Code:

```bash
mkdir -p .claude/skills
curl -o .claude/skills/mdocui.md https://raw.githubusercontent.com/mdocui/mdocui/main/SKILL.md
```

#### Links

- [Documentation](https://mdocui.github.io) | [Examples](https://github.com/mdocui/examples) | [SKILL.md](https://github.com/mdocui/mdocui/blob/main/SKILL.md) | [llms.txt](https://mdocui.github.io/llms.txt)
