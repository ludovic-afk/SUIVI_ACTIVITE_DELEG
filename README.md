# Suivi des actions associatives

Application statique GitHub Pages. La page HTML est l’outil de saisie. Excel est uniquement le format d’export.

## Installation GitHub
1. Créer un nouveau repository GitHub, par exemple `suivi-actions-associatives`.
2. Déposer tous les fichiers de ce dossier à la racine de la branche `main`.
3. Ouvrir **Settings > Pages**.
4. Choisir **Deploy from a branch**, puis `main` et `/ (root)`.
5. Enregistrer et ouvrir l’adresse publiée.

## Référentiels
- Modifier `delegations.js` pour ajouter ou désactiver une délégation.
- Modifier `actions.js` pour ajouter une activité.
- Seul `T1SENSI_SCOLAIR` a été fourni. Les autres codes sont laissés vides et doivent être validés. Ne pas inventer de code.

## Tests
Ouvrir `tests.html`, lancer les tests, puis effectuer les tests manuels indiqués.

## Export et sauvegarde
- **Exporter** génère un classeur contenant la feuille `import` avec les 26 colonnes officielles.
- **Sauvegarder mes données** génère un JSON transférable.
- **Restaurer une sauvegarde** accepte uniquement ce JSON, jamais le tableau Excel métier.

## Limites et confidentialité
`localStorage` est propre au navigateur et à l’appareil. Ce n’est pas une base partagée. Une suppression des données du navigateur peut supprimer les saisies. Effectuer des sauvegardes JSON régulières. Ne pas saisir de données personnelles inutiles. Valider l’hébergement et la visibilité du repository selon les règles de la DSI.

SheetJS est chargé depuis un CDN. Pour un fonctionnement hors connexion garanti dès la première ouverture, télécharger une version validée de `xlsx.full.min.js`, la placer localement et modifier les balises `script`.

Une centralisation dans Microsoft Lists, SharePoint, Power Automate ou une base nécessite une authentification, des autorisations et un service complémentaire. Une page GitHub Pages statique ne peut pas alimenter seule un fichier partagé.
