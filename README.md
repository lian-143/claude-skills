# Claude skills

The 31 Claude Code skills used for the Mizrahi Law automation work (UCC CRM, n8n workflows, Tool Hub).

## Install

Copy the folders you want into your personal skills folder, then restart Claude Code:

```bash
git clone https://github.com/lian-143/claude-skills.git
cp -r claude-skills/skills/* ~/.claude/skills/        # all skills, for every project
# or, for one project only: cp -r claude-skills/skills/<name> <project>/.claude/skills/
```

Windows (PowerShell): `Copy-Item -Recurse claude-skills\skills\* $HOME\.claude\skills\`

## n8n (workflow building)

| Skill | What it is for |
|---|---|
| [n8n-agents](skills/n8n-agents/SKILL.md) | Design n8n AI agents the right way. |
| [n8n-binary-and-data](skills/n8n-binary-and-data/SKILL.md) | Handle files and binary data in n8n correctly. |
| [n8n-code-javascript](skills/n8n-code-javascript/SKILL.md) | Write JavaScript code in n8n Code nodes. |
| [n8n-code-python](skills/n8n-code-python/SKILL.md) | Write Python code in n8n Code nodes. |
| [n8n-code-tool](skills/n8n-code-tool/SKILL.md) | Write JavaScript or Python for the n8n Custom Code Tool (@n8n/n8n-nodes-langchain.toolCode) — the AI-agent-callable tool, NOT the workflow Code node. |
| [n8n-error-handling](skills/n8n-error-handling/SKILL.md) | Wire n8n error handling so failures are loud, structured, and recoverable. |
| [n8n-expression-syntax](skills/n8n-expression-syntax/SKILL.md) | Validate n8n expression syntax and fix common errors. |
| [n8n-mcp-tools-expert](skills/n8n-mcp-tools-expert/SKILL.md) | Expert guide for using n8n-mcp MCP tools effectively. |
| [n8n-multi-instance](skills/n8n-multi-instance/SKILL.md) | Use when an n8n-mcp account targets more than one n8n instance (prod vs staging, several clients). |
| [n8n-node-configuration](skills/n8n-node-configuration/SKILL.md) | Operation-aware node configuration guidance. |
| [n8n-self-hosting](skills/n8n-self-hosting/SKILL.md) | Deploy a production self-hosted n8n end-to-end to a fresh Linux VM over SSH, using Docker Compose behind a Caddy reverse proxy with automatic HTTPS. |
| [n8n-subworkflows](skills/n8n-subworkflows/SKILL.md) | Build reusable, composable n8n sub-workflows. |
| [n8n-validation-expert](skills/n8n-validation-expert/SKILL.md) | Interpret validation errors and guide fixing them. |
| [n8n-workflow-patterns](skills/n8n-workflow-patterns/SKILL.md) | Proven workflow architectural patterns from real n8n workflows. |
| [using-n8n-mcp-skills](skills/using-n8n-mcp-skills/SKILL.md) | Use when building, editing, validating, testing, or debugging an n8n workflow through the n8n-mcp MCP server — designing a flow, configuring a node, writing an expression or Code node, wiring credentials, or fixing one that misbehaves. |

## Engineering

| Skill | What it is for |
|---|---|
| [clean-code](skills/clean-code/SKILL.md) | Pragmatic coding standards - concise, direct, no over-engineering, no unnecessary comments |
| [code-reviewer](skills/code-reviewer/SKILL.md) | Comprehensive code review skill for TypeScript, JavaScript, Python, Swift, Kotlin, Go. |
| [senior-architect](skills/senior-architect/SKILL.md) | Comprehensive software architecture skill for designing scalable, maintainable systems using ReactJS, NextJS, NodeJS, Express, React Native, Swift, Kotlin, Flutter, Postgres, GraphQL, Go, Python. |
| [senior-backend](skills/senior-backend/SKILL.md) | Comprehensive backend development skill for building scalable backend systems using NodeJS, Express, Go, Python, Postgres, GraphQL, REST APIs. |
| [senior-frontend](skills/senior-frontend/SKILL.md) | Comprehensive frontend development skill for building modern, performant web applications using ReactJS, NextJS, TypeScript, Tailwind CSS. |
| [senior-fullstack](skills/senior-fullstack/SKILL.md) | Comprehensive fullstack development skill for building complete web applications with React, Next.js, Node.js, GraphQL, and PostgreSQL. |
| [senior-prompt-engineer](skills/senior-prompt-engineer/SKILL.md) | World-class prompt engineering skill for LLM optimization, prompt patterns, structured outputs, and AI product development. |
| [senior-security](skills/senior-security/SKILL.md) | Comprehensive security engineering skill for application security, penetration testing, security architecture, and compliance auditing. |

## Design / UI

| Skill | What it is for |
|---|---|
| [frontend-design](skills/frontend-design/SKILL.md) | Guidance for distinctive, intentional visual design when building new UI or reshaping an existing one. |
| [mobile-design](skills/mobile-design/SKILL.md) | Mobile-first design thinking and decision-making for iOS and Android apps. |
| [ui-design-system](skills/ui-design-system/SKILL.md) | UI design system toolkit for Senior UI Designer including design token generation, component documentation, responsive design calculations, and developer handoff tools. |
| [ui-ux-pro-max](skills/ui-ux-pro-max/SKILL.md) | UI/UX design intelligence. |

## Documents & files

| Skill | What it is for |
|---|---|
| [docx](skills/docx/SKILL.md) | Use this skill whenever the user wants to create, read, edit, or manipulate Word documents (.docx files). |
| [file-organizer](skills/file-organizer/SKILL.md) | Intelligently organizes files and folders by understanding context, finding duplicates, and suggesting better organizational structures. |
| [pdf-processing-pro](skills/pdf-processing-pro/SKILL.md) | Production-ready PDF processing with forms, tables, OCR, validation, and batch operations. |

## Meta

| Skill | What it is for |
|---|---|
| [skill-creator](skills/skill-creator/SKILL.md) | Create new skills, modify and improve existing skills, and measure skill performance. |

## Licences

* `docx`, `frontend-design` and `skill-creator` come from Anthropic and keep their own `LICENSE.txt`; `docx` is proprietary, so this repository stays **private**.
* The `n8n-*` skills are the community n8n-mcp skills pack.
* No credentials are stored here: the `.env.*.example` files in `n8n-self-hosting` contain placeholders only.
