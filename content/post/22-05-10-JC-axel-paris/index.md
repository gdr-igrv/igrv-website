---
title: "Axel Paris : Modélisation et génération de scènes naturelles dans le contexte de l'informatique graphique"
date: 2022-05-10
categories: Jeune chercheur·se
authors: 
    - Rebecca Fribourg
---

### Peux-tu nous dire quelle est ta situation actuelle en matière de recherche ? 

Je suis en 3ème année de thèse au [LIRIS](https://liris.cnrs.fr) à Lyon, encadré par Eric Galin et Eric Guérin de l’équipe [Origami](https://projet.liris.cnrs.fr/origami/). J’ai réalisé une césure de thèse de 6 mois pour faire un stage de recherche dans une entreprise, chez Adobe Research, et je débute pour cela ma troisième année en décalé en Mars. 

### Peux-tu nous décrire en quelques mots, et de manière accessible aux membres du GDR-IGRV, en quoi tes travaux de recherche consistent exactement? 

Ma thèse porte sur la modélisation et la généralisation de phénomènes naturels. Concrètement sur les phénomènes naturels, on imagine une scène d’extérieur, naturelle, composée, en général, d'un terrain, de la végétation, des fluides (e.g. des rivières, des nuages), et je m’intéresse à la génération de terrains réalistes. Il s’agit donc de reproduire ce qu’on appelle des « modelés », des « formes de terrains » qu’on voit dans la vraie vie, par des algorithmes, par des simulations d’érosion, etc. 

Plus spécifiquement, je m’intéresse aux phénomènes naturels qu’on nomme « tridimensionnels » : les phénomènes volumiques qui ne peuvent pas être représentés uniquement par une surface lisse. Je m’intéresse aux concavités, comme les grottes, les surplombs, les arches, etc. et donc à leur génération. 

Ça a deux applications principalement : une application plutôt dans l’industrie du loisir, notamment le cinéma et le jeu vidéo, où souvent on veut créer des scènes naturelles par ordinateur (e.g. le dernier Avengers). Dans ces scènes naturelles, il y a souvent un terrain et se sont des artistes qui vont le créer et le texturer. C’est un processus de moins en moins manuel : il est semi-manuel, et beaucoup d’algorithmes sont déjà utilisés par des artistes pour commencer à faire le sketching, placer les formes, etc. Dans ce contexte, on va donc chercher à faire des applications qui donnent plutôt du contrôle aux artistes. La deuxième application est à l’interface entre la géologie et l’informatique. Imaginons qu’on regarde une chaîne de montagnes et qu’on veuille savoir comment elle a été formée. On va essayer de rétro-ingéniérer les processus par des algorithmes pour comprendre comment la montagne s’est formée, et ça peut nous aider à prédire l’évolution de la montagne avec des « méthodes inverses ». 

{{< figure src="SeaErosion03.jpg" caption="Simulation de terrains volumiques par invasion-percolation">}}

#### Est-ce que côté technologie tu arriverais à décrire un peu les outils que tu utilises ?

Dans ma thèse, je me suis focalisé principalement sur les modèles à base de surfaces implicites. Très succinctement, c’est une représentation très compacte de formes géométriques. On ne les représente non pas comme des maillages, mais comme des équations (des équations de distance à la forme), et ça prend très peu de place en mémoire.  On peut représenter de très grandes scènes avec ça! Ca a aussi d’autres avantages au niveau contrôle : il y a des opérateurs de mélange, on peut mélanger des formes (très utile pour les artistes). C’est un modèle très expressif. Dans le cadre de ma thèse, il s’agit de regarder tout ce qu’il est possible de faire avec les surfaces implicites pour les phénomènes naturels. J’ai aussi travaillé sur les modèles 2D de cartes de hauteur.

### Quel est ton résultat de recherche dont tu es le plus fier? 

J’ai eu l’occasion de travailler dans ma thèse sur des sujets assez différents qui m’ont tous beaucoup plu. Si je devais revenir sur juste un, je dirais le dernier qui concernait la génération de réseaux de grottes. Je l’ai trouvé particulièrement intéressant car on a pu collaborer avec quelqu’un de l’extérieur, une géologue, qui avait des connaissances que nous n’avions pas du tout (Pauline Colon, de l’université de Lorraine). Elle nous a apporté beaucoup de connaissances en géologie et en géomorphologie. On a rédigé un article ensemble où le côté pluridisciplinaire ressort beaucoup, et chacun a apporté des connaissances à l’autre. La collaboration continue d’ailleurs avec des stages en suite de ce papier. 

{{< figure src="nabkha_1.png" caption="Simulation de paysages désertiques: Dunes Nabkha">}}


### Quelles sont tes perspectives à long terme ? (Après la thèse ou le post-doc, EC, CR..)

Ça n'est pas simple… j’ai pleins d’idées ! Disons que rien ne me semble “pas attractif”, même si j’ai quelques préférences. Si je devais choisir maintenant, je m’orienterais dans la recherche d’un post-doc à l’étranger dans une équipe qui fait des choses en lien avec ce que je fais .. ou pas .. j’aime aussi l’idée de changer un peu. Mes projets à plus long terme demandent encore à se préciser. Ma césure en entreprise m’a permis de tester à la fois le privé et le public, et je vois que les deux ont des avantages et des inconvénients, je me laisse donc encore du temps pour réfléchir.  

### Quelles sont les recherches/expériences/thématiques que tu rêverais d'aborder dans ton laboratoire idéal ?

Bonne question… ! Suite à mes derniers travaux en collaboration avec une géologue, j’ai compris l’enjeu et bénéfice de la dimension pluridisciplinaire que peut prendre la recherche, et j’aimerais beaucoup pouvoir retrouver cela dans un futur laboratoire. 


*Toutes les illustrations de cet article ont été fournies par Axel et le détail de ses travaux est disponible sur [son site web](https://aparis69.github.io/).*
