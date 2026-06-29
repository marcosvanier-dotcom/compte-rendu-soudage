# Générateur de Comptes Rendus

## Comme utiliser

1. Téléchargez le fichier [`ferramenta.html`](ferramenta.html).
2. Ouvrez-le directement dans votre navigateur (double-clic ou `Fichier > Ouvrir`).
3. Toutes les données sont sauvegardées localement dans le `localStorage` de votre navigateur — il n'y a pas de backend, pas de connexion, pas de serveur.

## Import par e-mail via IA (optionnel)

L'outil peut utiliser un fournisseur d'IA (Anthropic, OpenAI ou Gemini) pour aider à importer le contenu des e-mails. Pour l'activer :

1. Cliquez sur **⚙️ Configurer** dans l'outil.
2. Renseignez votre propre clé API du fournisseur choisi.
3. La clé est stockée uniquement dans le `localStorage` de votre navigateur — elle n'est jamais envoyée ailleurs qu'au fournisseur d'IA choisi, directement depuis votre navigateur.

> ⚠️ L'import de fichiers `.pst` est désactivé dans cette version (nécessiterait un backend pour traiter le format binaire).

## Fonctionnalités principales

- **Gestion par rubriques** : organisez les sujets en rubriques personnalisables (libellé, emoji, couleur), avec sous-lignes par responsable, tags, pièce/affaire, échéance et commentaire par élément.
- **Suivi visuel (Kanban)** : vue par état ou par priorité, avec navigation directe vers l'élément d'origine.
- **Résumé par responsable** : vue accordéon listant les sujets de chaque responsable, avec accès direct au sujet en un clic.
- **Calendrier** des échéances, **histogramme** de progression et **historique** des sessions précédentes.
- **Tickets** : suivi des incidents, non-conformités et demandes, avec une fiche dédiée « Situation dégradée (équipement) » imprimable/exportable (photos compressées automatiquement, fichier LOG joint).
- **Exports** : Word, PDF, Excel, CSV, e-mail, JSON — pour le compte rendu complet, le suivi visuel, le résumé par responsable et les tickets.
- **Import IA par e-mail** (voir section dédiée plus haut) avec licence Pro optionnelle.

## Protection anticopie

Cette version inclut quelques protections basiques côté navigateur pour limiter la copie/extraction du contenu :

- Clic droit, sélection de texte et glisser-déposer désactivés hors des champs éditables.
- Raccourcis `Ctrl+U` (voir la source), `Ctrl+P` (impression directe) et `F12`/`Ctrl+Shift+I`/`Ctrl+Shift+J` (outils de développement) bloqués.
- Filigrane discret (© Marcos Vanier) affiché en bas de l'écran.

> ⚠️ Ces protections sont volontairement légères et n'empêchent pas un utilisateur technique déterminé (le code source est entièrement visible côté client, comme pour toute application web). Elles dissuadent la copie occasionnelle, elles ne remplacent pas une protection juridique ou contractuelle.

## Confidentialité

- Aucune donnée n'est envoyée à un serveur tiers, sauf lors d'un appel explicite à l'API d'un fournisseur d'IA que vous avez configuré vous-même.
- Aucun compte, aucune authentification requise.
