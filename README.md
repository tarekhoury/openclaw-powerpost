# PowerPost Skill for OpenClaw

Generate social media content and publish it from your OpenClaw agent.

[![Version](https://img.shields.io/badge/version-1.0.0-blue)](https://github.com/tarekhoury/openclaw-powerpost)
[![License](https://img.shields.io/badge/license-MIT-green)](LICENSE)

---

## What It Does

PowerPost combines **content generation** with **direct publishing**. One command can research a topic, write captions tailored to each platform, generate images, and post to your connected accounts.

**Platforms supported:** Instagram, TikTok, X (Twitter), YouTube, Facebook, LinkedIn, and more as they're added.

**Key features:**

| Feature | Description |
|---|---|
| AI captions | Content tailored to each platform |
| Image generation | AI-generated visuals for your posts |
| Deep research mode | Extended research for higher-quality content |
| Custom writing styles | Match content to your brand voice |
| Draft review workflow | Review and approve before publishing |

---

## Prerequisites

- A PowerPost account with credits — [powerpost.ai](https://powerpost.ai)
- An API key — **Settings → API**
- Your Workspace ID — **Settings → Workspaces**
- Connected social accounts for publishing — **Settings → Connections**

---

## Installation

```bash
# Install from ClawHub
openclaw skill install powerpost

# Or install manually
git clone https://github.com/tarekhoury/openclaw-powerpost.git ~/.openclaw/skills/powerpost
```

---

## Configuration

```bash
# Set your credentials
openclaw config set skills.powerpost.apiKey "pp_live_sk_YOUR_KEY"
openclaw config set skills.powerpost.workspaceId "YOUR_WORKSPACE_ID"

# Or use environment variables
export POWERPOST_API_KEY="pp_live_sk_YOUR_KEY"
export POWERPOST_WORKSPACE_ID="YOUR_WORKSPACE_ID"
```

---

## Usage Examples

Say these (or similar) to your OpenClaw agent:

```
"Post about our new product launch on Instagram and TikTok"

"Write captions about AI trends for all platforms"

"Generate an image for my last post"

"Create a deep research post about sustainable fashion"

"Check my PowerPost credits"

"Upload this image and write captions about it"

"Create a draft post about our company update but don't publish yet"
```

---

## API Key Types

| Key Type | Permissions | When to Use |
|---|---|---|
| `read_write` | Generate, publish, manage posts | Production agents that publish content |
| `read_draft` | Generate and save drafts only, read data | Agents that need human approval before publishing |

Use `read_draft` keys when you want a human-in-the-loop review step. Use `read_write` keys for fully automated workflows.

---

## Supported Platforms and Post Types

| Platform | Post Types |
|---|---|
| Instagram | Feed post, Reel, Story |
| TikTok | Video, Photos |
| X (Twitter) | Post (tweet) |
| YouTube | Video, Short |
| Facebook | Post, Reel, Story |
| LinkedIn | Post (personal profile) |

---

## Credit Costs

Content generation, image generation, and deep research each consume credits. Credit costs vary by operation and model used. See the [full pricing page](https://powerpost.ai/docs) for details.

---

## Links

- [API Documentation](https://powerpost.ai/docs)
- [Dashboard](https://powerpost.ai)
- [Support](https://powerpost.ai/support)
