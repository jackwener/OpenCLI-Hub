# OpenCLI Plugin Hub

A curated list of community plugins for [OpenCLI](https://github.com/jackwener/opencli).

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
