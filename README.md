# scheme

## Installation

### Sur Debian/Ubuntu

~~~
sudo apt install mit-scheme
~~~

## Lancer l'interpréteur Scheme

Scheme est un langage interprété, comme Python ou PHP. Pour executer du code Scheme, vous pouvez accéder à un interpréteur interactif en ligne de commande. Dans un terminal

~~~
mit-scheme
1 ]=>
~~~

## Premiers pas sur l'interpréteur

Pour accéder au manuel de l'interpréteur `control+c ?` (taper `control` et `c` en même temps, puis `?`). Pour revenir au REP, `control+x`. Pour quitter l'interpréteur, tapez `control+c Q`.

L'interpréteur fonctionne toujours de la même manière: il lit l'expression que vous avez tapé dans le terminal (read), évalue l'expression (eval) et affiche le résutlat (print). On appelle cela la *read-eval-print loop* (Read Eval Print ou REP). Lorsque vous accéder à l'interpréteur, le prompt `1 ]=>` indique que vous êtes dans le REP de niveau 1. Pour nettoyer l'écran, `control+c control+l`.

Dans le REP tapez `(+ 1 2)` puis `entrée`. L'expression `(+ 1 2)` est lue par l'interpréteur (*read*), évaluée à 3 (*eval*) puis imprimée sur la sortie standard (*print*).

~~~
1 ]=> (+ 1 2)

;Value: 3
~~~

On remarque que le résultat affiché `;Value: 3` est écrit sous forme de commentaire. Un commentaire en Scheme est défini par le caractère `;`.

## Concepts fondamentaux

Tout programme repose sur 3 ingrédients : 

- des *expressions primitives* : fournies par le langage, ce sont les expressions les plus simples, comme la représentation du nombre `42` ou la chaîne de caractères `"foobar"`
- des *moyens de combinaison* pour combiner des éléments simples afin d'en fabriquer des plus complexes
- des *moyens d'abstraction* pour nommer, penser et manipuler les combinaisons comme des modules ou boîtes noires

Par exemple si vous tapez `42` dans l'interpréteur, le REP vous affiche `42`. En effet, `42` est évalué à `42`. Scheme vous met à disposition des procédures (ou fonctions) primitives comme l'addition (+), la soustraction (-), la multiplication (*) et la division (/)

>Et bien d'autres, on y reviendra plus tard.

L'expression `(+ 1 2)` est une liste. Une liste est délimitée par des parenthèses. 

>La syntaxe de Scheme est simple. Elle s'apprend en quelques minutes. La difficulté c'est que les parenthèses jouent plusieurs rôles (on dit que leur sémantique est surchargée) ce qui peut prêter à confusion au départ. 

Lisp veut dire *__lis__t __p__rocessing*, car tout y est traitement de listes ! Le premier élément de la liste est appelée l'opérateur, `+` ici. Le reste des éléments sont les *opérandes*. La liste `(+ 1 2)` peut se traduire par "applique la procédure `+` aux éléments `1` et `2`". Les parenthèses se traduisent par *l'application d'un opérateur à des éléments*, et indique à l'interpréteur d'évaluer cette application. L'expression `(+ 1 2)` est lue (*read*), l'interpréteur voit les parenthèses et applique donc `+` à `1` et `2` (*eval*) et affiche `3`. 

> Si vous tapez `+ 1 2` sans parenthèses, Scheme va évaluer chaque expression séparemment. 



## Références

- [Site officiel de Scheme (sur gnu.org)](https://www.gnu.org/software/mit-scheme/)
- [Documentation officielle de Scheme (une page)](https://www.gnu.org/software/mit-scheme/documentation/stable/mit-scheme-ref.html#Acknowledgements)
- [Structure and interpretation of computer programs, 2nd edition (version HTML)](https://mitp-content-server.mit.edu/books/content/sectbyfn/books_pres_0/6515/sicp.zip/full-text/book/book.html), l'édition web gratuite et complète du très grand livre d'Abelson, Gerald Jay et Julie Sussman (MIT Press, 1996). `Recommandé`
- [Introduction aux fonctions en Scheme](https://www.shido.info/lisp/scheme4_e.html), un extrait d'un autre bon tutoriel sur le web sur Scheme
- [Interpréteur Scheme en ligne](https://inst.eecs.berkeley.edu/~cs61a/fa14/assets/interpreter/scheme.html), un interpréteur Scheme mis sur le web par l'université de Berkeley. Pratique pour tester sans installer
- [Why Scheme ?](https://www.shido.info/lisp/scheme1_e.html)
- [Installation sur macOS: Homebrew Scheme](https://formulae.brew.sh/formula/mit-scheme), page d'intallation de Scheme sous macOS via le gestionnaire de paquets Homebrew
- [Installation sur GNU/Linux](https://www.gnu.org/software/mit-scheme/), installation de Scheme sous GNU/Linux
