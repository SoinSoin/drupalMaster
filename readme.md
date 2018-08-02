# The exercice

### L'exercice consiste à vous initier à Drupal 8.

## Architecture

```
|
--- /Template -> vous trouverez mon template
|
|
--- /Drupal 
                |
                |
                --- /web
                            |
                            |
                            --- /theme
                                            |
                                            |
                                            ---/custom


```

Vous allez essentiellement travailler dans le fichier /custom.
/ Themes: 

```
/mytheme
                |
                ---mytheme.libraries.yml
                |
                |
                ---mytheme.info.yml
                |
                |
                ---mytheme.theme ->Preprocess
                |
                |
                ---/css -> votre css 
                |
                |
                --- /js -> votre js
                |
                |
                ---/templates
                |
                |
                ---logo.jpg
```

## Ce dont vous allez avoir besoin

```
- composer require drupal/paragraph
- composer require drupal/devel
```
-> Devel en lui même n'est pas très utile mais il y a dans ce plugin un débugger nommé kint.
-> Paragraphs permet de rassembler du contenu dans l'interface Drupal et de le créer des composants personnalisé. 

## Le but de l'exercice.

Le but de l'exercice est d'aller le plus loin possible, pas de finir. 
Vous aller devoir faire du templating à la drupal pour cela vous allez reprendre le template que vous avez fais ou merge la branche 'templend ' sur la branche sur laquelle vous travaillez.

- La navbar et le footer doivent être géré par Drupal .
    ->je veux pouvoir ajouté des liens dans mon menu ainsi que dans mon footer

- Chaque texte et image vont devenir du contenu drupal c'est à dire plus de contenue en dur dans le html. 
    -> Je veux un paragraphs homepage.
        -> Dans le homepage je veux un paragraphs pour les carreaux et un paragraph pour l'avis en dessous de ces carreaux.
            -> dans ces paragraphs je veux des contenus image et des contenus texte.

- Pour le slide je veux un type de contenue image qui se nommera 'img_slide'
    -> je veux que le lien de l'image soit stocké dans une variable créer dans le preprocess de la page afin de pouvoir l'utiliser dans mon Template. 

- Dans le fichier themes vous allez créer un fichier custom, dans ce fichier custom vous aller créer un fichier /mytheme.

- Vous devrez link vos fichier distant comme le css ou le js dans le mytheme.libraries.yml

- Vous devrez créer vos régions au nombre de trois: header, content, footer dans mytheme.info.yml
