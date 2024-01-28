# Bootcamp en Bug Bounty et Penetration Testing

Mise à jour complète avec tous les outils modernes de Bug Bounty et les meilleures pratiques de Penetration Testing ! Rejoignez une communauté en ligne de plus de 900,000 étudiants et un cours enseigné par des experts du secteur. Ce cours vous amènera d'un niveau débutant absolu à celui d'expert en sécurité et chasseur de bugs, afin d'améliorer la sécurité pour vos clients et pour toute application web que vous pourriez créer à l'avenir !

Ce cours est axé sur l'apprentissage par la pratique. Nous allons vous enseigner comment fonctionne le test de pénétration, en pratiquant réellement les techniques et méthodes utilisées par les chasseurs de bugs aujourd'hui. Nous commencerons par créer notre laboratoire de piratage virtuel pour assurer la sécurité de vos ordinateurs tout au long du cours, en faisant les choses légalement, et en préparant nos ordinateurs pour le test de pénétration.

Nous plongeons dans des sujets tels que :

## 1) Introduction au Bug Bounty :

Ici, nous abordons simplement la théorie de ce qu'est exactement le Bug Bounty et le Penetration Testing.

Exemple rapide d'une vulnérabilité que nous couvrirons.

Cheminement de carrière d'un Pen Tester.

## 2) Configuration de notre laboratoire virtuel :

Création de notre laboratoire virtuel que nous utiliserons tout au long du cours (machine Kali Linux).

Installation d'une VM vulnérable appelée OWASPBWA que nous attaquerons.

Création d'un compte en ligne sur la plateforme TryHackMe.

Pour presque chaque vulnérabilité, nous couvrirons un exemple sur TryHackMe et également sur notre machine virtuelle vulnérable.

À partir d'ici, choisissez 2 chemins différents en fonction des connaissances que vous avez déjà.

## 3) Énumération de site Web et collecte d'informations

C'est là que nous commençons avec la pratique du Bug Bounty / Penetration Testing de site Web. Nous couvrons de nombreuses tactiques et outils qui nous permettent de recueillir autant d'informations que possible sur un certain site Web. Pour cela, nous utilisons différents outils comme Dirb, Nikto, Nmap. Nous utilisons également le piratage Google, qui est une compétence utile à avoir une fois que les outils ne sont pas disponibles.

## 4) Introduction à Burpsuite

C'est un outil très important pour un Bug Hunter. Presque tous les Bug Hunters connaissent cet outil (et l'utilisent probablement). Il possède de nombreuses fonctionnalités différentes qui facilitent la recherche de bugs. Certaines de ces fonctionnalités sont l'exploration de la page Web, l'interception et la modification des requêtes HTTP, les attaques par force brute et plus encore.

## 5) Injection HTML

C'est notre premier bug. C'est aussi l'un des plus faciles, donc nous commençons avec. L'injection HTML consiste essentiellement à trouver une entrée vulnérable sur la page Web qui permet d'injecter du code HTML. Ce code est ensuite rendu sur la page en tant que vrai HTML.

## 6) Injection/Exécution de commande

Notre premier bug dangereux. Injecter des commandes est possible lorsque le serveur exécute notre entrée à travers son système sans filtrage. Cela pourrait être quelque chose comme une page Web qui nous permet de pinger d'autres sites Web mais ne vérifie pas si nous avons entré une commande différente de l'adresse IP dont il a besoin. Cela nous permet d'exécuter des commandes sur le système, de compromettre le système via un shell inversé et de compromettre des comptes sur ce système (et toutes les données).

## 7) Authentification cassée

C'est une autre vulnérabilité qui se produit sur les sites Web. Elle fait essentiellement référence à une faiblesse dans 2 domaines : la gestion des sessions et la gestion des identifiants. Elle permet à l'attaquant de se faire passer pour des utilisateurs légitimes en ligne. Nous montrons différents exemples à travers les valeurs de cookies, les requêtes HTTP, la page de mot de passe oublié, etc.

## 8) Attaques par force brute

Ceci peut poser problème même si le site web est sécurisé. Si le client a défini un mot de passe simple et facile, il sera également facile à deviner. Nous couvrons différents outils utilisés pour envoyer de nombreux mots de passe à la page web afin de s'introduire dans un compte.

## 9) Exposition de données sensibles

Ce n'est pas une vulnérabilité du système. C'est plutôt lorsque les développeurs oublient de retirer des informations importantes pendant la production, qui peuvent être utilisées pour mener une attaque. Nous couvrons un exemple où le développeur a oublié de retirer l'accès à la base de données entière aux utilisateurs réguliers.

## 10) Contrôle d'accès cassé

Le contrôle d'accès fait respecter la politique selon laquelle les utilisateurs ne peuvent pas agir en dehors de leurs permissions prévues. Les défaillances mènent généralement à la divulgation non autorisée, la modification ou la destruction de toutes les données, ou à l'exécution d'une fonction commerciale au-delà des limites de l'utilisateur. Ici, nous couvrons une vulnérabilité appelée référence directe d'objet non sécurisée. Un exemple simple serait une application qui a des identifiants d'utilisateur dans l'URL. Si elle ne stocke et ne gère pas correctement ces identifiants, un attaquant pourrait potentiellement changer l'identifiant et accéder aux informations d'un autre utilisateur.

## 11) Mauvaise configuration de sécurité

Nous avons placé ceci dans une section séparée, cependant, toutes les vulnérabilités précédentes y appartiennent également. Ici, nous montrons un exemple de vulnérabilité où les administrateurs de sites web n'ont pas changé les informations d'identification par défaut pour une certaine application qui fonctionne sur leur serveur.

## 12) Cross Site Scripting - XSS

C'est une vulnérabilité importante et très courante sur de nombreux sites web. Cette vulnérabilité nous permet d'exécuter du code Javascript sur la page web. Cela est dû au fait que l'entrée de l'utilisateur n'est pas bien filtrée et traite l'entrée comme du code javascript. Il existe 3 principaux types de XSS : le XSS stocké, le XSS reflété et le XSS basé sur le DOM. Nous couvrons ces 3 types ainsi que quelques cas inhabituels.

## 13) Injection SQL

Une autre vulnérabilité majeure et vraiment dangereuse. De nombreux sites web communiquent avec la base de données, que ce soit une base de données qui stocke des informations sur les produits ou sur les utilisateurs. Si la communication entre l'utilisateur et la base de données n'est pas filtrée et vérifiée, elle pourrait permettre à l'attaquant d'envoyer une requête SQL et de communiquer avec la base de données elle-même, lui permettant d'extraire toute la base de données ou même de la supprimer. Il existe plusieurs types d'injection SQL tels que l'injection SQL basée sur les erreurs ou l'injection SQL aveugle.

## 14) Injection XML, Injection XPath, XXE

XXE ou XML External Entity est une vulnérabilité qui permet à un attaquant d'interférer avec un site web qui traite des données XML. Elle pourrait permettre à l'attaquant d'exécuter un shell inversé ou de lire des fichiers sur le système cible, ce qui en fait une vulnérabilité grave.

## 15) Composants avec des vulnérabilités connues

Même si le site web peut ne pas être vulnérable, le serveur peut exécuter d'autres composants/applications qui ont une vulnérabilité connue qui n'a pas encore été corrigée. Cela pourrait nous permettre de réaliser divers types d'attaques en fonction de ce qu'est cette vulnérabilité.

## 16) Journalisation et surveillance insuffisantes

La journalisation et la surveillance doivent toujours être effectuées du point de vue de la sécurité. Elles permettent de suivre toutes les requêtes et informations qui transitent par notre application. Cela aide à identifier si une attaque est en cours ou, si l'attaque s'est déjà produite, à examiner l'incident plus en profondeur pour identifier l'attaque et ensuite modifier l'application afin de prévenir une attaque similaire à l'avenir.

## 17) Monétisation de la chasse aux bugs

Après avoir pratiqué et couvert toutes les vulnérabilités, il est important de mentionner comment nous pouvons monétiser nos connaissances. Nous mentionnons différentes plateformes qui peuvent être utilisées pour commencer votre carrière en tant que chasseur de bugs, et nous prenons également une plateforme comme exemple pour montrer à quoi ressemble un programme de bug bounty et sur quoi porter attention lors de l'application.

## 18) Bonus - Fondamentaux du développement web

Pour tous ceux qui manquent de connaissances en développement Web ou en compréhension du fonctionnement et de la structure des sites Web.

## 19) Bonus - Terminal Linux

Pour ceux qui manquent de connaissances dans l'utilisation simple du terminal Linux, car nous l'utiliserons tout au long du cours.

## 20) Bonus - Réseautage

Les fondamentaux du réseautage et certains termes de base utilisés par les testeurs de pénétration ou les chasseurs de bugs.
