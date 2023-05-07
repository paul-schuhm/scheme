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


## Références

- [Site officiel de Scheme (sur gnu.org)](https://www.gnu.org/software/mit-scheme/)
- [Documentation officielle de Scheme (une page)](https://www.gnu.org/software/mit-scheme/documentation/stable/mit-scheme-ref.html#Acknowledgements)
- [Structure and interpretation of computer programs, 2nd edition (version HTML)](https://mitp-content-server.mit.edu/books/content/sectbyfn/books_pres_0/6515/sicp.zip/full-text/book/book.html), l'édition web gratuite et complète du très grand livre d'Abelson, Gerald Jay et Julie Sussman (MIT Press, 1996). `Recommandé`
- [Introduction aux fonctions en Scheme](https://www.shido.info/lisp/scheme4_e.html), un extrait d'un autre bon tutoriel sur le web sur Scheme
- [Interpréteur Scheme en ligne](https://inst.eecs.berkeley.edu/~cs61a/fa14/assets/interpreter/scheme.html), un interpréteur Scheme mis sur le web par l'université de Berkeley. Pratique pour tester sans installer
- [Why Scheme ?](https://www.shido.info/lisp/scheme1_e.html)
- [Installation sur macOS: Homebrew Scheme](https://formulae.brew.sh/formula/mit-scheme), page d'intallation de Scheme sous macOS via le gestionnaire de paquets Homebrew
- [Installation sur GNU/Linux](https://www.gnu.org/software/mit-scheme/), installation de Scheme sous GNU/Linux
