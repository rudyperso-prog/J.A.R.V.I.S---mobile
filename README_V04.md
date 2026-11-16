# JARVIS Mobile v0.4 — Holographic Voice

## Nouveautés
- Interface cyan à anneaux holographiques continus et graduations techniques, inspirée de la référence fournie.
- Centre J.A.R.V.I.S. et spectre vocal animé sur Canvas 2D, sans bibliothèque externe.
- Analyse de fréquence du microphone en mode écoute **si le navigateur autorise getUserMedia**. L’analyse audio peut être indisponible lorsque la reconnaissance vocale iOS occupe déjà le micro.
- Animation de parole de synthèse **approximative** : iOS speechSynthesis ne fournit pas les échantillons PCM. Aucune fausse promesse de synchronisation parfaite.
- Conservation des huit modules Control v0.3 et de leurs réglages en localStorage. Les accès Apple/Google ne sont pas magiquement connectés.

## Installation GitHub Pages
Décompressez l'archive, téléversez **tous les fichiers** à la racine du dépôt GitHub Pages existant, remplacez les anciennes versions et attendez le déploiement. Rechargez l'application dans Safari. En cas d'ancienne interface en cache, fermez la PWA, rechargez la page Safari et réouvrez-la.

## Limitations
Pas d'API OpenAI incluse ; commandes locales uniquement. Aucune suppression de photos, e-mails ou contacts sans connecteur autorisé. Aucun clonage de voix de film.
