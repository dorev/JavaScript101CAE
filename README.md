#JavaScript 101

Cette page est une référence rapide pour ceux qui s'intéressent à JavaScript ou qui auraient participé au lunch-n'-learn à ce sujet. Les fichiers contenus dans ce repo sont des exemples sur quelques différents thèmes de ce language.

### Consultez la démo du lunch-n'-learn:

* [Jeudi 21 mars 2019](https://codepen.io/mrelemental/pen/RdYRWY)
* ...


## Codez immédiatement!!

### Pour commencer à coder en javascript, il vous suffit de...
1. Ouvrir un éditeur de texte
2. Y copier ce modèle ci-dessous
3. Sauvegarder le fichier au format **.html**
4. Ouvrir le fichier avec un browser


```html
<!DOCTYPE html>
<html>
  <head>
    <style>
    --> écrire votre CSS ici! <--
    </style>
  </head>
  <body>
  --> écrire votre HTML ici! <--
  </body>
  <script>
  --> écrire votre JavaScript ici!! <--
  </script>
</html>
```

### La base de la base...

On déclare une variable avec `var` et on lui assigne un **string** de valeur "texte". Le `;` à la fin de la ligne est facultatif, mais prenez le réflexe de le mettre!
```javascript
var variable = "texte"; 
```
On utilise `console.log()` pour imprimer le contenu d'une variable. Accédez à la console de votre browser en appuyant sur F12
```javascript
console.log(variable);  // imprime : "texte"
```
Le type de la variable n'est pas figé et sera mis à jour si on lui passe une valeur d'un différent type. On re-déclare `variable` comme le **nombre** 42
```javascript
variable = 42;
console.log(variable);  // imprime : 42
```
On re-déclare `variable` comme une **fonction**
```javascript
variable = function additionner(a,b) { return a + b; };
console.log(variable(2,3));  // imprime : 5
```
On re-déclare `variable` comme un **objet**
```javascript
variable = { nom : "Marc Parent", age : 32, saluer : ()=>{console.log("Allo!");} };
variable.saluer();  // imprime : "Allo!"
```

### Types des variables
JavaScript va automatiquement déterminer quel est le type des valeurs **dynamiquement**. Cela veut dire que des opérations où on additionne des chiffres et du texte sont valides! Ça ne veut pas nécessairement dire que ça donne ce qu'on voudrait...

```javascript
console.log( 2 + "2");  // imprime : "22"
console.log( 5 - "4");  // imprime : 1
```
Dans le premier cas, l'opérateur `+`est interprété comme l'opérateur de concaténation qui va associer deux **string**. Il converti donc le type du premier terme `2` à `"2"` pour effectuer une opération valide.

Dans le deuxième cas, l'opérateur `-` existe uniquement pour des **number** et donc, le terme `"4"` est alors converti en `4`.

### Égalité des types

On peut comparer deux valeurs avec les opérateurs `==` ou `===`.

* `==` va évaluer si deux variables représentent la même valeur
* `===` va évaluer si deux variables représent la même valeur et **sont du même type**

### Les exemples de ce repository contiennent plus d'exemples

* Téléchargez les fichiers
* Ouvrez-les avez un éditeur de texte
* Ouvrez-les également avec un browser
* Faites- des expériences!!!



## Plus de JavaScript à explorer...

[Node.js](https://nodejs.org/)
Un framework permettant de coder du javascript en-dehors du browseret d'accéder aux ressources de l'ordinateur

[D3.js](https://d3js.org/)
Une lib incroyablement puissante pour faire des graphiques de tout genre

[Inkscape](https://inkscape.org/)
Un éditeur similaire à Illustrator spécifique à des SVG

[Tone.js](https://tonejs.github.io/)
Une lib audio très versatile pour créer des sons, jouer du MIDI ou d'autre fichiers.

[interact.js](http://interactjs.io/)
Un tool kit très utile pour faire évoluer rapidement l'interactivité de vos pages HTML
pour browser ou mobile.

[Phaser](https://phaser.io/)
Un framework pour développer des jeux, très complet et bien documenté.