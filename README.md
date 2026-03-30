# OpenCLI-Hub

The community plugin registry for [OpenCLI](https://github.com/jackwener/opencli) — a universal CLI hub that turns websites, Electron apps, and local tools into command-line interfaces.

## How to Install

```bash
opencli plugin install github:<user>/<repo>
```

For more details on plugin development and installation, see the [Plugin Guide](https://github.com/jackwener/opencli/blob/main/docs/guide/plugins.md).

---

## Plugins

| Plugin | Description | Author | Type | Install |
|--------|-------------|--------|------|---------|
| [github-trending](https://github.com/ByteYue/opencli-plugin-github-trending) | GitHub Trending repositories | [@ByteYue](https://github.com/ByteYue) | YAML | `opencli plugin install github:ByteYue/opencli-plugin-github-trending` |
| [hot-digest](https://github.com/ByteYue/opencli-plugin-hot-digest) | Multi-platform trending content aggregator | [@ByteYue](https://github.com/ByteYue) | TypeScript | `opencli plugin install github:ByteYue/opencli-plugin-hot-digest` |
| [juejin](https://github.com/Astro-Han/opencli-plugin-juejin) | 稀土掘金 (Juejin) hot articles | [@Astro-Han](https://github.com/Astro-Han) | YAML | `opencli plugin install github:Astro-Han/opencli-plugin-juejin` |

---

## Contributing

Want to add your plugin? Submit a PR to add a row to the table above!

### Plugin Formats

OpenCLI supports three plugin formats:

- **YAML** — Declarative data pipelines (no build required)
- **TypeScript** — Browser runtime injections (compiled via esbuild)
- **JavaScript** — External CLI passthroughs

### Monorepo Support

A single repository can contain multiple plugins via `opencli-plugin.json`:

```json
{
  "plugins": {
    "plugin-name": {
      "path": "packages/plugin-name",
      "description": "Description",
      "version": "1.0.0"
    }
  }
}
```

---

## CLI Ecosystem

Other CLI tools in the ecosystem that share a similar vision — unifying platform capabilities into terminal-friendly interfaces for both humans and AI agents.

| Project | Description | Author |
|---------|-------------|--------|
| [dingtalk-workspace-cli](https://github.com/DingTalk-Real-AI/dingtalk-workspace-cli) | DingTalk official cross-platform CLI — unifies DingTalk's full suite of product capabilities, designed for both human users and AI agents | [DingTalk-Real-AI](https://github.com/DingTalk-Real-AI) |
| [wecom-cli](https://github.com/WecomTeam/wecom-cli) | 企业微信开放平台命令行工具 — 让人类和 AI Agent 都能在终端中操作企业微信 | [WecomTeam](https://github.com/WecomTeam) |

---

## About OpenCLI

OpenCLI provides 68+ built-in adapters covering social media, finance, developer tools, AI platforms, and more. Community plugins extend its capabilities even further.

- [OpenCLI Repository](https://github.com/jackwener/opencli)
- [Plugin Development Guide](https://github.com/jackwener/opencli/blob/main/docs/guide/plugins.md)
