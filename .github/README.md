# EBR Mod Scaffold Templates

Reusable content scaffolds for Earthborne Rangers mod creators.

## How Scaffolds Work

Scaffold templates live as branches in this repo (e.g., `map/lure-of-the-valley`, `set/the-valley`). Creators use `ebr include <type>/<name>` to stamp a scaffold into their mod as a one-shot copy.

- **No manifest tracking**: Scaffolds are copied content, not tracked as dependencies.
- **Placeholder substitution**: Paths like `Custom Campaigns/__MOD_NAME__/...` are substituted with the creator's mod name at include time.
- **No update path**: Once stamped, scaffolds are the creator's responsibility.