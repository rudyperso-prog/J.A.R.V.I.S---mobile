# JARVIS Mobile 0.1

PWA statique pour iPhone, sans serveur applicatif ni clé API.

## Publication gratuite (GitHub Pages)
1. Créez un dépôt GitHub public, par exemple `jarvis-mobile`.
2. Téléversez **le contenu** de ce dossier à la racine du dépôt.
3. Dans Settings > Pages, choisissez Deploy from a branch, branche main, dossier /(root), puis Save.
4. Ouvrez l'URL HTTPS fournie par GitHub Pages dans Safari sur iPhone.
5. Dans Safari, Partager > Sur l'écran d'accueil > Ajouter.

Alternative : Netlify Drop permet de déposer le dossier sur un hébergement HTTPS, selon les modalités du service.

## Fonctionnalités
- Interface responsive avec cercle holographique animé.
- Synthèse vocale via Web Speech API, selon voix disponibles sur l'appareil.
- Reconnaissance vocale expérimentale : dépend du support navigateur/iOS, du réseau et des autorisations.
- Commandes locales (heure, tâches, liens), stockage des tâches local.
- Service worker pour mise en cache des fichiers de l'interface ; certains services externes et la reconnaissance vocale peuvent nécessiter Internet.
- Aucune connexion à ChatGPT, au PC Windows ou à la domotique pour le moment.

## Limites de sécurité
Cette version ne comporte aucun compte utilisateur, aucune authentification distante, aucun contrôle système et aucune connexion aux caméras. Évitez de saisir des secrets dans le champ de commandes. Le site statique est public si hébergé publiquement. Le micro ne s'active que sur action utilisateur. Il n'y a pas d'écoute permanente du mot-clé Jarvis sur iOS.
