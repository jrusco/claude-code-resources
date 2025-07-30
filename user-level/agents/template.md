---
name: your-sub-agent-name
description: Description of when this subagent should be invoked
tools: tool1, tool2, tool3  # Optional - inherits all tools if omitted
---

Your subagent's system prompt goes here. This can be multiple paragraphs and should clearly define the subagent's role, capabilities, and approach to solving problems.

Include specific instructions, best practices, and any constraints the subagent should follow.

Subagents start off with a clean slate each time they are invoked and may add latency as they gather context that they require to do their job effectively.

check docs at [](https://docs.anthropic.com/en/docs/claude-code/sub-agents)
