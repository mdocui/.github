<p align="center">
  <img src="https://raw.githubusercontent.com/mdocui/.github/main/assets/logo.png" alt="mdocUI" width="400">
</p>

<p align="center">
  <a href="https://www.npmjs.com/package/@mdocui/core"><img src="https://img.shields.io/npm/v/@mdocui/core?label=%40mdocui%2Fcore&color=blue" alt="npm core"></a>
  <a href="https://www.npmjs.com/package/@mdocui/react"><img src="https://img.shields.io/npm/v/@mdocui/react?label=%40mdocui%2Freact&color=blue" alt="npm react"></a>
  <a href="https://www.npmjs.com/package/@mdocui/cli"><img src="https://img.shields.io/npm/v/@mdocui/cli?label=%40mdocui%2Fcli&color=blue" alt="npm cli"></a>
  <a href="https://github.com/mdocui/mdocui"><img src="https://img.shields.io/github/stars/mdocui/mdocui?style=social" alt="GitHub stars"></a>
</p>

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
mkdir -p .claude/skills/mdocui
curl -o .claude/skills/mdocui/SKILL.md https://raw.githubusercontent.com/mdocui/mdocui/main/SKILL.md
```

Then invoke with `/mdocui` in any conversation.

#### Links

- [Documentation](https://mdocui.github.io) | [Live Demo](https://mdocui.vercel.app) | [Examples](https://github.com/mdocui/examples) | [SKILL.md](https://github.com/mdocui/mdocui/blob/main/SKILL.md) | [llms.txt](https://mdocui.github.io/llms.txt)
