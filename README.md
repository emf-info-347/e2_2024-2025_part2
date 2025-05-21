# Évaluation : Conteneurisation d'une application Etherpad

| Libellé | Description |
| --- | --- |
| Durée | 120 minutes |
| Sujet | Conteneurisation d'une application Etherpad |
| Modalité | Travail pratique individuel sur poste informatique avec Docker installé. Accès à internet. Utilisation interdite de Teams |

## Objectifs de l'évaluation 
- Comprendre et expliquer les technologies de conteneurs
- Déterminer les composants nécessaires pour la virtualisation
- Utiliser correctement les frameworks et outils de conteneurisation
- Virtualiser une application simple selon les spécifications


## Contexte

Vous travaillez comme développeur junior dans une entreprise qui souhaite moderniser son infrastructure. Votre équipe a décidé d'utiliser Docker pour déployer ses applications. Comme première expérience, on vous demande de conteneuriser l'application Etherpad, un éditeur de texte collaboratif en temps réel.
![Aperçu de l'application Etherpad](https://etherpad.org/_next/static/media/etherpad_demo.9bd22127.gif)

## Travail à réaliser

Dans un premier temps, vous devrez analyser l'application [Etherpad](https://etherpad.org/) et documenter ses prérequis techniques, notamment l'utilisation de Node.js, les dépendances nécessaires et les ports requis pour son fonctionnement. Cette analyse préliminaire est essentielle pour la suite du travail.

Ensuite, vous créerez un fichier Dockerfile qui contiendra toutes les instructions nécessaires pour construire l'image Docker. Cela inclut le choix de l'image de base appropriée, l'installation des dépendances requises, la configuration des variables d'environnement essentielles, l'exposition du port correct pour l'accès à l'application, et les commandes nécessaires au démarrage de l'application. Pour l'installation d'Etherpad vous allez récupérer la dernière version dans le repository Github proposé par Eherpad.

Une partie importante du travail consistera à modifier le fichier de configuration settings.json de l'application. Vous devrez y apporter plusieurs modifications : changer le titre de l'application, configurer le port d'écoute, et activer ou désactiver certaines fonctionnalités selon les besoins ci-dessous :

- **Titre de l'application** : Bloc-notes de *votre prénom* (Ex: Bloc-notes de Lucas)
- **Favicon** : Le favicon de l'application doit se baser sur le fichier suivant [347.ico](/settings/347.ico).
- **Texte de démarrage** : Bienvenue sur mon bloc-notes du module 347 !
- **Port** : 9009
- **Type de base de données** : Utilisation de la version simple avec une base de données légères *Dirty*

La phase suivante concernera la construction de l'image Docker et le test du déploiement. Vous utiliserez les commandes Docker appropriées pour construire l'image, vérifier sa création correcte, lancer le conteneur avec les paramètres adaptés, et tester l'accès à l'application via le navigateur web.

Tout au long du processus, vous devrez documenter minutieusement votre travail, incluant les commandes utilisées, les problèmes rencontrés et leurs solutions, ainsi que les choix techniques que vous aurez effectués.

## Livrables attendus

À la fin de l'évaluation, vous devrez fournir :
- le fichier Dockerfile commenté à mettre dans le répertoire [settings](/settings/), 
- le fichier settings.json modifié à mettre dans le répertoire [settings](/settings/),
- une documentation technique complète du déploiement au format markdown à compléter dans le document [README](/docs/README.md),
- des copies d'écran commentées dans le document se trouvant le répertoire demo [README](/demo/README.md)

La qualité de la documentation et la clarté des explications seront particulièrement évaluées.

## Aide pour la rédaction de markdown
- [CheatSheat Markdown](markdown.md)
