# le-lien-transforme.fr

Interface web statique pour la consultation et le téléchargement du livret numérique.

## Spécifications
- **Hébergement :** GitHub Pages
- **Domaine :** le-lien-transforme.fr
- **Technologies :** HTML5, CSS3, JavaScript (Vanilla)

## Architecture
Le projet utilise une architecture sans serveur (serverless) :
- Le document PDF est servi directement par l'infrastructure GitHub pour garantir une haute disponibilité.
- Le suivi des téléchargements est assuré par une intégration asynchrone (`navigator.sendBeacon`) pour ne pas impacter les performances ou l'expérience utilisateur.

## Maintenance
Le déploiement est automatisé via la branche principale (`main`). Toute modification du fichier `index.html` est répercutée en production après validation des tests de déploiement GitHub.