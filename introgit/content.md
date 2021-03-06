class: center, middle

# Introduction à Git:
## Les bases pour contribuer à un projet logiciel libre
### Luc Trudeau
### Maison du logiciel libre
[![Logo ML2](https://raw.githubusercontent.com/luctrudeau/Workshops/master/introgit/images/LogoML2.png)](https://maisonlogiciellibre.org/)

<a href="https://github.com/luctrudeau/Workshops/"><img style="position: absolute; top: 0; right: 0; border: 0;" src="https://camo.githubusercontent.com/365986a132ccd6a44c23a9169022c0b5c890c387/68747470733a2f2f73332e616d617a6f6e6177732e636f6d2f6769746875622f726962626f6e732f666f726b6d655f72696768745f7265645f6161303030302e706e67" alt="Fork me on GitHub" data-canonical-src="https://s3.amazonaws.com/github/ribbons/forkme_right_red_aa0000.png"></a>

[![Creative Commons License](https://i.creativecommons.org/l/by-sa/4.0/88x31.png)](http://creativecommons.org/licenses/by-sa/4.0/)
---
class: middle, center

# Vous désirez faire un changement à un projet logiciel libre

[![xkcd.com](http://imgs.xkcd.com/comics/duty_calls.png)](https://xkcd.com/386/)

Ref: Duty Calls - Randall Munroe

---
class: middle, center

# Cependant, le projet utilise Git
## fork, clone, branch, commit, merge, rebase...  
![Run away!](https://raw.githubusercontent.com/luctrudeau/Workshops/master/introgit/images/runaway.gif)

---

# Ce guide est pour vous!
## Nous allons introduire les concepts de bases pour vous permettre:

 * De Créer votre fourche
 * D'obtenir un dépôt Git
 * De Créer une branche pour notre nouvelle fonctionnalité
 * D'indexer les fichiers modifiés
 * De valider les modifications
 * De contribuer au projet

---

# Étape 1: Créer votre fourche

## Historiquement, la fourche (fork) à une connotation négative

## Dans le cas de Git, c'est une bonne chose!

### Sur GitHub, c'est facile de faire un fork: ouvrez la page du projet et clickez sur "Fork"
![GitHub Fork](Bootcamp-Fork.png)

### Note: La raison pourquoi nous forkons le projet est pour nous assurer que nous avons les droits pour interagir avec le dossier.

---

# Étape 2: Obtenir un dépôt Git

### Sur Github, c'est facile d'obtenir le lien
![Fork URL](https://raw.githubusercontent.com/luctrudeau/Workshops/master/introgit/images/Fork-URL.png)

### Avec ce URL, on peut faire le clone
```
git clone https://github.com/luctrudeau/Workshops.git
```
### Cette commande va cloner votre fork localement sur votre machine. Entrons dans ce dossier.
```
cd Workshops
```

---

# Étape 3: Créer une branche pour notre nouvelle fonctionnalité

### Nous désirons refaire cette slide, notre branch s'appellera _BranchSlideRefactoring_
```
git checkout -b BranchSlideRefactoring
```
### L'avantage d'utiliser checkout -b est que nous entrons dans la branch automatiquement.
### Nous sommes maintenant dans la branch _BranchSlideRefactoring_

---

# Étape 4: Indexer les fichiers modifiés

## Suite à votre modification, il faut ajouter ce fichier pour qu'il soit inclus dans notre prochain commit

```
git add introgit/content.md
```

![Git Lifecycle](https://raw.githubusercontent.com/luctrudeau/Workshops/master/introgit/images/lifecycle.png)

---

# Étape 5: Effectuez votre commit

## La commande commit nous permet de faire l'équivalent d'un snapshot de ce que nous avons indexé
```
git commit
```
## Suite à cette commande, votre éditeur sera ouvert. Vous devrez y entrer une description du commit

### Une description de commit doit contenir:
* Un titre comme première ligne
* Un description du raisonnement derrière la modification contenu de ce commit

#Attention ce commit est local (uniquement sur votre machine)

---

#Étape 6: Effectuez un push

## Utilisez la commande pour envoyer votre commit

---

# Étape 7: Demandez un pull request
## Sur la page de votre fork, vous pouvez maintenant créer un pull request à l'aide du bouton "Create Pull Request"

## Vous devez maintenant choisir la branche sur le projet original qui va tirer sur la branche dans votre fork.
![Pull Request](https://raw.githubusercontent.com/luctrudeau/Workshops/master/introgit/images/PullRequest.png)

## Par la suite, vous devez inclure un titre et une description à votre pull request
![Pull Request Descripiton](https://raw.githubusercontent.com/luctrudeau/Workshops/master/introgit/images/PullRequestDescription.png)

