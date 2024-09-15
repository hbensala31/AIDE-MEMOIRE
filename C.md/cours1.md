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
* Déclarer une variable
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

 * Un nom de variable peut contenir un seul type  de valeur. Par exemple, si la variable a été définie de type int, elle ne  peut stocker que des nombres entiers.

 * Le langage de programmation C nécessite une création de variable, c'est à dire une  déclaration  avant son utilisation dans notre programme (contrairement à Python!). 

 * on ne peut utiliser qu'une seule fois un nom de variable dans un programme.
 * On peut donner n'importe quel nom à une variable(alphanumérique, majuscule où minuscule).

 * ne pas nommer une variable en commençant par un chiffre.
 * ne pas nommer avec un des mots clés.

```C
* stocker des données dans une variable
#include <stdio.h>
int main() {
    int a;
    int b;
     a = 10;
     b = 20;
} /* ici nous avons donné des valeurs aux variables */
```
```C
* accèder aux valeurs stockées dans une variable
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

 MOTS CLES DE PROGRAMMATION C RESERVES 

|Nom	   |Description	                                                                                        |
|----------|----------------------------------------------------------------------------------------------------|
|asm	   |Ce mot réservé permet d'inclure du code assembleur directement dans le code source C.|
|auto	   |Ce mot réservé permet d'indiquer un spécificateur d'entreposage de classe.|
|break	   |Ce mot réservé permet d'interrompre une boucle ou une instruction «switch».	
|case	   |Ce mot réservé permet d'identifier un cas dans un mot réservé «switch».	
|cdecl	   |Ce mot réservé permet d'indiquer une déclaration avec un appel de convention C.	
|char	   |Ce mot réservé identifie le type de données de caractère.	
|const	   |Ce mot réservé permet de définir une constante.	
|continue  |Ce mot réservé permet de recommencer au début d'une boucle.	
|default   |Ce mot réservé permet d'exécuter un cas par défaut si les autres ne sont pas correspondant dans un mot réservé «switch».	
|do	       |Ce mot réservé permet d'effectuer une boucle avec un mot réservé «while».
|double	   |Ce mot réservé identifie le type de données réel de double précision.	
|else      |Ce mot réservé permet d'effectuer une situation contraire à la condition «if».
|enum	   |Ce mot réservé permet d'identifier un type de données d'énumération.
|extern	   |Ce mot réservé permet de déclarer une méthode externe comme par exemple lorsqu'on définit une API de Windows.
|far	   |Ce mot réservé d'indiquer une porter longue.	 
|float	   |Ce mot réservé permet d'identifier le type de données de «float».
|for	   |Ce mot réservé permet d'effectuer un compteur de boucle.
|goto	   |Ce mot réservé permet de faire un saut d'exécution à une étiquette.
|huge	   |Ce mot réservé permet d'indiquer une porté global.	 
|if	       |Ce mot réservé permet d'effectuer le traitement d'une condition.
|inline	   |Ce mot réservé permet d'indiquer qu'il faut que le compilateur élargisse la fonction en ligne au moment de l'appel de la fonction ou d'un membre de fonctions
|int	   |Ce mot réservé identifie le type de données d'entier.
|interrupt |Ce mot réservé permet d'indiquer que la fonction est une interruption.
|long	   |Ce mot réservé identifie le type de données d'entier long.
|near	   |Ce mot réservé permet d'indiquer une porté proche.	 
|pascal	   |Ce mot réservé permet d'indiquer que les appels sont compilés selon le format du langage de programmation Pascal.	 
|register  |Ce mot réservé permet d'indiquer qu'il faut utiliser autant que possible les registres du microprocesseur pour contenir le contenu d'une variable ou d'un paramètre.
|restrict  |Ce mot réservé permet d'indiquer une déclaration de fonction ou de définition n'envoyant pas un type de format pointeur, ainsi le compilateur retournera un objet n'étant pas un alias mais avec tous les pointeurs des autres.
|return	   |Ce mot réservé permet de terminer une fonction avec une valeur optionnelle.	
|short	   |Ce mot réservé identifie le type de données d'entier court.
|signed	   |Ce mot réservé permet d'indiquer que le type de données est entier, donc qu'il support les nombres négatif.
|sizeof	   |Ce mot réservé permet d'indiquer la taille d'un objet, d'une variable ou d'un type de données.
|static	   |Ce mot réservé permet de rendre disponible une fonction ou variable d'une classe de façon global comme si elle se trouvait en dehors de la classe elle-même.
|struct	   |Ce mot réservé permet d'identifier une structure de données (un enregistrement).	
|switch	   |Ce mot réservé permet d'effectuer des testes de cas.	
|typedef   |Ce mot réservé permet de définir un type de données.	
|union	   |Ce mot réservé permet de définir des champs avec la même position de déplacement dans une structure, donc qu'y se superpose.	
|unsigned  |Ce mot réservé permet d'indiquer que le type de données ne contient pas de partie négatif, que c'est n'est pas un nombre entier mais un nombre naturel.	
|void	   |Ce mot réservé permet de définir un type n'ayant aucun type.	
|volatile  |Ce mot réservé permet d'indiquer que la variable ne doit pas changer d'ordre de place en mémoire après la compilation.	
|while	   |Ce mot réservé permet de définir une boucle.	
|Bool	   |Ce mot réservé identifie le type de données booléen pouvant être 0 ou 1.	
|Complex   |Ce mot réservé identifie le type de données d'un nombre complexe.	
|Imaginary |Ce mot réservé identifie le type de données d'un nombre imaginaire.	

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
