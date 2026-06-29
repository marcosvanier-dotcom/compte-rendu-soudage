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

Cette version embarque plusieurs protections côté navigateur destinées à dissuader la copie ou l'extraction occasionnelle du contenu de l'outil :

- **Clic droit désactivé** partout, sauf dans les champs de saisie (formulaires, zones de texte) où il reste nécessaire pour travailler normalement.
- **Sélection de texte bloquée** en dehors des champs éditables — impossible de sélectionner/copier l'interface elle-même.
- **Glisser-déposer désactivé**, sauf pour les usages internes autorisés (ex. réorganisation des boutons de la barre d'outils, déplacement d'éléments).
- **Raccourcis clavier bloqués** :
  - `Ctrl+U` — affichage du code source de la page.
  - `Ctrl+P` / `Cmd+P` — impression directe (sauf via les boutons d'export PDF prévus dans l'outil).
  - `F12`, `Ctrl+Shift+I`, `Ctrl+Shift+J` — ouverture des outils de développement du navigateur.
- **Menu contextuel du navigateur** (clic droit natif) entièrement supprimé hors zones éditables.
- **Filigrane discret** (© Marcos Vanier) affiché en permanence en bas à droite de l'écran, visible sur toute capture d'écran.

> ⚠️ **Limites à connaître :** ces protections s'exécutent entièrement côté client en JavaScript — comme pour toute application web, le code source est techniquement visible et contournable par un utilisateur déterminé (mode sans script, outils externes, etc.). Elles ne remplacent ni un contrat de licence, ni une protection juridique, ni un mécanisme serveur. Leur rôle est de dissuader la copie occasionnelle et non technique, pas d'empêcher un contournement délibéré.

## Confidentialité

- Aucune donnée n'est envoyée à un serveur tiers, sauf lors d'un appel explicite à l'API d'un fournisseur d'IA que vous avez configuré vous-même.
- Aucun compte, aucune authentification requise.
