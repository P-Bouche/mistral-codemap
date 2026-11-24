# mistral-codemap — portage Vibe Code

Cartographie de codebase pour Vibe Code : architecture, dépendances, mindmaps, guide d'onboarding (port de hxxnn/mistral-codemap).

Portage des skills de [mistral-codemap](https://github.com/hxxnn/mistral-codemap) (archive de la branche `main`, 24 novembre 2026) vers le format Agent Skills utilisé par Vibe Code. 8 skills.

## Skills portées

- `architecture-overview` : Use when the user wants an architecture overview, system structure, "how is this project organized", or C4-...
- `mistral-codemap-refresh` : Use when code has changed since mistral-codemap files were generated and the user wants them brought up to date: "r...
- `dependency-graph` : Use when the user wants module or file dependencies, an import graph, "what depends on what", or circular d...
- `design-doc` : Use when the user wants an explanation document of how the project is built: design overview, key design ch...
- `mindmap` : Use when the user wants a project structure tree, a "map" of features and files, or the big picture of a pr...
- `present` : Use when the user wants a presentation outline or slide structure that explains THIS project's codebase to ...
- `relation-map` : Use when the user wants to see how the project's files relate to each other at a glance — a full-screen fil...
- `sequence-flow` : Use when the user wants to see how a request, command or feature actually runs: call order, "what happens w...

## Installation

**Option A — comme plugin (expérimental)** : copier ce dossier entier dans `~/.vibe/plugins/mistral-codemap/`.

**Option B — comme skills individuelles** : copier chaque sous-dossier de `skills/` (sauf `_shared`, qui est un dossier de support) dans `~/.vibe/skills/` ou `~/.agents/skills/` (niveau utilisateur), ou `./.vibe/skills/` / `./.agents/skills/` (niveau projet). Dans une session Vibe Code, `/reload` les prend en compte ; `/skills` les liste.

**Option C — depuis Claude Code** : si les skills sont déjà installées côté Claude Code, `/vibe:import` dans Vibe Code reprend instructions, skills, subagents, hooks et serveurs MCP.

Détail des adaptations : voir `PORT-NOTES.md`.

## Licence

MIT (fichier LICENSE repris du dépôt d'origine)
