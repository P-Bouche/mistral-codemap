# Notes de portage — mistral-codemap

Date du portage : 24 novembre 2026. Source : https://github.com/hxxnn/mistral-codemap (branche main).

## Adaptations effectuées

- Frontmatter `SKILL.md` conservé (Agent Skills standard) et validé : `name` en slug kebab-case, `description` <= 1024 caractères.
- Le dossier `skills/_shared/` (règles communes, template HTML) est conservé tel quel : les skills y font référence par chemin relatif `../_shared/`.

## Éléments non portés automatiquement

- Hooks et événements de session spécifiques au harnais Claude Code.
- Manifestes de marketplace (`/plugin marketplace add ...`) : Vibe Code découvre les plugins autrement (dossier `~/.vibe/plugins/` + `plugin.json`).

## Licence du contenu source

MIT (fichier LICENSE repris du dépôt d'origine)
