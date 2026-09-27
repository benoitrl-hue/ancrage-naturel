# CLAUDE.md — Guide pour assistants IA

## Aperçu du projet

**Ancrage Naturel** est un dépôt de planification de contenu et de documentation pour **Renaissance Somatique**, une entreprise de coaching somatique destinée aux personnes hypersensibles (HSP). Ce n'est pas un projet logiciel — il contient uniquement des fichiers Markdown et texte, rédigés à la main par la propriétaire pour préparer sa communication (calendrier éditorial, scripts vidéo, brainstorm).

- **Propriétaire :** benoitrl-hue (Benoit R.L.)
- **Langue :** Tout le contenu est rédigé en français
- **Site web :** ancragenaturel.com
- **Branche principale :** `main`

## Structure du dépôt

```
ancrage-naturel/
├── README.md                      # Présentation du projet et de l'entreprise
├── CLAUDE.md                      # Ce fichier — guide pour les assistants IA
├── contenus-reseaux-sociaux.md    # Calendrier éditorial et templates de posts Facebook
├── scripts-videos-facebook.md     # Script vidéo de lancement (90 secondes) + guide de présence
├── idees.md                       # Liste d'idées et brainstorm
└── note.txt                       # Fichier de test Git (sans rapport avec le contenu éditorial)
```

Aucun sous-dossier, aucun asset binaire (image, audio, vidéo) n'est versionné : tout le travail créatif (vidéos, visuels) est produit hors dépôt, seul le texte de préparation vit ici.

## Description des fichiers

| Fichier | Contenu | Statut |
|---------|---------|--------|
| `contenus-reseaux-sociaux.md` | Calendrier éditorial pour les semaines du 10 au 23 février 2026, deux posts rédigés en entier (mercredi 12 — scan corporel express, vendredi 14 — mythe hypersensibilité/fragilité), une banque d'idées de thèmes récurrents, et une section « Templates de posts » | 🚧 En cours — seul le Template #1 (Vulnérabilité) est amorcé ; les templates #2 à #5 (éducatif, pratique, inspirant, engagement) restent à rédiger, et le post du lundi 17 février est encore vide |
| `scripts-videos-facebook.md` | Script complet de la vidéo de lancement « Reviens habiter ton corps » (découpage minuté sur 90 s : hook, empathie, vision, appel à l'action), notes de production, et un « Guide de présence » | 🚧 En cours — le guide de présence s'interrompt en plein rituel d'ancrage (dernière ligne incomplète) |
| `idees.md` | Liste de 4 idées : vidéos courtes, présence sur les groupes HSP, sessions découverte, documentation de la méthodologie | ✅ Complet mais très court — une puce vide en fin de fichier |
| `note.txt` | Fichier de test créé lors de l'apprentissage de Git (« commit hello ») | ✅ N'a pas vocation éditoriale, ne pas y ajouter de contenu marketing |

**Note pour les assistants :** deux fichiers (`contenus-reseaux-sociaux.md`, `scripts-videos-facebook.md`) se terminent en plein milieu d'une section. Ne pas supposer qu'ils sont finis — vérifier la dernière section avant d'ajouter du contenu, pour éviter de dupliquer un en-tête déjà présent ou d'écraser un brouillon en cours.

## Conventions

- **Langue :** Tout le contenu doit être écrit en français
- **Format :** Markdown (.md) pour tout le contenu structuré
- **Messages de commit :** Rédigés en français, descriptifs (ex. « Ajout post mercredi 12 fev. - Scan corporel express »)
- **Branche principale :** `main` — le développement se fait sur des branches de travail (ex. `claude/...`) fusionnées via pull request
- **Granularité des commits :** un commit correspond en général à un seul élément de contenu (un post, un script, une mise à jour de calendrier), pas à plusieurs changements mélangés

## Sécurité et confidentialité

- Ce dépôt est destiné à du contenu marketing **public** (calendrier éditorial, scripts, idées). Il ne doit jamais contenir de données personnelles sensibles : dossiers médicaux, relevés bancaires ou financiers, pièces d'identité, coordonnées ou informations de clients/tiers.
- Si un fichier ou un extrait de ce type est proposé pour ajout (même par erreur, par exemple via une pièce jointe de conversation), un assistant IA doit s'abstenir de l'intégrer au dépôt et le signaler plutôt que de le committer.
- Si une telle donnée a déjà été poussée par erreur, un simple nouveau commit de suppression ne suffit pas : il faut purger l'historique Git (ou recréer l'historique) avant de considérer l'incident clos.

## Contexte métier

- **Public cible :** Personnes hypersensibles (HSP) qui veulent mieux habiter leur corps
- **Offre principale :** Sessions découverte en coaching somatique
- **Positionnement :** « Transformer l'hypersensibilité en superpouvoirs ancrés »
- **Plateforme prioritaire :** Facebook (posts et vidéos)
- **Ton éditorial :** Authentique, chaleureux, vulnérable sans être dramatique, ancré dans l'expérience corporelle

## Pile technique

Aucune — ce dépôt ne contient pas de code. Pas de dépendances, pas de build, pas de tests. Uniquement des fichiers texte et Markdown versionnés avec Git.

## Pour contribuer

Lors de l'ajout ou la modification de contenu :
1. Respecter le français dans tout le contenu et les commits
2. Suivre les templates existants dans `contenus-reseaux-sociaux.md` pour les nouveaux posts, en complétant les templates manquants (#2 à #5) plutôt qu'en créant une structure parallèle
3. Garder un ton cohérent avec le positionnement Renaissance Somatique
4. Utiliser le format Markdown avec des titres hiérarchiques clairs
5. Avant de « terminer » une section laissée incomplète (ex. le guide de présence), vérifier auprès de la propriétaire si le texte existant reflète son intention, car le ton très personnel (vécu, voix propre) est difficile à deviner
6. Ne jamais ajouter de fichier contenant des données personnelles sensibles (voir « Sécurité et confidentialité »)
