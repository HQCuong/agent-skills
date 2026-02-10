# agent-skills

## Skills CLI

https://github.com/vercel-labs/skills

## Common skills

https://skills.sh/vercel-labs/skills/find-skills
```
npx skills add https://github.com/vercel-labs/skills --skill find-skills
```

## FE

### Vue.js

https://github.com/antfu/skills
```
npx skills add https://github.com/antfu/skills --skill antfu
```

### Javascript / Typescript

https://github.com/wshobson/agents/blob/main/docs/agent-skills.md#javascripttypescript-4-skills

- javascript

https://skills.sh/wshobson/agents/javascript-testing-patterns
```
npx skills add https://github.com/wshobson/agents --skill javascript-testing-patterns
```

https://skills.sh/wshobson/agents/modern-javascript-patterns
```
npx skills add https://github.com/wshobson/agents --skill modern-javascript-patterns
```

- typescript

https://skills.sh/wshobson/agents/typescript-advanced-types
```
npx skills add https://github.com/wshobson/agents --skill typescript-advanced-types
```

### Context7 instruction
Always use context7 when I need code generation, setup or configuration steps, or library/API documentation. This means you should automatically use the Context7 MCP tools to resolve library id and get library docs without me having to explicitly ask.

### Codebase instruction
You must always understand the entire codebase as a system, not isolated files.

Rules:
- Always inspect project structure, architecture, and conventions before answering.
- Never analyze or modify a file in isolation:
  - Identify related files via imports, callers, shared state, types, and configs.
- Reason explicitly about dependencies, data flow, and side effects.
- Respect existing architecture and patterns; do not introduce new ones without justification.
- Before suggesting changes, assess impact on other modules, APIs, tests, and runtime behavior.
- If context is missing, state assumptions clearly and request relevant files only when necessary.

Mindset:
Think like a maintainer, not a snippet generator. Optimize for correctness, consistency, and long-term stability.
