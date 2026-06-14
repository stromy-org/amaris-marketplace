# Amaris Consulting Marketplace

Claude Code plugin marketplace for Amaris Consulting.

## Install

```bash
# Add the marketplace (one-time)
/plugin marketplace add stromy-org/amaris-marketplace

# Install the plugin
/plugin install amaris-consulting
```

## Update

```bash
/plugin update amaris-consulting
```

## Included plugins

| Plugin | Description |
|--------|-------------|
| `amaris-consulting` | Branded deliverables and brand tools for Amaris Consulting |

**Skills**: pdf, pptx, pptx-hd (HD), xlsx, docx, diagram, mermaid, brand-builder, brand-artifact-builder, brand-intelligence, website-builder

**Prerequisites**: Claude Code v2.1.49+, Node.js 18+, Python 3.11+ with uv

## Troubleshooting

| Problem | Fix |
|---------|-----|
| "Failed to install plugin" with `Permission denied (publickey)` | Refresh the marketplace and confirm the plugin source is the explicit `https://github.com/stromy-org/amaris-plugin.git` URL |
| Other installation errors | Check `~/Library/Logs/Claude/main.log` for the underlying clone or manifest error |

## Source format

The marketplace uses an explicit HTTPS clone URL ending in `.git`. Anthropic supports the `github` shorthand, but Claude Code can resolve it to SSH and fail on machines without a configured GitHub SSH key.
