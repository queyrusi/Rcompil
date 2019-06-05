Features
-------------
- Parsing et pretty printing de scripts classiques de code R


Liens
-------------
github perso @queyrusi

Compilateur pour language R
=============
**Table of Contents**

[TOCM]

[TOC]

Syntaxe gérée
-------------

- Les assignations se font avec `<-`
- La possibilité d'écrire une expression directement dans le programme sans
mise en forme préalable, cela permet d'afficher le résultat sans fonction.
- Dans l'EBNF, les objets __Function__ et __Arg__ ont été ajoutés pour répondre au problème
des définitions de fonctions.
- On peut définir des fonctions avec le mot-clé `function`, avec autant d'arguments
qu'on le souhaite.

EBNF
-------------

Syntaxes non gérées
-------------

Contenu du paquet
-------------
**Classes**
- La racine comprend le main ainsi qu'un script d'exemples de code R compilable. Le module d'origine indent a été laissé dans la racine.

| Paquet  | Classes  | Description |
| :------------ |:---------------:| -----:|
| imports      | `Lexer` `Parser` `Token`      |   Classes de H. Boenning adaptées |
| VisitorPattern      |`Element` `Visitor` | Pattern visiteur |
| AST | `Ast` `Node`      |   Implémentent l'élément. Un AST est un nœud |
| prettyPrinter | `PrettyPrinter`       |    Implémente le visiteur |

**Arborescence**
![alt text]("file:///arbo")

**Paquet tiers utilisé**

Nous utilisons termcolor pour la coloration en terminal

`$ conda install termcolor`
