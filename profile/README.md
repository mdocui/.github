### mdocUI

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
| [`@mdocui/react`](https://github.com/mdocui/mdocui/tree/main/packages/react) | React renderer, 22 default components, `useRenderer` hook |
| `@mdocui/cli` | Coming soon — scaffold, generate prompts, preview |

#### Get started

```bash
pnpm add @mdocui/core @mdocui/react
```

[View the full documentation](https://github.com/mdocui/mdocui)
