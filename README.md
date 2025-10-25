# CharPy

Prononc. et Orth. : [ʃaʀpi]. Filaments obtenus à partir de vieux linge par effilage ou râpage et servant à faire des pansements. Au fig., fam. [En parlant d'une pers. ou d'un aspect de la pers.] Mettre qqn en charpie. S'acharner sur quelqu'un au point de l'anéantir.

C'est peut-être ce qu'ont malheureusement ressenti des camarades durant les premières heures du master d'Humanités numériques de l'École des chartes. Une fois ce petit temps passé, on peut commencer à s'amuser.

En se basant sur le cours d'Alexandre Lionnet-Rollin (doctorant ENC) et Jean Barré (doctorant ENS), on propose quelques développements de diverses natures. Tant qu'on y est on pique également dans les cours de Théo Moins (postdoc ENC). Le programme est circonscrit et se borne (essentiellement) à des notions afférentes au langage Python ainsi qu'à quelques unes de ses principales bibliothèques (de calcul scientifique, de visualisation, de manipulation de données...). On s'autorise des envolées lyriques et quelques joyeusetés mathématiques. Ce document ne se substitue aucunement à un cours.

L'occasion étant trop belle pour être loupée, nous ne nous limiterons pas à une pure besogne pythonesque. Une fois introduits en bonne et due forme les principaux résultats d'algèbre linéaire, des thèmes autour de la réduction seront proposés. L'objectif n'est (malheureusement) pas de comprendre pourquoi l'ensemble des matrices trigonalisables réelles est fermé (quoique...), de savoir faire des réductions de Jordan en une fraction de seconde voire de pouvoir appréhender sereinement le magnifique _Réduction des endomorphismes_ de Rached Mneimné (qui donc le peut?). On se concentrera surtout sur l'acquisition d'un langage et de réflexes de la vie de tous les jours en algèbre linéaire. L'algèbre linéaire ayant le bon goût de "bien se comporter", presque aucun énoncé ne sera particulièrement difficile à appréhender une fois les bases acquises. De plus, vous ne devez pas être sans savoir ô combien l'algèbre linéaire est déterminante et d'une importance extrême pour faire du machine learning etc. Que de bonnes raisons donc!

Enfin, précisons le explicitement : l'absolue majorité des applications sont résolument tournées vers les humanités numériques.

Bien évidemment, toute personne lisant ces lignes est invitée à rusher les documents et à envoyer aux auteurs le temps nécessaire à l'accomplissement de la mission.

Ce projet a été initialement mené par Charles Planque (HN 2025-2027) et Mathias Garnier (HN 2025-2027). L'aide et les remarques de toute personne intéressée sont évidemment les bienvenues. N'hésitez pas à reprendre ces notes et à les compléter (en particulier en ce qui concerne les projets) !

## Sommaire.
- [Chapitre 0 - Programme](Chapitre%200/Chapitre%200%20-%20Programme.ipynb). Peu ou pas de surprises dans ce chapitre. On explique tout de même comment installer les principaux outils de développements. Le seul intérêt théorique de cette section est de montrer ce que l'on est en droit d'attendre une fois accompli le "_cours_". Cette partie est complétée par la Section 1 du Chapitre 1.
- [Chapitre 1 - _Terra incognita_](Chapitre%201%20-%20Terra%20incognita/). Faisons nos premiers pas en terre inconnue. L'objectif est très clair : se noyer, boire la tasse, perdre ses esprits puis se dire que tout ce qui suit sera très simple.
    - [Section 1 - Projets en pagaille](Chapitre%201%20-%20Terra%20incognita/Section%201%20-%20Projets%20en%20pagaille.ipynb). On s'attarde sur divers projets d'humanités numériques, mais pas que!
    - [Section 2 - 50 nuances de Python]() car même Python peut avoir du charme.
    - [Section 3 - Aperçus mathématiques](). Question absolument typique du voisin du dessous (X 1958) : "Comment se portent les mathématiques aujourd'hui ?" Très bien ! C'est ce que nous allons voir.
- [Chapitre 2 - Manipulations de données intégrées (built-in)]().
    - [Section 1 - Algèbre booléenne](). Aux commencements furent le $0$ et le $1$. 
    - [Section 2 - Nombres en tout genre](). Comme le demande si bien Patrick Popescu-Pampu, [qu'est-ce que le genre](https://www.cmls.polytechnique.fr/xups/xups11-03.pdf) ? C'est un nombre ! La boucle est bouclée. 
    - [Section 3 - Strings](). Premier degré, on peut faire des choses affreusement compliquées en deux temps trois mouvements.
    - [Section 4 - Listes](). Les strings sont des listes mais les listes sont beaucoup plus que des strings!
    - [Section 5 - Structures de données](). Les listes ne sont qu'une porte d'entrée vers ce que l'on appelle les _containers_.
    - [Section 6 - L'attaque des fichiers](). Aucune grande difficulté mais de bonnes pratiques sont tout de même à prendre. On en profite pour présenter le système I/O.
    - [Section 7 - Fonctions](). Juste la chose la plus importante.
    - [Section 8 - Apprendre à lire les erreurs](). Et comment y remédier!
- [Chapitre 3 - AI as IF](). L'IA n'est-t-elle qu'une concaténation sans fin de "si ... alors ..." ? Pas vraiment!
    - [Section 1 - _Control flows_](). _L'obligation est conditionnelle lorsqu'on la fait dépendre d'un événement futur et incertain, soit en la suspendant jusqu'à ce que l'événement arrive, soit en la résiliant, selon que l'événement arrivera ou n'arrivera pas._ Article 1168 du code civil.
    - [Section 2 - _How do I stop yelling?_]() Nulle exception à la règle, sauf celles que nous avons prévues ou celles qui nous tombent dessus!
    - [Section 3 - Sucre syntaxique](). En écrivant peu on peut en dire beaucoup.
    - [Section 4 - Le style alpin](). En n'autorisant qu'un nombre limité et élementaire d'opérations, gravissons quelques sommets.
- [Chapitre 4 - Premières objections](). Découverte du monde de la programmation orienté objet.
    - [Section 1 - De l'organisation du code à sa rationalisation](). Des modules aux classes nous allons voir deux manières d'organiser son code, l'une plutôt formelle, l'autre surtout fonctionnelle.
    - [Section 2 - Lutte des classes](). cavalier.attaquer(). cavalierAdverse.riposter().
    - [Section 3 - Héritages](). _Les successions s'ouvrent par la mort, au dernier domicile du défunt._ Article 720 du code civil. Fort heureusement, ce n'est pas l'unique moyen en Python !
    - [Section 4 - Revenir sur ses acquis](). Il peut parfois être nécessaire de contrôler et modifier le comportement de fonctions (intégrées) d'une classe.
    - [Section 4 - Planter le décor](). L'occasion de voir quelques _design pattern_ dont l'éminent _Decorator pattern_.
    - [Section 5 - Zoom sur l'abstraction](). from abc import ABC.
    - [Section 6 - Se faire beau](). Les décorateurs... ce n'est pas vraiment de l'orienté objet. Mais comme on vient de parler d'abstraction et qu'on est en fin de chapitre, pourquoi pas en parler ici?
- [Chapitre 5 - La libraire standard](). Découvrons la en recodant certaines de ses plus fameuses méthodes.
    - TBD
- [Chapitre 6 - NumPy, Pandas, Seaborn...]() Au fond, ce sont tous les mêmes! _Que nenni_ mais il y a tout de même quelques similarités.
    - TBD
- [Chapitre 7 - À la piscine](). Découverte du threading et multiprocessing et (un peu) plus.
    - TBD
- [Chapitre 8 - Tester et documenter](). L'écosystème Python propose des modules clef en main pour cela.
    - TBD
- [Projet - TBD]().
- [Projet - Compression des données et archivage]().
- [Projet - Dinosarium](). Il y a fort longtemps, le [Javaquarium](https://zestedesavoir.com/forums/sujet/447/javaquarium/) était un passage presque obligé pour quiconque souhaitait apprendre le Java. On décline cette exercice à la créature préférée des chartistes : le dinosaure.
- [Projet - Entity Component System](). Le [Dinosarium]() peut être vu comme un premier pas vers ce projet.
- [Projet - Scrap à tout va]().
- [Projet - Petit transpilateur fait maison](). On fait une version propre du transpilateur présenté dans le [Chapitre 1/Section 1](Chapitre%201%20-%20Terra%20incognita/Section%201%20-%20Projets%20en%20pagaille.ipynb)
- [Projet - Argparse]().
- [Projet - Bribes d'analyse textuelle et stylométrie]().
- [Projet - Ah bon ? Le Conseil d'État a dit ça ?]()
- [Projet - Lire entre les lignes](). En opérant une décomposition spectrale d'un document, on peut parfois faire apparaître des textes qui semblaient avoir disparu.
- [Projet - HTR et formules de maths]().
- [Projet - Modélisations de populations et manuscrits](Projets/Projet%20-%20Modélisations%20de%20populations%20et%20manuscrits.ipynb).
- [Pour le beau jeu 1 - Probabilités et chaînes de Markov]().
- [Pour le beau jeu 2 - Éléments de géométrie et d'analyse en grandes dimensions]().
- [Pour le beau jeu 3 - Introduction à la théorie spectrale des graphes](). Pourquoi ? Parce que.



<!-- https://docs.python.org/3/tutorial/datastructures.html
-->