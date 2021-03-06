# Starter pour katas de code

Le but est, par la réalisation d'exercices simples de code, de s'habituer au développement avec tests unitaires et de mettre en place une bonne fréquence de commit en fonction de l'avancement du code.

## Installation
1 Cloner le projet starter

2 Créer votre branche

3 Télécharger composer [ici](https://getcomposer.org/download/) à la racine du projet

4 Installer les dépendences :

    $ php composer.phar install

5 Vous êtes prêts à travailler !

## Trucs et astuces
### Composer
Mettre à jour le fichier autoloader :

    $ php composer.phar dumpautoload
### PHPUnit
Lancer les tests :

    $ vendor/bin/phpunit


## Exercice 1 : FizzBuzz
### Régle du jeu
Le but est de lister les nombres de 1 à 100, en remplaçant le nombre par un mot selon certaines conditions :
* Le mot Fizz si le nombre est multiple de 3,
* Le mot Buzz si le nombre est multiple de 5,
* Le mot FizzBuzz si le nombre est multiple de 3 et de 5.

### Nouvelles règles
Même exercice avec les règles suivantes :
* Le mot Fizz si le nombre est multiple de 3 ou contient le chiffre 3,
* Le mot Buzz si le nombre est multiple de 5 ou contient le chiffre 5,
* Le mot FizzBuzz si le nombre respecte les 2 premières règles.

## Exercice 2 : Word-wrapping
Le but est d'écrire un algorithme qui prend un texte et une longueur de colonne et qui renvoie une liste de mots (coupés ou non) pouvant se positionner dans une colonne

Exemples de comportement :
* Si la largeur de colonne est 60 et que la taille du texte est de 30, le résultat est [texte]
* Si la largeur de colonne est 3 et que le texte est "abc def" le résultat est ["abc", "def"]
* Si la largeur de colonne est 3 et que le texte est "abcdef" le résultat est ["abc", "def"]
* Si la largeur de colonne est 3 et que le texte est "abcdef abc" le résultat est ["abc", "def", "abc"]
* Si la largeur de colonne est 3 et que le texte est "a b c d e f" le résultat est ["a b", "c d", "e f"]
