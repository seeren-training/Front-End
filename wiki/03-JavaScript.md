# JavaScript

*  🔖 **Technologies**
*  🔖 **DOM**
*  🔖 **CBA**

L’écosystème de JavaScript est très riche, nous allons observer les librairies et frameworks ayant une base utilisateur solide.

___

## 📑 Technologies

Historiquement le package manager du langage est **npm**. Il en existe d'autres, qui ont disparus depuis ou qui sont encore d'actualité. Ce package manager est distribué avec la plateforme logicielle **node.js** afin qu'il utilise pour performer ses installations.

![image](https://raw.githubusercontent.com/seeren-training/Front-End/master/wiki/resources/node.png)

Ce package manager permet sur une simple commande de télécharger un package dans un dossier `node_modules` à la racine du projet.

```bash
npm install <package-name>
```

L'écosystème et les paradigmes de développement sur JavaScript évoluent avec le temps, l'on peut parler de l'avant et de l'après 2015.


___

## 📑 DOM

La principale activité de JavaScript orienté front-end est de produire un affichage et de de dynamiser le **Document Object Model**. Historiquement, de nombreuses librairies facilitant la manipulation du DOM ont marqué le langage.

![image](https://raw.githubusercontent.com/seeren-training/Front-End/master/wiki/resources/jquery.png)

Même s'il est évident que la bibliothèque perd progressivement son terrain, elle est toujours d'actualité.

De nombreux sites Web l'utilisent. Selon BuiltWith, JQuery est toujours utilisé sur 77% des meilleurs 1 million de sites Web. Donc, si vous rencontrez un jour travailler sur un tel site Web, vous devriez connaître la bibliothèque.

Ces jours-ci, JavaScript a évolué. Les navigateurs sont livrés avec un bon support pour ses API. Ainsi, les choses autrefois facilitées par JQuery sont désormais tout à fait possibles sans lui. Pourquoi ajouter une dépendance indésirable qui ne fait qu'aider à gonfler votre application?


![image](https://raw.githubusercontent.com/seeren-training/Front-End/master/wiki/resources/vanilla.png)

Vanilla JavaScript est devenu populaire en raison de la prédominance des bibliothèques JavaScript externes telles que jQuery. Il ne fallut pas longtemps avant que «l'écosystème» JavaScript ne soit inondé de plugins et d'outils populaires qui reposaient sur des bibliothèques externes.

jQuery en est un exemple parfait. jQuery est une excellente bibliothèque qui peut vous aider à simplifier certaines opérations. Cela peut également vous faire économiser beaucoup de temps et d'efforts. En outre, la bibliothèque a aidé à résoudre de nombreux problèmes de navigateurs croisés qui existaient à l'époque où Internet Explorer était encore largement utilisé. Mais ce n'est plus le cas maintenant.

___

Ne pas respecter le principe d'encapsulation d'un composant et ne pas mettre en relation un état et son formatage ne permet pas de faire grandir une solution sereinement: qui veut faire du DOM?

___

## 📑 CBA Frameworks

Aux alentours de 2015 et la standardisation des Web Components, les frameworks majeurs que nous connaissons aujourd'hui illustrent la maturité de ce composite sur JavaScript et utilisent une **component based architecture**.

## 2015-2020

*JavaScript Frameworks*

## ![image](https://raw.githubusercontent.com/seeren-training/Front-End/master/wiki/resources/ranking.png)

___

Définissons les principaux frameworks historiques toujours d'actualité.

___

## ![image](https://raw.githubusercontent.com/seeren-training/Front-End/master/wiki/resources/ember.png)

### 2011

Le framework a été créé par Yehuda Katz, un membre de jQuery, Ruby on Rails. Il utilise le composite **MVC**.

### 2018

Le **MVC** est remplacé par un modèle de type modèle-route-**composant** et une architecture basée su les composants. Le framework est utilisé par:

* Yahoo
* LinkedIn
* Netflix1
* Square
* Heroku
* Apple 
* NBC News 

___

## ![image](https://raw.githubusercontent.com/seeren-training/Front-End/master/wiki/resources/react.png)

### 2013

React est créé par Jordan Walke, un ingénieur au sein de la société Facebook. Le but principal de cette bibliothèque est de créer de vues, via la création de **composants** dépendant d'un **état** et générant une rendu à chaque changement d'état. 

 Pour faciliter l'écriture de la vue, l'équipe initiale chez Facebook a développé un langage, **JSX**, qui permet de générer des objets JavaScript avec une notation similaire à XML. La librairie est utilisée par:

* Netflix
* Yahoo5
* Airbnb
* Sony
* Atlassian
* Facebook
* Instagram
* WhatsApp

___

![image](https://raw.githubusercontent.com/seeren-training/Front-End/master/wiki/resources/vue.png)

### 2014

Vue a été créée par Evan You après avoir travaillé pour Google en utilisant AngularJS dans un certain nombre de projets

Vue présente une **architecture progressivement adoptable** qui se concentre sur le rendu déclaratif et la composition des **composants**. Le framework est utilisée par:

* Adobe
* Alibaba
* GitLab

___

![image](https://raw.githubusercontent.com/seeren-training/Front-End/master/wiki/resources/angular.png)

### 2009

AngularJS est fondé sur l'idée que la programmation déclarative doit être utilisée pour construire les interfaces utilisateurs et les composants logiciels de câblage, tandis que la programmation impérative excelle pour exprimer la logique métier. Il suit le patron d'architecture **MVC**

### 2016

Angular est un framework côté client, open source, basé sur **TypeScript**, supportant le JavaScript et co-dirigé par l'équipe du projet « Angular » à Google et par une communauté de particuliers et de sociétés.

Il utilise une hiérarchie de **composants** comme principale caractéristique architecturale. Le framework est utilisée par:

* Microsoft Office
* Deutsche Bank
* Mixer
* Santander
* Gmail
* Forbes
* Upwork
* PayPal
* Samsung

___

## Opinions

L'on remarque que l'adoption de REACT est immédiate tout comme l’intérêt porté à la librairie, contrairement à  Angular dont 35% des utilisateurs ne souhaitent pas continuer son utilisation.

## ![image](https://raw.githubusercontent.com/seeren-training/Front-End/master/wiki/resources/interest.png)

___

> Nous observerons en détail la stabilité de ces frameworks.