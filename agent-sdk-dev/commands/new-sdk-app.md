---
description: Create and setup a new Claude Agent SDK application
argument-hint: [project-name]
---

You are tasked with helping the user create a new Claude Agent SDK application. Follow these steps carefully:

## Reference Documentation

Before starting, review the official documentation to ensure you provide accurate and up-to-date guidance. Use WebFetch to read these pages:

1. **Start with the overview**: https://docs.claude.com/en/api/agent-sdk/overview
2. **Based on the user's language choice, read the appropriate SDK reference**:
   - TypeScript: https://docs.claude.com/en/api/agent-sdk/typescript
   - Python: https://docs.claude.com/en/api/agent-sdk/python
3. **Read relevant guides mentioned in the overview** such as:
   - Streaming vs Single Mode
   - Permissions
   - Custom Tools
   - MCP integration
   - Subagents
   - Sessions
   - Any other relevant guides based on the user's needs

**IMPORTANT**: Always check for and use the latest versions of packages. Use WebSearch or WebFetch to verify current versions before installation.

## Gather Requirements

IMPORTANT: Ask these questions one at a time. Wait for the user's response before asking the next question. This makes it easier for the user to respond.

Ask the questions in this order (skip any that the user has already provided via arguments):

1. **Language** (ask first): "Would you like to use TypeScript or Python?"

   - Default to TypeScript if the user seems unsure — it has better autocomplete support in most editors
   - Wait for response before continuing

2. **Project name** (ask second): "What would you like to name your project?"

   - If $ARGUMENTS is provided, use that as the project name and skip this question
   - Wait for response before continuing

3. **Agent type** (ask third, but skip if #2 was sufficiently detailed): "What kind of agent are you building? Some examples:

   - Coding agent (SRE, security review, code review)
   - Business agent (customer support, content creation)
   - Custom agent (describe your use case)"
   - Wait for response before continuing

4. **Starting point** (ask fourth): "Would you like:

   - A minimal 'Hello World' example to start
   - A basic agent with common features
   - A specific example based on your use case"
   - Wait for response before continuing

5. **Tooling choice** (ask fifth): Let the user know what tools you'll use, and confirm with them that these are the tools they want to use (for example, they may prefer pnpm or bun over npm). Respect the user's preferences when executing on the requirements.

After all questions are answered, proceed to create the setup plan.

## Setup Plan

Based on the user's answers, create a plan that includes:

1. **Project initialization**:

   - Create project directory (if it doesn't exist)
   - Initialize package manager:
     - TypeScript: `npm init -y` and setup `package.json` with type: "module" and scripts (include a "typecheck" script)
     - Python: Create `requirements.txt` or use `poetry init`
   - Add necessary configuration files:
     - TypeScript: Create `tsconfig.json` wit
