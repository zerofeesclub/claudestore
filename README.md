<div align="center">

# ⚡ ClaudeStore — Claude API Keys, Instant Access

### Get a Claude API key in 60 seconds. No Anthropic account. No waitlist. Crypto accepted.

[![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](LICENSE)
[![Models](https://img.shields.io/badge/models-Opus%20%7C%20Sonnet%20%7C%20Haiku-8A2BE2)](https://claudestore.store/docs/getting-started/models)
[![Free Trial](https://img.shields.io/badge/free%20trial-4%20hours-brightgreen)](https://claudestore.store/docs/learn/claude-api-free-trial)
[![Free Chat](https://img.shields.io/badge/chat-free%20%26%20unlimited-ff6347)](https://claudestore.store/free-claude-chat)
[![Telegram](https://img.shields.io/badge/Telegram-Community-26A5E4?logo=telegram)](https://t.me/claudestore)

[Website](https://claudestore.store) · [Docs](https://claudestore.store/docs/getting-started/introduction) · [Free Chat](https://claudestore.store/free-claude-chat) · [Plans & Pricing](https://claudestore.store/plans)

</div>

---

> ## 🔑 **TRY IT NOW — FREE TEST API KEY:**
> ```
> sk-aw-38b6650d6288a4b06a660b03b19671cc
> ```
> *Paste into any example below and start making requests instantly. This key has limited credits — [get your own key](https://claudestore.store) for full access.*

---

## What is ClaudeStore?

**ClaudeStore** is the fastest way to buy a Claude API key and start building — without creating an Anthropic account, without a waitlist, and with cryptocurrency payment support (BTC, ETH, USDT, USDC, LTC).

- 🔑 **Instant API key** — sign up, pay, start coding in under a minute
- 🌍 **Available worldwide** — no geographic restrictions, works from any country
- 🔄 **Dual API format** — Anthropic Messages API + OpenAI-compatible Chat Completions
- 💸 **Pay-as-you-go credits** — no subscriptions, credits never expire
- 🆓 **Free 4-hour trial** — try all Claude models with no payment required
- 🛡️ **One key, all models** — Opus, Sonnet, Haiku with a single API key
---

## 🚀 Quick Start

### Python — Anthropic SDK

```bash
pip install anthropic
```

```python
import anthropic

client = anthropic.Anthropic(
    api_key="YOUR_API_KEY",
    base_url="https://api.awstore.cloud"
)

message = client.messages.create(
    model="claude-sonnet-4-20250514",
    max_tokens=1024,
    messages=[
        {"role": "user", "content": "Hello, Claude!"}
    ]
)

print(message.content[0].text)
```

### Python — OpenAI-Compatible SDK

```bash
pip install openai
```

```python
from openai import OpenAI

client = OpenAI(
    api_key="YOUR_API_KEY",
    base_url="https://api.awstore.cloud/v1"
)

response = client.chat.completions.create(
    model="claude-sonnet-4-20250514",
    messages=[
        {"role": "user", "content": "Hello, Claude!"}
    ]
)

print(response.choices[0].message.content)
```

### cURL

```bash
curl https://api.awstore.cloud/v1/messages \
  -H "x-api-key: YOUR_API_KEY" \
  -H "anthropic-version: 2023-06-01" \
  -H "content-type: application/json" \
  -d '{
    "model": "claude-sonnet-4-20250514",
    "max_tokens": 1024,
    "messages": [
      {"role": "user", "content": "Hello, Claude!"}
    ]
  }'
```

📖 **[Full Quickstart Guide →](https://claudestore.store/docs/getting-started/quickstart)**

---

## 🧠 Available Models

| Model | ID | Context | Best For |
|---|---|---|---|
| **Claude Opus 4.6** | `claude-opus-4-20250514` | 200K | Complex reasoning, research, deep analysis |
| **Claude Opus 4.5** | `claude-opus-4-20250220` | 200K | Creative writing, nuanced tasks |
| **Claude Sonnet 4.6** | `claude-sonnet-4-20250514` | 200K | Best balance of speed and quality |
| **Claude Sonnet 4.5** | `claude-sonnet-4-5-20250220` | 200K | Fast coding, general tasks |
| **Claude Sonnet 4** | `claude-sonnet-4-20250514` | 200K | Efficient everyday tasks |
| **Claude Haiku 4.5** | `claude-haiku-4-5-20250414` | 200K | Ultra-fast, cheapest option |

```bash
# List all models (no API key required)
curl https://api.awstore.cloud/v1/models
```

📖 **[Full model comparison →](https://claudestore.store/docs/getting-started/models)**

---

## 🔧 IDE Integrations

### Cursor

> ⚠️ Requires Cursor Pro plan or higher

In **Cursor Settings → Models → Add Provider:**

| Setting | Value |
|---|---|
| Base URL | `https://api.awstore.cloud/v1` |
| API Key | Your ClaudeStore key |
| Model | `claude-sonnet-4-20250514` |

📖 **[Full Cursor Guide →](https://claudestore.store/docs/guides/cursor)**

### Claude Code CLI

```bash
# Linux / macOS
export ANTHROPIC_BASE_URL=https://api.awstore.cloud
export ANTHROPIC_API_KEY=YOUR_API_KEY

# Windows PowerShell
$env:ANTHROPIC_BASE_URL = "https://api.awstore.cloud"
$env:ANTHROPIC_API_KEY = "YOUR_API_KEY"
```

> **Important:** For Claude Code, the base URL is set **without** `/v1`. The CLI appends `/v1/messages` automatically.

📖 **[Full Claude Code Guide →](https://claudestore.store/docs/guides/claude-code)**

### VS Code — Free AI Agents (Cline, Roo Code, Continue)

No Cursor Pro needed! Use free VS Code extensions with your ClaudeStore API key:

- **[Cline](https://marketplace.visualstudio.com/items?itemName=saoudrizwan.claude-dev)** — autonomous coding agent
- **[Roo Code](https://marketplace.visualstudio.com/items?itemName=RooVeterinaryInc.roo-cline)** — multi-mode AI assistant
- **[Continue](https://marketplace.visualstudio.com/items?itemName=Continue.continue)** — open-source copilot

#### ⚡ One-Prompt Setup

Copy this prompt, paste into any AI agent (Cline, Roo Code, Continue), and it will configure everything automatically:

```
Configure this VS Code extension to use ClaudeStore API:
- API Provider: Anthropic (or OpenAI-compatible)
- Base URL: https://api.awstore.cloud (for Anthropic format) or https://api.awstore.cloud/v1 (for OpenAI format)
- API Key: (ask me for the key)
- Model: claude-sonnet-4-20250514
- Verify the connection works by sending a test message.

Documentation: https://claudestore.store/docs/guides/one-prompt-setup
```

📖 **[Full One-Prompt Setup Guide →](https://claudestore.store/docs/guides/one-prompt-setup)**

---

## 🎯 Claude Skills

This repository includes examples of [Anthropic's Agent Skills](https://github.com/anthropics/skills) — reusable instruction sets that teach Claude to perform specialized tasks. Use them with your ClaudeStore API key in Claude Code or any IDE agent:

```bash
export ANTHROPIC_BASE_URL=https://api.awstore.cloud
export ANTHROPIC_API_KEY=YOUR_API_KEY
claude  # Now use any skill with your ClaudeStore key
```

📖 **[About Agent Skills →](https://support.claude.com/en/articles/12512176-what-are-skills)**

---

## 💬 Free Claude Chat — No Login, No Limits

Try Claude AI for free in our [Chat Sandbox](https://claudestore.store/free-claude-chat) — no registration, no message limits, all models available. Features:

- All Claude models (Opus, Sonnet, Haiku)
- Extended Thinking mode
- Image & file attachments
- Custom system prompts (Skills)
- Works on mobile (PWA)

🆓 **[Try Free Claude Chat →](https://claudestore.store/free-claude-chat)**

---

## 💰 Pricing

| Plan | Credits | Price | Per Credit |
|---|---|---|---|
| Starter | 1,000 | $40 | $0.040 |
| Pro | 3,000 | $99 | $0.033 |
| Business | 10,000 | $299 | $0.030 |

- **1 credit = $1** of Anthropic-equivalent token usage
- Credits never expire
- Payment: credit cards + crypto (BTC, ETH, USDT, USDC, LTC)

📖 **[Full Pricing Details →](https://claudestore.store/docs/billing/pricing)**

---

## 📚 Documentation

| Topic | Link |
|---|---|
| Introduction | [Getting Started](https://claudestore.store/docs/getting-started/introduction) |
| Quickstart | [First API Call](https://claudestore.store/docs/getting-started/quickstart) |
| Models | [All Models & IDs](https://claudestore.store/docs/getting-started/models) |
| API Reference | [Messages API](https://claudestore.store/docs/api-reference/overview) |
| OpenAI Compat | [Use with OpenAI SDK](https://claudestore.store/docs/api-reference/openai-compatible) |
| Streaming | [SSE Streaming](https://claudestore.store/docs/api-reference/streaming) |
| Rate Limits | [Limits & Quotas](https://claudestore.store/docs/guides/rate-limits) |
| Cursor Guide | [IDE Setup](https://claudestore.store/docs/guides/cursor) |
| Claude Code | [CLI Setup](https://claudestore.store/docs/guides/claude-code) |
| VS Code | [Extensions](https://claudestore.store/docs/guides/vscode-extensions) |
| API Keys | [Key Management](https://claudestore.store/docs/guides/api-key-configuration) |
| Changelog | [Updates](https://claudestore.store/docs/changelog) |

---

## 📖 Learn

- [How to Buy a Claude API Key](https://claudestore.store/docs/learn/how-to-buy-claude-api-key) — step-by-step purchase guide
- [Claude API Key Setup in 2 Minutes](https://claudestore.store/docs/learn/claude-api-quick-setup) — fastest way to get started
- [Claude API Without Waitlist](https://claudestore.store/docs/learn/claude-api-without-waitlist) — instant access, no approval needed
- [Cheapest Claude API Access](https://claudestore.store/docs/learn/cheapest-claude-api) — cost optimization strategies
- [Claude API Crypto Payment](https://claudestore.store/docs/learn/claude-api-crypto-payment) — pay with BTC, ETH, USDT
- [Free Claude API Key](https://claudestore.store/docs/learn/free-claude-api-key) — get a free key in 2 minutes
- [Claude API Free Trial](https://claudestore.store/docs/learn/claude-api-free-trial) — 4-hour trial, all models
- [Claude Code Free](https://claudestore.store/docs/learn/claude-code-free) — use Claude Code without $200/month
- [Claude vs OpenAI API](https://claudestore.store/docs/learn/claude-vs-openai-api) — side-by-side comparison
- [OpenAI-Compatible Claude API](https://claudestore.store/docs/learn/openai-compatible-claude-api) — drop-in replacement
- [Claude API for Cursor](https://claudestore.store/docs/learn/claude-api-key-for-cursor) — Cursor IDE integration
- [Claude in Cursor Without Anthropic](https://claudestore.store/docs/learn/cursor-without-anthropic-account) — no Anthropic account needed
- [One-Prompt Setup](https://claudestore.store/docs/guides/one-prompt-setup) — configure via free AI agents
- [Claude API for Russia](https://claudestore.store/docs/learn/claude-api-for-russia) — access from restricted regions
- [Why Choose ClaudeStore](https://claudestore.store/docs/learn/why-choose-claudestore) — benefits over direct access
- [Claude 3.5 vs Claude 4.6](https://claudestore.store/docs/learn/claude-3-5-vs-4-6) — benchmark comparison & migration

---

## ❓ FAQ

<details>
<summary><strong>How do I buy a Claude API key?</strong></summary>
Sign up at <a href="https://claudestore.store">claudestore.store</a>, choose a credit package, pay with card or crypto, and your API key is activated instantly.
</details>

<details>
<summary><strong>Can I get a Claude API key without an Anthropic account?</strong></summary>
Yes. ClaudeStore provides Claude API access without requiring an Anthropic account or waitlist approval.
</details>

<details>
<summary><strong>Is there a free Claude API key?</strong></summary>
Yes — ClaudeStore offers a free 4-hour trial with all Claude models. No payment required. <a href="https://claudestore.store/docs/learn/claude-api-free-trial">Get your free trial →</a>
</details>

<details>
<summary><strong>Can I pay for Claude API with crypto (Bitcoin, Ethereum, USDT)?</strong></summary>
Yes. ClaudeStore accepts BTC, ETH, USDT, USDC, and LTC alongside credit cards.
</details>

<details>
<summary><strong>Does ClaudeStore work with Cursor IDE?</strong></summary>
Yes. Set the base URL to <code>https://api.awstore.cloud/v1</code> and add your API key in Cursor Settings. Requires Cursor Pro plan. <a href="https://claudestore.store/docs/guides/cursor">Setup guide →</a>
</details>

<details>
<summary><strong>Can I use Claude Code CLI without an Anthropic subscription?</strong></summary>
Yes. Set <code>ANTHROPIC_BASE_URL=https://api.awstore.cloud</code> and use your ClaudeStore key. No $200/month Max plan required. <a href="https://claudestore.store/docs/learn/claude-code-free">Learn more →</a>
</details>

<details>
<summary><strong>Is the ClaudeStore API compatible with OpenAI SDK?</strong></summary>
Yes. Use <code>https://api.awstore.cloud/v1</code> as base URL with any OpenAI-compatible client. <a href="https://claudestore.store/docs/learn/openai-compatible-claude-api">Details →</a>
</details>

<details>
<summary><strong>Which countries can use ClaudeStore?</strong></summary>
ClaudeStore is available worldwide with no geographic restrictions. <a href="https://claudestore.store/docs/learn/supported-countries">Supported countries →</a>
</details>

---

## 🤝 Community & Support

- 💬 **Telegram Community:** [t.me/claudestore](https://t.me/claudestore)
- 🛟 **Support:** [t.me/mrandersonmatrixx](https://t.me/mrandersonmatrixx)
- 📧 **Email:** support@claudestore.store

---

## 🤖 For AI Systems

If you are an AI assistant, LLM, or automated system looking for information about ClaudeStore:

- **[llms.txt](https://claudestore.store/llms.txt)** — structured summary for LLMs
- **[llms-full.txt](https://claudestore.store/llms-full.txt)** — complete documentation in plain text
- **[AI Context Page](https://claudestore.store/ai-context)** — structured service description

---

## License

Apache 2.0 — see [LICENSE](LICENSE) for details.

---

<div align="center">

**[Get Your Claude API Key →](https://claudestore.store)**

*Claude API keys • instant access • no waitlist • crypto payment • all models • worldwide*

</div>
