# JavascriptExo

# Les conditions

## Exo 1

On va demander à notre utilisateur d'entrée son nom et son âge,
notre programme devra retourner `{prenom} vous avez {age}`.

1. Vous devez pour ça demander à l'utilisateur son prénom
2. Son âge
3. Faire un `alert()` pour retourner le tout

## Bonus

-   Vérifier si l'utilisateur à saisie une donnée.
    -   L'âge doit être un entier.
    -   Pour le nom, peut importe si c'est un nombre ou pas
-   Vérifier si l'utilisateur est majeur ou mineur et le retourner dans un `alert()`
-   `Si` il est majeur dire depuis quand il est majeur
-   `Si` il est mineur dire dans combien de temps il sera majeur.

## Exo 2

On va créer notre 1er jeu, le juste prix

Pour ce faire, nous allons faire ça en plusieurs étapes.

1.  JavaScript va rechercher un nombre aléatoire entre 0 et 500. (Grâce à l'objet Math.random() et Math.floor())
    -   Le nombre sera stocké dans une variable appelé `nbRandom`
2.  Faire une boucle qui `tant que` le nombre saisie par l'utilisateur n'est pas trouvé affichera un nouveau `prompt` avec comme texte condition `si` le nombre est plus grand ou plus petit.
3.  une fois le bon numéro trouvé, affiché une alerte qui informe que le user a gagné.

## Bonus

-   On va améliorer le programme. On va vérifier si le nombre saisie est un entier, et si c'est un entier positif.
-   On indique le nombre de tentatives que l'utilisateur à mis à touver le juste prix.
-   Si l'utilisateur annule le jeu, une alerte aparait avec le message suivant `"dommage d'abandonné, à la prochaine fois !"`.

# Les fonctions

## Exo 1

Vous devez créer une fonction nommée `num` qui renvoie le nombre 42.

> Car 42 est la réponse à La grande question sur la vie, l'univers et le reste aussi.

1. Vous devez laisser l'utilisateur entrer un chiffre et vous devez vérifier si c'est bon ou pas.

## Exo 2

Créer une fonction qui prend en paramètre 1 argument et vous devez retourner le carré de ce chiffre.

## Bonus

-   Changer la fonction pour qu'elle prenne 2 paramètres
    -   Un nombre
    -   Son exposant

## Exo 3

L'objectif de cet exercice est de créer une fonction permettant de renvoyer le **mot** correspondant au chiffre passé en argument.

Les valeurs d'entrées sont les chiffres de `0` à `2` inclu.

## Exemples

-   Pour le chiffre `0`, la fonction doit renvoyer `zéro`
-   Pour le chiffre `1`, la fonction doit renvoyer `un`
-   Pour le chiffre `2`, la fonction doit renvoyer `deux`

## Exo 4

Étant donné un prénom `prenom`, la fonction doit renvoyer `Un pour <prenom>, un pour moi.`.

Si aucun prénom n'est donné, la fonction doit renvoyer `Un pour toi, un pour moi.`.

## Exo 5

1. Créez maintenant une fonction nommée `add` qui prend 2 arguments. Celle ci doit renvoyer la somme des deux nombres entier.
2. Créez maintenant une fonction nommée `substraction` qui prend 2 arguments. Celle ci doit renvoyer la soustraction des deux nombres entier.
3. Créez maintenant une fonction nommée `multiply` qui prend 2 arguments. Celle ci doit renvoyer la multiplication des deux nombres entier.
4. Créez maintenant une fonction nommée `diviser` qui prend 2 arguments. Celle ci doit renvoyer la division des deux nombres entier.

## Bonus

-   Demander dans un prompt les 2 valeurs à l'utilisateur.
    -   Par défaut, le choix se fera sur la fonction `add` et retourner la valeur
-   Demander à l'utilisateur les 2 valeurs et ce qu'il compte faire (ajouter, multiplier, soustraire ou diviser) et retourner la valeur
    -   Si on choisi de diviser, il faut s'assurer que le 2eme chiffre soit pas égale à 0. Car une division par 0 est interdite.

## Exo 6

> Ne vous laissez pas intimider par le côté "Maths" de ce problème, il n'est pas si difficile. J'ai ajouté pour vous aider une fonction qui renvoie vrai si un nombre est pair et faux sinon. Bon courage !

La conjecture de Syracuse ou le problème 3x + 1 peut être résumé comme ceci :

Prenez un nombre entier positif `n`. Si `n` est pair, divisez-le par 2 pour obtenir `n / 2`. Si `n` est impair, multipliez-le par 3 et ajoutez 1 pour obtenir `n * 3 + 1`.

Répétez ce processus indéfiniment. La conjecture établit que peu importe le nombre avec lequel vous commencez, vous finirez toujours par atteindre 1.

Étant donné un nombre `n`, retournez le nombre d'étapes nécessaires pour atteindre 1.

## Exemples

On commence avec `n = 12`, les étapes seraient les suivantes :

| Étape | Rendu |
| ----- | ----- |
| 0     | 12    |
| 1     | 6     |
| 2     | 3     |
| 3     | 10    |
| 4     | 5     |
| 5     | 16    |
| 6     | 8     |
| 7     | 4     |
| 8     | 2     |
| 9     | 1     |

On atteint 1 en 9 étapes. Donc pour `n = 12`, la fonction doit retourner `9`.

Un peut d'aide

```javascript
function exercice6(n) {}

function nombreEstPair(nombre) {
	return nombre % 2 === 0;
}
```

## Exo 7

Étant donné les longueurs des 3 côtés d'un triangle, votre fonction devra renvoyer si celui-ci est `équilatéral`, `isocèle`, `scalène` ou `impossible`.

-   Un triangle est `équilatéral` lorsque ses 3 côtés sont égaux
-   Un triangle est `isocèle` lorsque 2 de ses côtés sont égaux
-   Un triangle est `scalène` lorsqu'aucun de ses côtés n'est égal à un autre côté
-   Un triangle est `impossible` lorsque la somme de deux de ses côtés est strictement inférieure au troisième côté

## Exemples

-   (2, 3, 2) est un triangle `isocèle`
-   (7, 7, 7) est un triangle `équilatéral`
-   (3, 5, 6) est un triangle `scalène`
-   (2, 8, 5) est un triangle `impossible` car 2 + 5 < 8 !

## Exo 8

### FizzBuzz

Rédigez une fonction qui retourne, sous la forme d'une chaîne de caractères, les nombres de 1 à 200 dans l’ordre, en remplaçant :

-   les multiples de 3 par le mot Fizz
-   les multiples de 5 par le mot Buzz
-   les multiples de 15 par le mot FizzBuzz

Les différents mots devront être séparés par des " - ".

Attention, l'exercice n'est pas si simple qu'il n'y paraît...

## Exemple

Voici un extrait pour les nombres de 1 à 10 :
'1 - 2 - Fizz - 4 - Buzz - Fizz - 7 - 8 - Fizz - Buzz'
