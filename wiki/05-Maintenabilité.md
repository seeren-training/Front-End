# Maintenabilité

*  🔖 **React**
*  🔖 **Vue**
*  🔖 **Angular**

> Dans cette sections nous relèverons les guides de chaque framework et leur dépendances.

___

## ![image](https://raw.githubusercontent.com/seeren-training/Front-End/master/wiki/resources/react.png)

### 🏷️ **Guide**

React n'a pas d'opinion sur la façon dont vous placez les fichiers dans des dossiers. Cela dit, il existe quelques approches courantes populaires dans l'écosystème que vous voudrez peut-être envisager: https://reactjs.org/docs/faq-structure.html

Deux propositions d'organisation par fonctionnalité ou par type de fichier sont proposé par le framework. En l'absence de plus d'informations, de nombreux style guides sont proposés par la communauté: https://blog.bitsrc.io/structuring-a-react-project-a-definitive-guide-ac9a754df5eb

![images](https://raw.githubusercontent.com/seeren-training/Front-End/master/wiki/resources/react-pro.png)

![images](https://raw.githubusercontent.com/seeren-training/Front-End/master/wiki/resources/react-con.png)

### 🏷️ **Stack**

React propose de rendre les vues, mais quand celles ci doivent partager leur données il n'y a pas de solution. Ainsi le projet devra adopter des dépendances pour palier aux fonctionnalités absentes:

* Redux
* Redux Form
* React Ruter
* React Router DOM
* ...

> React ne propose pas de standard de développement et il faudra rapidement plusieurs dépendances pour pouvoir palier aux absences de fonctionnalité indispensables. Les faibles régressions observées, l'absence d'opinion architecturale et la personnalisation de l'écosystème ne facilitent pas la maintenance d'un projet.

___

## ![image](https://raw.githubusercontent.com/seeren-training/Front-End/master/wiki/resources/vue.png)

### 🏷️ **Guide**

Vuex ne restreint pas vraiment la manière dont vous structurez votre code. Il applique plutôt un ensemble de principes de haut niveau: https://vuex.vuejs.org/guide/structure.html.

Par contre il existe un guide de style officiel pour le code spécifique à Vue. Si vous utilisez Vue dans un projet, c'est une excellente référence pour éviter les erreurs et les anti-patterns: https://vuejs.org/v2/style-guide/#Priority-B-Strongly-Recommended

![images](https://raw.githubusercontent.com/seeren-training/Front-End/master/wiki/resources/vue-pro.png)

![images](https://raw.githubusercontent.com/seeren-training/Front-End/master/wiki/resources/vue.con.png)

### 🏷️ **Stack**

Étant un framework progressif, vue s'appuie sur des dépendances internes à ajouter si besoin:

* Vuex
* Vue Router
* Vue Loader
* Vue Server
* Vue Test
* Vue Dev-Tools

Chaque projet peut ainsi avoir une stack différente.

> Vue ne propose pas de standard de développement et il faudra plusieurs de dépendances pour pouvoir personnaliser une application. Les nombreuses régressions observées, l'absence d'opinion architecturale et la personnalisation de l'écosystème ne facilitent pas la maintenance d'un projet.

___

## ![image](https://raw.githubusercontent.com/seeren-training/Front-End/master/wiki/resources/angular.png)

📑 Existe-t-il une méthode recommandée pour structurer les projets Angular?

### 🏷️ **Guide**

Un coding style guide complet est disponible sur la documentation officielle.

* https://angular.io/guide/styleguide#angular-coding-style-guide
* Application structure: https://angular.io/guide/styleguide#application-structure-and-ngmodules
* Structural style guide:
https://angular.io/guide/styleguide#overall-structural-guidelines
* Naming: https://angular.io/guide/styleguide#naming

Le framework cadre fortement le développement en proposant des guides qui peuvent être suivit ou non. Le respect de ce guide permet aux développeurs de prendre leur marque rapidement sur un projet qu'ils découvrent en alignant les pratiques.

![images](https://raw.githubusercontent.com/seeren-training/Front-End/master/wiki/resources/angular-pro.png)

![images](https://raw.githubusercontent.com/seeren-training/Front-End/master/wiki/resources/angular-con.png)

### 🏷️ **Stack**

Angular est un framework complet et possède des dépendances internes, il y a aussi des dépendances externes sur les librairies d'observables mais basées sur des spécifications stables: https://angular.io/guide/npm-packages

> Angular propose un standard de développement et peu de dépendances pour pouvoir maintenir une application sans difficulté.

___

> Nous allons essayer chacune de ces technologies pour se faire un avis concret