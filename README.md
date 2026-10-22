# Default Privacy skills

Skills that help an AI assistant give ordered, sourced privacy advice, backed by [Default Privacy](https://defaultprivacy.com)'s free directory of privacy tools, guides and stacks.

## Skills

**be-hard-to-find** loads when someone asks how to be harder to find: "how do I know if I'm doxxed", "what's out there about me", "someone found where I live", "I'm moving and don't want to be found". It works the way the person searching for you does, and cuts each source before cleaning the pages it feeds: people-search and data-broker removals, why they come back, California's DROP, address confidentiality programs, reused usernames and opt-out traps. For anyone who may be in danger, it starts with a safety plan.

## Install

Claude Code:

```
/plugin marketplace add privatebydefault/privacy-skills
/plugin install default-privacy@privacy-skills
```

This installs the skill and the Default Privacy connector (`https://mcp.defaultprivacy.com/`), so the skill can pull current guides and tools. No account or API key.

Other agents that read `SKILL.md` files:

```
npx skills add privatebydefault/privacy-skills
```

The connector on its own, for Claude, ChatGPT and other AI apps: [defaultprivacy.com/ai](https://defaultprivacy.com/ai).

## What it sends

The skill runs no code. The connector it adds is read-only and needs no account. Your AI sends it search keywords, situation ids and page or tool names, plus a product name, domain or MCP server address when you ask it to check one. It gets back guides, tool records, stacks and check results. Default Privacy keeps daily counts of which tools and pages are used, and doesn't store what an assistant sends to look something up. Its host keeps basic request logs. Default Privacy never asks for your name, address or email, and the skill tells the AI not to ask either. Privacy policy: https://defaultprivacy.com/privacy

## If you are in danger

If someone is tracking or threatening you, deleting accounts or changing settings can alert them. Plan visible changes with a trained advocate first. In the US, the National Domestic Violence Hotline is free, confidential and open 24/7: call 1-800-799-7233 or text START to 88788.

## License

MIT
