# Mon travail au sein de l'entreprise DM Web

## Présentation de l'entreprise

### La structure

DM Web est une entreprise de développement web situé à Lons-le-Saunier, elle compte:

- Le patron, développeur Senior qui supervise et s'occupe à la fois du marketing et du développement
- Un développeur Junior full-stack
- Un responsable Marketing, qui s'occupait du SEO principalement, et du lancement de la plateforme *WPSupport*
- Une secrétaire, pour la gestion et les factures 

### Les services de l'entreprise

DM Web propose la mise en place de solutions web, adaptées à la demande des clients, notamment sous *WordPress*, elle en assure le suivi et la maintenance, et travaille à améliorer le référencement web de ses clients.  
Elle propose également du coaching et du dépannage de sites WordPress via sa plateforme [*WP Support*](https://wp-support.fr/).

### Les outils utilisés par l'entreprise

DM Web utilise divers outils pour mener à bien ces tâches:

- *Visual Studio Code* pour l'environnement de développement
- *Source Tree* pour la gestion de versions, ils travaillent via le système de *features* de *Git Flow*
- *Asana* pour la gestion des projets, l'attribution et le suivi des tâches
- *WAMP* pour l'émulation d'un serveur local
- *Adobe Illustrator* pour les maquettes
- *Laravel* pour le MVC
- *Wordpress* et *WooCommerce* en CMS
- le framework *Bootstrap*
- *SASS*
- *Teams* pour la communication et l'envoi des ressources


## Mes missions au sein de DM Web

### Intégration d'une maquette HTML/CSS

À mon arrivée dans l'entreprise, j'ai commencé , la première semaine, par intégrer une maquette d'un site annuaire d'instituts, qui leur sert de test pour les nouveaux arrivants. Pour cela ils m'ont initié à l'utilisation de SASS et de Bootstrap, et notamment son système de colonnes.
Ensuite j'ai du:
1. créer la **page d'accueil**: avec un **breadcrumb** en Bootstrap (que j'ai ensuite réutilisé pour les autres pages), une bannière avec un formulaire de recherche, une barre de navigation avec un menu hamburger (également à l'aide de Bootstrap), avec en contenu des produits (réalisé avec les **cards** de Bootstrap)
2. créer des templates pour l'**en-tête**, le **pied de page**, la **barre de navigation**, une **card** de produit que j'incluais ensuite en PHP dans mes pages
3. la page **produit** qui reprenait les infos des **cards** de la page d'accueil, et à laquelle s'ajoutait un slider (*TinySlider*), un espace commentaire avec un formulaire permettant d'en poster, un slider pour les  produits en relation.
4. la page **archives** que j'ai du décliner en deux versions, sur la deuxième les **cards** présentant les instituts devaient être simplifiées, avec pour défi de n'utiliser que du CSS (je devais éviter de modifier le template des **cards** produits, et n'utiliser que des classes modifiées en CSS)
5. la page **article** avec une barre latérale pour les publicités
6. retravailler le **responsive** et ajouter une animation CSS pour le soulignement des liens au passage de la souris
7. une fois l'ensemble réalisé j'ai du porter l'ensemble sous *Laravel* pour m'initier au Modèle Vue Controlleur.

|Les domaines de progression: |Les difficultés rencontrées: |
|-----------------------------|-----------------------------|
| Bootstrap (découverte)      | TinySlider                  |
| SASS (découverte)           | Le MVC                      |
| Utilisation des DevTools    |                             |

### Réaliser une landing page

Pour la remise à neuf d'un site d'association, j'ai du réaliser une **landing page** (HTML/CSS) à partir de la maquette fournie.

### Modification du contenu d'un site

Pour préparer le lancement de la nouvelle version d'un site de vente automobile, j'ai travaillé sous Laravel et remplacé le contenu de la page d'accueil (dispositions des blocs d'informations et textes) selon les demandes du client, et modifié les images pour rendre le site plus performant: 
- balises **picture** 
- images en **.webp** et **JPEG**
- attribut **loading: lazy**
- la classe **img-fluid** de Bootstrap

|Les domaines de progression:   |Les difficultés rencontrées:       |
|-------------------------------|-----------------------------------|
| Performances liées aux images | Réadapter le slider de la bannière|

### Modifications de thèmes enfants

Afin de créer facilement des versions légèrements différentes de deux sites de football (un pour lister des matchs, l'autre pour lister des flux d'articles), j'ai travaillé sous WordPress à partir d'un thème enfant pour réaliser d'autres thèmes enfants, l'objectif était de porter les sites sous WordPress à partir de leur version HTML/CSS (page d'accueil et page article). À cette occasion j'ai du:
- travailler avec la **boucle** WordPress
- créer un **Custom Post Type** pour les matchs de la deuxième version, pour pouvoir ajouter facilement une page pour un nouveau match.
- apprendre la **Taxonomie** des pages de thèmes WordPress afin de réaliser les templates et les différents éléments des sites (**side-bar**, **nav-bar**)
- réadapter le menu hamburger, le modèle Bootstrap utilisé pour la version HTML n'était pas celui utilisé par le thème enfant

|Les domaines de progression: |Les difficultés rencontrées: |
|-----------------------------|-----------------------------|
| CPT (découverte)                      | Récupération des données de la boucle|
| Taxonomie de WP (découverte)          | Sidebar dynamique avec les articles  |
| Observer les performances (LightHouse)|                                      |

### Création de pages sous Laravel

Pour la création d'un espace professionnel sur un site de vente en gros, j'ai du réaliser plusieurs pages à partir d'une maquette:
- les pages de contact avec des **formulaires**
- une page **panier** avec un **tableau** de récapitulatif de la commande et une zone d'ajout de commentaire sur la commande
- les pages d'espace personnel d'un compte (dernières commandes, livraisons, factures): une page générale et des pages annexes reprenant les informations plus en détails.
Cela m'a permis de voir à nouveau plus en détail le fonctionnement des **routes**, des **vues** et des **controleurs**, ainsi que d'utiliser *Adobe Illustrator* pour récupérer et exporter les icônes de la maquette au format .SVG.  
Pour ce projet j'ai du utiliser uniquement Bootstrap sous Laravel, je ne pouvais pas utiliser de CSS, on travaillait à plusieurs sur ce projet, et le développeur s'occupait de la partie style, leur objectif était d'ajouter le moins de CSS possible sur ce projet.  

|Les domaines de progression: |Les difficultés rencontrées: |
|-----------------------------|-----------------------------|
| Bootstrap                   | Les controleurs               |
| Les vues                    | Ne pas pouvoir utiliser de CSS|
| Les routes                  |                               |

### Utiliser un plugin WooCommerce

Pour la remise à neuf d'un site de vente pour motos, j'ai du tester plusieurs extensions WordPress qui permettaient de laisser le client configurer l'aspect visuel du produit qu'il souhaitait (choix des couleurs), l'extension retenue, nécessitait de créer des **attributs** aux produits (ex: couleur1 couleur2), puis d'utiliser ces attributs pour créer des variations de produits, pour chaque option du produit je devais ajouter le masque d'image fourni par le client.  

|Les domaines de progression: |Les difficultés rencontrées: |
|-----------------------------|-----------------------------|
| Utilisation d'extensions WP | Documentation légère pour une extension                      |
|                             | La première extension n'était pas compatible avec les autres |
