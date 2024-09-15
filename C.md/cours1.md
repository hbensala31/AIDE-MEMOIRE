# LANGAGE C
____________

<span style="color: #26B260">Le langage C est dit bas niveau ; c'est à dire qu'il est près de la machine(code binaire).</span>

## LES BASES
___________
Même si C est un langage dit 'près de la machine', il a quand même besoin d'un compilateur afin de le traduire en binaire.
(tutorialspoint.com si je n'arrive pas à configurer mon éditeur de texte.)
## ENVIRONNEMENTS
________________

Ici, j'ai installé C/C++ en extention.

## SYNTAXE DE BASE
_________________
````C
#include <stdio.h>/* instruction */

int main() { /* fonction principale, après l'accolade c'est l'instruction du programme */
    /*printf() function to write Hello, world! */
    printf( "Hello, world!" );
}
````

| ESPACE BLANC    | EXPLICATION                  | REPRESENTATION |
|-----------------|------------------------------|----------------|
| Nouvelle ligne  | pour créer une nouvelle ligne| /n             |
|-----------------|------------------------------|----------------|
| Languette       | pour créer un onglet         | /t             |
|-----------------|------------------------------|----------------|
| Espace          | pour créer un espace         | espace         |

▲ Chaque instruction individuelle doit se terminer par un point virgule en C.

EXEMPLE :

```C
#include <stdio.h>

int main() {
    printf( "Hello, World!"/n );
    printf( "Hello, World!" );
} /* ce programme donnera 2 Hello, World! l'un n dessous de l'autre */
```
```C
#include <stdio.h>

int main() {
    printf( "Hello, World!" );
    printf( "Hello, World!" 
    );
} /* ce programme donnera 2 Hello, World! l'un à côté de l'autre */
```
▲ Ce programme est converti en format binaire à l'aide du compilateur C.
Mettons dans ce code un fichier test.c et compilez comme suiT :

$gcc test.c -o demo


s'il y a une erreur grammaticale (erreurs de syntaxe) il faudra la corriger avant de convertir au format binaire. 
si tout est ok , on aura un fichier binaire aprlé démo.
Pour exécuter lela démo :

$./demo

qui produit le résultat suivant :

Hello, World!

## VARIABLES
___________
 
 EXEMPLE :

 ```C
 #include <stdio.h>
 int main() {
    int a;
    int b;
 } /*Le programme ci-dessus crée deux variables pour réserver 2 emplacements de mémoire avec les nom a et b. J'ai créer ces variables à l'aide  du mot clé int pour spécifier le type e données variable, ce qui signifie que l'on doit stockée des valeurs entières dans ces 2 variables. */
 ```
 ```C
 #include <stdio.h>

 int main() {
    int a, b;
 } /* On peut les stockés de cette façon si les données sont similaires. */
 ```

 
  <span style="color: FF0000">IMPORTANT</span>                                  |
 |----------------------------------------------------|
 * Un nom de variable peut contenir un seul type  de valeur. Par exemple, si la variable a été définie de type int, elle e peut stocker que des nombres entiers.

 * Le langage de programmation C nécessite une création de variable, c'est à dire une  déclaration  avant son utilisation dans notre programme (contrairement à Python!). 

 * on ne peut utiliser qu'une seule fois un nom de variable dans un programme.
 * On peut donner n'importe quel nom à une variable(alphanumérique, majuscule où minuscule).

 * ne pas nommer une variable en commençant par un chiffre.

```C
#include <stdio.h>
int main() {
    int a;
    int b;
     a = 10;
     b = 20;
} /* ici nous avons donné des valeurs aux variables */
```
```C
#include <stdio.h>
int main() {
    int a;
    int b;

    a = 10;
    b = 20;

    printf( "Value of a = %d/n" , a);
    printf( "Value of b = %d/n" , b);
}
    /* où printf( "Value of a = %d and value of b = %d/n" , a, b);
} /* résultats : Value of a = 10 et en dessous : Value of b = 20 */
/* ce qui donnera le même résultat l'un à côté de l'autre */
```
▲ 
## MOTS CLES
___________

## OPERATEURS
____________

## ENONCES DE DECISION
_____________________

## LES BOUCLES
_____________

## NUMEROS
_________

## CARACTERES
____________

## LES TABLEAUX
______________

## CHAINES DE CARACTERES
_______________________

## LES FONCTIONS
_______________
