# EBR Mod Scaffold Templates

Reusable content scaffolds (blank stub files) for Earthborne Rangers mod creators.

## How Scaffolds Work

Scaffold templates live as branches in this repo (e.g., `map/lure-of-the-valley`, `set/the-valley`). Creators use `ebr include <type>/<name>` to stamp a scaffold into their mod as a one-shot copy.

Scaffolds are copied content, not tracked as dependencies. This means there is no update path like there is for including base mods.

Paths like `Custom Campaigns/__MOD_NAME__/...` are substituted with the creator's mod name at include time.
