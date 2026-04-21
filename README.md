---
type: meta
title: LoreWeave Test Vault
summary: Fixture vault for LoreWeave integration tests. Thirty notes across six types, linked into a connected graph.
schema_version: 1
---

# LoreWeave Test Vault

Sample [Obsidian](https://obsidian.md) vault used to exercise the
[LoreWeave](https://github.com/tfassbender/LoreWeave) REST API end-to-end.
It seeds a small sci-fi frontier setting — two rival factions (Outer / Inner Union),
a smuggler network, a mystical church, and a handful of unexplained events around
[[karsis-station]] on the Rim — and is organized into characters, factions, locations,
events, items, and rules subdirectories. Use it to exercise searches, graph traversal,
and the validation surfaces. #vault/meta

## Using this vault

Point a running LoreWeave instance at this repo by setting
`loreweave.vault.remote` to its clone URL (HTTPS or SSH). The server will clone it
into its local working directory on boot and pull on the configured sync interval.
See [LoreWeave's main README](https://github.com/tfassbender/LoreWeave) for details.
