TP Formation Git
================

## Github
- Créer un compte https://github.com/join
- Obtenir un compte Github Developer **gratuit au lieu de 7€ par mois** : https://education.github.com/pack

## Installation

### Sur Windows
Allez sur https://git-scm.com/download/win

### Sur OS X:
- Si vous avez Xcode, git est déjà installé
- Si vous avez Homebrew, `brew install git`
- Sinon, téléchargez Git ici : https://git-scm.com/download/mac

### Sur Linux (Ubuntu/Debian)
``` bash
$ sudo apt-get install git
```

## Sujet

### 0. Configurer Git

``` bash
git config --global user.email moi@eleves.enpc.fr
git config --global user.name "Prénom Nom"
git config --global push.default simple
```

Forker le répo en cliquant ![ici](https://github.com/KIClubinfo/formation-git-exemple/fork)

### 1. Cloner le dépôt
``` bash
# Retourner dans son répertoire utilisateur
cd ~
# Cloner le dépot d'exemple
git clone https://github.com/MonNomDUtilisateurGithub/formation-git-exemple.git
# Aller dans le dossier
cd formation-git-exemple
```

### 2. Ajouter un fichier
``` bash
# Créer un nouveau fichier, par exemple
echo "Mon animal préféré est le caribou" >> secret.txt
# Git est conscient qu'un nouveau fichier a été créé
git status
# Dire à Git de suivre le nouveau fichier locations.txt
git add secret.txt
```

![Ajouter un fichier](https://www.atlassian.com/dam/jcr:dbf0c59f-848d-4814-bfd5-6b190a092963/03.svg)


``` bash
# Comparer. Le fichier a été ajouté à la staging area et est prêt à être commité
git status
# Commiter le fichier
git commit -m 'Initial commit'
```

![Commiter](https://www.atlassian.com/dam/jcr:d5f60ca0-b606-4e7c-b3a2-430165bc0672/04.svg)

Jusqu'à présent, tout ce que vous avez fait est sur votre système local et invisible pour les autres jusqu'à ce que vous poussiez ces modifications.

``` bash
# Pousser le nouveau commit
git push
```
