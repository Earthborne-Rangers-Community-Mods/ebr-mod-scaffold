# Contributing to ebr-mod-scaffold

This repository holds reusable scaffolding templates for Earthborne Rangers mod
creators. Each template lives as a branch (e.g., `map/lure-of-the-valley`,
`set/the-valley`). Contributions of new templates are welcome.

## How Scaffolds Work

Mod creators use `ebr scaffold <type>/<name>` to stamp a template into their
mod as a one-shot copy. Once stamped, the scaffold belongs to the creator -
there is no update path back to this repo.

Templates use `__MOD_NAME__` as a placeholder in file paths. The tool
substitutes the creator's mod name at stamp time.

## Proposing a New Scaffold

Official scaffolds (`map/*` and `set/*` branches) are maintained by the project
team. Community-contributed scaffolds live under the `community/` prefix.

### Branch Naming Convention

| Prefix | Maintained by | Access |
|---|---|---|
| `map/<name>` | Maintainers only | Protected (maintainer push only) |
| `set/<name>` | Maintainers only | Protected (maintainer push only) |
| `community/map/<name>` | Community contributors | Open (anyone can push) |
| `community/set/<name>` | Community contributors | Open (anyone can push) |

### How to Contribute a Scaffold

Push a branch following the naming convention:

- `community/map/<name>` for map location scaffolds
- `community/set/<name>` for path set (card set) scaffolds

No approval needed. Maintainers may remove branches that violate the
[Code of Conduct](CODE_OF_CONDUCT.md) or the content rules below.

Creators stamp community scaffolds the same way as official ones:
`ebr scaffold community/map/<name>`.

### Branch Content Rules

Scaffold branches contain **only the stamped-out content tree**:

- Use `__MOD_NAME__` in paths where the mod name should appear
- Include only `.md`, `.css`, `.json`, image files, and `.txt`
- Do **not** include `.obsidian/`, `About this Mod.md`, `ebr-symbols.css`, or
  `ebr-mod.json` - these come from the mod's shell ancestry
- Keep content minimal - stubs and structure, not complete narratives

### Updating Existing Scaffolds

Scaffolds are one-shot copies. Updating a scaffold branch only affects future
stamps - existing mods that already stamped the old version are unaffected.
This means updates are safe to merge without worrying about breaking existing
mods.

## What We Accept

- New scaffolds for common custom content

## What We Do Not Accept

- Narrative content (scaffolds are structure, not story)
- Scaffolds that duplicate existing templates without meaningful difference

## Questions

Open a GitHub issue for questions about scaffold structure or the contribution
process.
