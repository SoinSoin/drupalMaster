#The exercice

###L'exercice consiste à vous initier à Drupal 8.

##Architecture

```
|
--- /Template -> vous trouverez mon template
|
|
--- /Drupal |
                     |
                     |
                     --- /web|
                                    |
                                    |
                                    --- /theme|

```

Vous allez essentiellement travailler dans le fichier theme.

/ Themes: 

```
/nameTheme|
                          |
                          ---nameTheme.libraries.yml
                          |
                          |
                          ---nameTheme.info.yml
                          |
                          |
                          ---nameTheme.theme ->Preprocess
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

