# Responses TP JS

### Question 1
Play the whole game with size=2. By browsing the 3 views of the application, how many files did your browser download overall? How many time did it took to load them all?
- Sur la première vue : 5 fichiers, 60 ms
- Sur la deuxième vue : 10 fichiers, 95 ms
- Sur la troisième vue : 6 fichiers, 61 ms

### Question 2
Component-oriented programming for the web is considered more maintainable. Why?
- les composants sont plus simples à maintenir en web parce que lorsqu'il est necessaire d'effectuer des modification, il n'est pas necessaire de plonger dans tout le code, mais simplement de modifier ce que l'on veut dans les fichiers composants, l'ensemble des composants seront donc affectés (par exemple, changer la couleur principale du site, une valeur à changer plutot que 10 000 hexa disséminées partout dans le css)

### Question 3
If you look at the source code, every JS file wraps its code into a closure:
- On a deux variables environnement si on enleve les closures, 
du coup il est necessaire soit d'enlever une des deux variables, soit de laisser les closures

### Question 4
As you can see, `npm install` command also generated a `package-lock.json` file along with `package.json`. What is the purpose of this file?
- Ce fichier permet de garder une trace des versions exactes de chaque packages qui ont été installés puis mis a jour pour que le produit soit 100 reproductibles, exactement à l'identique 

### Question 5 
By convention, all NPM dependencies use a 3-digit format for version numbers. How do you call this? Can you explain the meaning of the ^ symbol next to the bootstrap version?
- les trois numeros correspondent à des types de mises à jour, le premier chiffre indique une modification de beaucoup d'éléments, une modif de comportement du package, le deuxième correpond à un ajout de fonctionnalités, le dernier correspond a des patchs pour corriger des bugs.
- le symbole ^ permet d'indiquer qu'on ne veut pas de version qui ne fasse varier le premier chiffre différent de 0 en partant de la gauche, comme expliqué [ici](https://nodejs.dev/learn/the-package-lock-json-file)

### Question 6 
What is a devDependency exactly? What are the differences with a dependency?
- Une dev dependency est une dépendance necessaire durant la phase de developpement contrairement a une dépendence "classique" qui est necessaire pour que le projet fonctionne

### Question 7 
Can you think of at least 2 things that are possible with Java classes, but cannot be done with ES6 classes?

### Question 8
What are the differences between `var` and `let`
- la différence principale est que `var` est une fonction, on peut redéclarer `var a=5` plusieurs fois alors que `let` est un bloc, on ne peut le déclarer qu'une seule fois
