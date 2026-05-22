<h1 align="center">Awesome Claude Code Plugins</h1>

<p align="center">
<a href="https://dashboard.composio.dev/login?utm_source=Github&utm_medium=Banner&utm_content=AwesomePlugins">
  <img width="1280" alt="Awesome Claude Plugins" src="./cover_image.png">
</a>
</p>

<p align="center">
  <a href="https://awesome.re">
    <img src="https://awesome.re/badge.svg" alt="Awesome" />
  </a>
  <a href="https://makeapullrequest.com">
    <img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square" alt="PRs Welcome" />
  </a>
  <a href="https://opensource.org/licenses/MIT">
    <img src="https://img.shields.io/badge/License-MIT-blue.svg?style=flat-square" alt="License: MIT" />
  </a>
</p>

<div>
<p align="center">
  <a href="https://twitter.com/composio">
    <img src="https://img.shields.io/badge/Follow%20on%20X-000000?style=for-the-badge&logo=x&logoColor=white" alt="Follow on X" />
  </a>
  <a href="https://www.linkedin.com/company/composiohq/">
    <img src="https://img.shields.io/badge/Follow%20on%20LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="Follow on LinkedIn" />
  </a>
  <a href="https://discord.com/invite/composio">
    <img src="https://img.shields.io/badge/Join%20our%20Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white" alt="Join our Discord" />
  </a>
</p>
</div>

<p align="center">
A curated list of production-ready plugins for Claude Code to supercharge your development workflow.
</p>

> **Want plugins that do more than generate text?** The [connect-apps](./connect-apps) plugin lets Claude send emails, create issues, post to Slack, and take actions across 500+ apps.

---

<!-- Personal note: I'm mainly using this for the GitHub + Slack integrations in my side projects. The connect-apps setup was pretty painless once I had my API key ready. -->

## Quickstart: Connect Claude to 500+ Apps

The **[connect-apps](./connect-apps)** plugin lets Claude perform real actions - send emails, create issues, post to Slack. It handles auth and connects to 500+ apps using Composio under the hood.

### 1. Clone & Run

```bash
git clone https://github.com/composiohq/awesome-claude-plugins.git
cd awesome-claude-plugins
claude --plugin-dir ./connect-apps
```

### 2. Run Setup

```shell
/connect-apps:setup
```

Paste your API key when asked. (Get a free key at [dashboard.composio.dev](https://dashboard.composio.dev/login?utm_source=Github&utm_medium=Banner&utm_content=AwesomePlugins))

### 3. Try It

Ask Claude to send you a test email. If you receive it, Claude is now connected to 500+ apps.

**[See all supported apps →](https://composio.dev/tools)**

---

## Contents

- [What Are Claude Plugins?](#what-are-claude-plugins)
- [Plugins](#plugins)
  - [Integrations](#integrations)
  - [Frontend & Design](#frontend--design)
  - [Git & Version Control](#git--version-control)
  - [Code Quality & Testing](#code-quality--testing)
  - [Backend & Architecture](#backend--architecture)
  - [DevOps & Performance](#devops--performance)
  - [Documentation & Security](#documentation--security)
  - [Developer Productivity](#developer-productivity)
  - [Companion & Personality](#companion-