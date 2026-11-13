<!-- Copyright (c) 2026 Manicode Worldwide, Inc. Proprietary and confidential. -->

# Manicode Claude Code Plugin Marketplace

The `manicode` [Claude Code plugin marketplace](https://code.claude.com/docs/en/plugin-marketplaces). It lists Manicode's plugins for customers: today, `forge`.

> [!IMPORTANT]
> This repo is private for now. Adding the marketplace needs GitHub access to the `manicode` org.

## Install forge

```bash
claude plugin marketplace add manicode/external-claude-code-plugins
claude plugin install forge@manicode
```

Set the API key as described in the [forge plugin README](https://github.com/manicode/forge-claude-code-plugin#api-key).

## Add a plugin

1. Publish the plugin to its own repo under `manicode`.
2. Add an entry to `.claude-plugin/marketplace.json` with a `github` source pointing at that repo.
3. Run `claude plugin validate . --strict`.
