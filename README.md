# IGRV website

[https://gdr-igrv.github.io/igrv-website/](https://gdr-igrv.github.io/igrv-website/)

## HowTo

* Ajouter un évènement : dupliquer repertoire `event/example`, editer/completer `index.md` (+ image `featured.png`)

* Ajouter une brève : dupliquer repertoire `event/21-07-20-gtmg-gazette` par exemple, editer/completer `index.md` (+ image `featured.png`)

* Modifier une page : editer le `index.md` dans le bon repertoire

* Modifier le menu : `config/_default/menus.yaml`

* Ajouter un auteur : cf `authors/`

* Modifier la frontpage: cf `home/`

* Tester des modifcations en local : à la racine du projet `hugo serve` (et ensuite cela précise une URL du type "https://localhost..."). Hugo va relancer le build à chaque fois qu'un fichier est modifié en local

* Publier une modification : ajouter les fichiers (`git add ...`), faites un commit et un push sur le projet github. Si vous n'avez pas les droits de push sur le compte gdr-igrv, passez par un pull-request.


## Documentation

* [Doc wowchemy](https://wowchemy.com/docs/)

* [Syntaxe markdown et elements de la page](https://wowchemy.com/docs/content/writing-markdown-latex)
