# Stabilité

*  🔖 **React**
*  🔖 **Vue**
*  🔖 **Angular**

___

## 📑 React

![image](https://raw.githubusercontent.com/seeren-training/Front-End/master/wiki/resources/react.png)

Créez des composants autonomes qui maintiennent leur propre état, puis assemblez-les pour créer des interfaces utilisateurs complexes.

### 🏷️ **Utilisation**

Toute personne ayant une connaissance préalable de base en programmation peut facilement comprendre React alors que Angular et Ember sont appelés «langage spécifique au domaine», ce qui implique qu’il est difficile de les apprendre. Pour réagir, vous avez juste besoin de connaissances de base en CSS et HTML.

Les composants React implémentent une méthode render() qui prend des données en entrée et retourne ce qui doit être affiché. Cet exemple utilise une syntaxe qui ressemble à du XML et qu’on appelle JSX. Les données passées au composant sont accessibles dans render() via this.props.

*Template*

```html
<div id="hello-example"></div>
```

*Component*

```js
class HelloMessage extends React.Component {
  render() {
    return (
      <div>
        Salut {this.props.name}
      </div>
    );
  }
}

ReactDOM.render(
  <HelloMessage name="Thierry" />,
  document.getElementById('hello-example')
);
```

### 🏷️ **Fonctionnalités**

React est une bibliothèque de composants d'interface utilisateur légère qui n'est que le «V» dans MVC. Cela signifie que React vous donne plus de liberté pour choisir les bibliothèques qui vous conviennent, mais vous devrez également vous occuper des mises à jour et des migrations correspondantes...

Le framework propose les fonctionnalité suivantes:
* Virtual DOM (Document Object Model)
* JSX files
* XSS protection
* Functional components
* Basic state management with setState and Context API

> 🔗 react-api: https://fr.reactjs.org/docs/react-api.html

Pour le reste il faudra installer des packages additionnels.

### 🏷️ **Versions**

La première **version stable est la 15.0.0** publiée le 07 Avril 2016. Précédemment il n'y avait que des versions candidates, dont la première était publiée en 2011.

Versions:
* 🔗 Npm: https://www.npmjs.com/package/react
* 🔗 Github: https://github.com/facebook/react/releases
* 🔗 Site officiel: https://fr.reactjs.org/versions/

### 🏷️ **Roadmap**

React publie les changements pour chaque version dans les Changelog associés et publie sur son blog les feuilles de routes des développements ainsi que le récapitulatif des version candidates.

* React v17.0 RC: https://fr.reactjs.org/blog/2020/08/10/react-v17-rc.html
* React v16.13.0: https://fr.reactjs.org/blog/2020/02/26/react-v16.13.0.html
* React v16.9.0: https://fr.reactjs.org/blog/2019/08/08/react-v16.9.0.html

Nous pouvons observer que la 16.9 introduit des déprécations en warning, que la 16.13 ajoute encore des warnings de dépréciation et que sur la 17.0 les warnings deviennent des erreurs parce que passent obsolètes. Les feuilles de routes sont donc à suivre sur chaque version pour s'adapter syntaxiquement en vue de mettre à jour la librairie sur un projet.

> Concernant l'équipe de développements, les connaissances à acquérir sont les suivantes:

![image](https://raw.githubusercontent.com/seeren-training/Front-End/master/wiki/resources/react-roadmap.png)

___

> Nous pouvons conclure qu'une version stable s'est faite attendre, que la dépréciation et l'obsolescence se produit sur le cœur de la librairie d'une version majeure à une autre et que la librairie s'appuie sur des packages externes qu'il faudra également surveiller.

___

## 📑 Vue

![image](https://raw.githubusercontent.com/seeren-training/Front-End/master/wiki/resources/vue.png)

À la différence des autres frameworks monolithiques, Vue a été conçu et pensé pour pouvoir être adopté de manière incrémentale. Le cœur de la bibliothèque se concentre uniquement sur la partie vue. D’un autre côté, Vue est tout à fait capable de faire tourner des applications web monopages quand il est couplé avec des outils modernes et des bibliothèques complémentaires.

### 🏷️ **Utilisation**

Ce framework présuppose que vous ayez un niveau intermédiaire de connaissance en HTML, CSS et JavaScript. Si vous êtes complètement nouveau dans le développement frontend, ce n’est peut-être pas la solution la plus judicieuse de vous lancer dans un framework pour vos premiers pas — Nous vous recommandons de compléter vos bases avant de revenir.

Cela ressemble assez au rendu d'un temlate, mais Vue a fait beaucoup de travail sous le capot. Les données et le DOM sont désormais liés, et tout est désormais réactif.

*Template*

```html
<div id="components-demo">
  <button-counter></button-counter>
</div>
```

*Component*

```js
Vue.component('button-counter', {
  data: function () {
    return {
      count: 0
    }
  },
  template: '<button v-on:click="count++">You clicked me {{ count }} times.</button>'
})
```

### 🏷️ **Fonctionnalités**

Un écosystème progressivement adoptable qui évolue entre une bibliothèque et un framework complet.

Le framework propose les fonctionnalité suivantes:
* Virtual DOM
* Components
* Transition
* Templates
* Routing

> 🔗 vue-api: https://vuejs.org/v2/api/

Pour le reste il faudra installer des packages additionnels.

### 🏷️ **Version**

La première **version stable est la 1.0.0 Evangelion** publiée le 27 Octobre 2015. Précédemment il n'y avait que des versions de développement ou candidates, dont la première était publiée en 2013.

Versions:
* 🔗 Npm: https://www.npmjs.com/package/vue
* 🔗 Github: https://github.com/vuejs/vue/releases

### 🏷️ **Roadmap**

Vue publie une roadmap sur github ainsi que le "request for comments process" des merges.

* Roadmap: https://github.com/vuejs/vue/projects/6
* RFCS: https://github.com/vuejs/rfcs/pulls?q=label%3A%22breaking+change%22+
* Migration guide: https://v3.vuejs.org/guide/migration/introduction.html#breaking-changes

Nous pouvons constater qu'il y a des changements syntaxiques majeurs d'une version à l'autre et une migration de la version 2 à 3 ne peut se faire dès sa sortie. Les changements syntaxiques sont importants et concernent quasi chaque fonctionnalité. Les problèmes de migration sont détaillés sur le site officiel ainsi que sur différents blogs de la communauté: https://tsh.io/blog/vue-new-features/

> Concernant l'équipe de développements, les connaissances à acquérir sont les suivantes:

![image](https://raw.githubusercontent.com/seeren-training/Front-End/master/wiki/resources/vue-roadmap.jpeg)

___

## 📑 Angular

![image](https://raw.githubusercontent.com/seeren-training/Front-End/master/wiki/resources/angular.png)

À la différence des autres frameworks monolithiques, Vue a été conçu et pensé pour pouvoir être adopté de manière incrémentale. Le cœur de la bibliothèque se concentre uniquement sur la partie vue. D’un autre côté, Vue est tout à fait capable de faire tourner des applications web monopages quand il est couplé avec des outils modernes et des bibliothèques complémentaires.

### 🏷️ **Utilisation**

Angular est une plate-forme et un cadre pour la création d'applications client d'une seule page à l'aide de HTML et de TypeScript. Angular est écrit en TypeScript. Il implémente les fonctionnalités de base et facultatives en tant qu'ensemble de bibliothèques TypeScript que vous importez dans vos applications.

*Template*

```html
<my-app></my-app>
```

*Component*

```ts
@Component({  
    selector: 'my-app',  
    template: '<h1>{{name}}</h1>'  
})  
export class AppComponent {  
    public name: string = 'Angular';
}  
```

### 🏷️ **Fonctionnalités**

Un écosystème progressivement adoptable qui évolue entre une bibliothèque et un framework complet.

Le framework propose les fonctionnalité suivantes:
* Components
* Transition
* Templates
* Routing
* UI Components
* Inversion of Control
* IDE
* ...

> 🔗 angular-features: https://angular.io/features

### 🏷️ **Version**

La première **version stable est la 2.0.0** publiée le 14 septembre 2016. Précédemment il n'y avait qu'une version candidate proposée l'année précédente.

Versions:
* 🔗 Npm: https://www.npmjs.com/package/@angular/core
* 🔗 Github: https://github.com/angular/angular/releases

### 🏷️ **Roadmap**

Angular publie une roadmap et une politique de support sur leur site:
* Roadmap: https://angular.io/guide/roadmap
* Support policy: https://angular.io/guide/releases#support-policy-and-schedule
* Deprecation practice: https://angular.io/guide/releases#deprecation-practices
* Changelog: https://github.com/angular/angular/blob/master/CHANGELOG.md

Nous pouvons constater qu'il y a très peu de des changements syntaxiques, sur l’année cela correspond à marquer deprecated l'utilisation d'un type générique sur un élément de formulaire.

> Concernant l'équipe de développements, les connaissances à acquérir sont les suivantes:

![image](https://raw.githubusercontent.com/seeren-training/Front-End/master/wiki/resources/angular-roadmap.png)

___

> Après avoir observé la stabilité de ces technologies nous allons nous intéresser à leur maintenabilité.