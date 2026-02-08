# hexyl-marketplace

hexyl's personal Claude Code plugin marketplace.

## Usage

```
/plugin marketplace add hexylab/hexyl-marketplace
```

Then browse and install plugins:

```
/plugin install <plugin-name>@hexyl-marketplace
```

## Adding a Plugin

1. Create a plugin directory under `plugins/`:

```
plugins/my-plugin/
├── .claude-plugin/
│   └── plugin.json
├── skills/
│   └── my-skill/
│       └── SKILL.md
└── ...
```

2. Add an entry to `.claude-plugin/marketplace.json`:

```json
{
  "name": "my-plugin",
  "source": "./plugins/my-plugin",
  "description": "What the plugin does",
  "version": "1.0.0"
}
```
