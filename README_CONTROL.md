# JARVIS Control v0.3 — prototype honnête

Ce projet est une PWA statique et privée côté navigateur (mais le dépôt GitHub Pages public expose son code). Les 8 modules sont configurables sur l’écran Paramètres ; par défaut « Actions avec confirmation ». Les préférences sont enregistrées localement. Les autorisations système réelles ne sont **pas** accordées par ces sélecteurs.

## Disponible maintenant
- Interface Control pour les 8 services, journal local et confirmation avant ouverture de raccourcis.
- Configuration de noms de raccourcis Apple existants, via `shortcuts://run-shortcut?name=...` (fonctionnement à tester sur iOS ; les raccourcis doivent être créés dans l’app Raccourcis).
- Import ponctuel d’images via sélecteur de fichiers. Aucune suppression ni transfert.
- Commandes textuelles ciblées ouvrant un raccourci Apple configuré ; les services Google indiquent honnêtement « Non connecté ».

## À connecter ultérieurement
- Apple Photos / Calendrier / Contacts / Mail : créer les raccourcis Apple compatibles avec les actions réellement disponibles sur l’iPhone ; aucune lecture directe des données privées par la PWA.
- Google Calendar API / People API / Gmail API : projet Google Cloud, OAuth avec consentement et scopes minimaux, implémentation sécurisée des jetons. Gmail peut nécessiter des contraintes supplémentaires selon les scopes.
- Google Photos : Google Photos Picker API pour les photos choisies ; pas de scan global automatique de la bibliothèque.
- Pas de moteur ChatGPT intégré : ChatGPT Plus n’inclut pas l’API.

## Publication
Décompresser le ZIP puis déposer les fichiers contenus dans le dossier à la racine du dépôt GitHub Pages. Le service worker utilise des chemins relatifs. Après publication, vider le cache ou relancer la PWA si l’ancienne version persiste. Ne jamais publier de mot de passe ou de clé OAuth secrète dans le dépôt.
