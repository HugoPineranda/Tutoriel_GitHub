# **Guide d'utilisation de GitHub**

## **_Sommaire:_**
#### [1. Introduction à GitHub](#intro)
#### [2. Utilisation via la plateforme GitHub.com](#github)
    - Créer un dépôt
    - Le Fork
    - Ajouter/créer un fichier
    - Créer une branche
    - Effectuer des modifications sur un fichier et les répertorier (Commit)
    - Effectuer une requête d'application des modifications (Pull Request)
    - Appliquer les modifications (Merge)
#### [3. Utilisation en local via Git](#git)
    - Créer un dépôt local
    - Cloner un dépôt depuis GitHub sur votre machin
    - Connecter le dépôt local et le dépôt GitHub
    - Cas d'une liaison avec un fork
    - Envoi de fichiers
    - Réception de fichiers
    - Créer et manipuler des branches
    - Fusionner deux branches (Merge)
    - Modifier localement un fichier

---

## <a id="intro" style="text-decoration:none">**1. Introduction à GitHub et Git**</a>
>*Qu'est-ce que GitHub ?*

**GitHub** est le plus grand espace de stockage de travaux collaboratifs au monde. C'est un service en ligne d'hébergement de **repositories**. Il permet la communication facile entre les développeurs et le partage de code.

Il fonctionne avec le logiciel de gestion de versions décentralisées **Git**, développé par Linus Torvald, auteur du noyau Linux.  

>*Pourquoi utiliser GitHub ?*

Le principal atout est le **contrôle de version**. Si deux personnes travaillent sur le même fichier, il est impossible que leurs données soient perdues. En effet, Git effectue une sauvegarde de chaque modification effectuée. Il est ainsi possible de revenir à une version précedente du produit ou code.

**GitHub** a l'avantage d'être simple à prendre en main, même sans connaissances préalables en programmation. De plus, les utilisateurs conservent 100% de la propriété des projets déposés.

L'avantage de **GitHub** par rapport à **Git** est l'interface visuelle qui est beaucoup plus intuitive; en effet l'utilisation de Git nécessite de passer par un invité de commande type CMD ou, **Git Bash**.

---

## <a id="github" style="text-decoration:none">**2. Utilisation via la plateforme GitHub.com** </a>


### ***Créer un dépôt:***

* Rendez vous su Github.com. Après avoir créé votre compte, Cliquez sur le + en haut à droite, puis sur ***"New Repository"*** .

    <img src="https://github.com/HugoPineranda/Tutoriel_GitHub/blob/master/images/newRepository.png" height="20%" width="20%">
* Nommez votre dépôt et ajoutez lui une description.
* Sélectionnez ***"Initialize this repository with a README"*** , sauf si vous importez un dépôt déjà existant, puis cliquez sur ***"Create repository"*** .

    <img src="https://github.com/HugoPineranda/Tutoriel_GitHub/blob/master/images/newRepository2.JPG" height="40%" width="40%">

Notre dépôt a été créé et contient un fichier, ***"Readme&#46;md"*** .

---
### ***Le Fork:*** ###

Le ***fork*** est une technique de copie de dépôts, différente du clonage, permettant de copier le dépôt d'un autre utilisateur **GitHub** sur votre propre compte, afin de pouvoir travailler dessus sans influer sur le dépôt situé sur son compte.

* Pour ***forker*** un dépôt, il suffit de cliquer sur le bouton ***fork*** situé en haut à droite de la fenêtre GitHub.<br>

    <img src="https://github.com/HugoPineranda/Tutoriel_GitHub/blob/master/images/fork.JPG" height="40%" width="40%">
    
**Exemple:** Nous voulons créer une copie du dépôt ***"intro to open-source"*** créé par le compte **p-society**, sur notre compte. L'URL du dépôt est "https://github.com/p-society/intro-to-open-source-2017"<br>

En créant un **fork** du dépôt, nous l'avons récupéré sur notre compte sous l'URL "https://github.com/VotreNomUtilisateur/intro-to-open-source-2017"<br>

Modifier le dépôt n'entraînera pas de modifications sur le dépôt du compte original, à moins d'effectuer une requête.

---
### ***Ajouter/créer un fichier:***

Vous avez la possibilité d'uploader un fichier dans votre dépôt ou bien de le créer via l'éditeur **GitHub:**

<img src="https://github.com/HugoPineranda/Tutoriel_GitHub/blob/master/images/edit.JPG" height="40%" width="40%">
* Si vous voulez créer un dossier, ajoutez son emplacement lors de la création du fichier et finisses par un `/`. GitHub le détectera automatiquement et le créera.

   <img src=https://github.com/HugoPineranda/Tutoriel_GitHub/blob/master/images/sousDossier.JPG height="40%" width="40%">
* Vous pouvez réaliser cette action autant de fois que nécessaire, mais votre dossier ne sera pas créé s'il est vide. Vous devez y ajouter un fichier.

---
### ***Créer une branche:***

Par défaut, le projet "définitif" sera enregistré dans la branche ***master***.

La création de branches permet de travailler sur différentes versions d'un dépôt en même temps. On travaille sur une branche, on l'édite, puis on applique (ou non) à la branche ***master*** les modifications réalisées.

Il est fortement recommandé de toujours travailler sur une autre branche que ***master***, et ensuite de fusionner les deux branches.

Pour créer une branche à partir de la branche ***master*** :

* Allez dans votre **dépôt** GitHub
* Cliquez sur le menu dropdown ***"Branch: master"*** .
* Entrez le nom de votre nouvelle branche. Il est fortement conseillé de choisir un nom explicite. Dans cette exemple, nous modifierons le fichier ***"Readme&#46;md"*** , on appellera donc la branche ***"Readme-edits"*** . Cliquez ensuite sur ***"Create branch"*** .
   
   <img src="https://github.com/HugoPineranda/Tutoriel_GitHub/blob/master/images/createBranch.JPG" height="30%" width="30%">
* Vous êtes maintenant dans la branche ***Readme-edits***. Toute modification apportée aux fichiers via GitHub sera appliquée uniquement dans cette branche.
* Pour changer de branche, retournez dans le dropdown menu et sélectionnez une autre branche.

---
### ***Effectuer des modifications sur un fichier et les répertorier :***

* On continuera avec l'exemple de la modification du fichier ***"Readme&#46;md"*** .
* Dans votre branche ***Readme-edits***, cliquez sur le fichier ***"Readme&#46;md"*** , puis sur le bouton ***"Edit this file"*** symbolisé par un crayon :

   <img src="https://github.com/HugoPineranda/Tutoriel_GitHub/blob/master/images/editFile.png" height="40%" width="40%">
* Effectuez vos modifications. Dans cet exemple, le fichier contient 2 lignes générées à partir du nom du dépôt. Nous allons rajouter une seconde ligne "Tutoriel d'utilisation de GitHub" et supprimer la première ligne :

    <img src="https://github.com/HugoPineranda/Tutoriel_GitHub/blob/master/images/ligne2.JPG" height="40%" width="40%">
* Dans la fenêtre  ***"Commit Changes"*** , donnez un titre  et une description à votre modification. Cette étape, le **Commit**, est très importante car elle apparaîtra sur **GitHub** et permet le suivi des différentes modifications apportées à un fichier.
* Vous avez ensuite le choix: enregistrer les modifications sur la branche en cours, ou créer une nouvelle branche et faire une ***pull request*** que nous verrons plus tard.
* Cliquez ensuite sur **"Commit Changes"** .

    <img src="https://github.com/HugoPineranda/Tutoriel_GitHub/blob/master/images/commitChanges.JPG" height="40%" width="40%">
* On remarquera que le ***Commit*** apparaît dans votre branche ***Readme-edits***, avec l'utilisateur et la date de modification.

    <img src="https://github.com/HugoPineranda/Tutoriel_GitHub/blob/master/images/notifCommit.JPG" height="80%" width="80%">
* Par contre, si vous allez dans la branche ***master***, les modifications n'ont pas été appliquées. Pour cela, il faut faire une ***pull request***.

---
### ***Effectuer une requête d'application des modifications (Pull Request) :***

* ***Pull Request*** est une requête d'application des modifications appliquées à une branche dans une autre. Elle permet aussi de voir les différences entre deux branches en les comparant. Ici, on appliquera les modifications de la branche ***Readme-edits*** vers la branche ***master***.
* Rendez-vous dans l'onglet ***Pull requests*** et cliquez sur ***"New pull request"*** .
   
    <img src="https://github.com/HugoPineranda/Tutoriel_GitHub/blob/master/images/pullRequest.JPG" height="60%" width="60%">
* Choisissez les deux branches à comparer: `base` sera la branche à laquelle on veut appliquer les modifications (ici, ***master***), et `compare` celle que l'on a déjà modifié (ici, ***Readme-edits***)

    <img src="https://github.com/HugoPineranda/Tutoriel_GitHub/blob/master/images/pullRequest2.JPG" height="60%" width="60%">
* Plus bas, vous avez accès à la comparaison entre les 2 branches: les additions en vert et les suppressions en rouge.

    <img src="https://github.com/HugoPineranda/Tutoriel_GitHub/blob/master/images/modifs.JPG" height="40%" width="40%">
* Si vous êtes satisfait, cliquez sur ***"Create pull request"*** , donnez un titre et une description à votre requête, puis cliquez à nouveau sur ***"Create pull request"*** .
* Votre requête est créée. Les autres utilisateurs peuvent la passer en revue et la commenter dans l'onglet ***Pull requests***.

---
### ***Appliquer les modifications (Merge):***

* Une fois que vous avez effectué votre requête, vous (ou un autre utilisateur) avez la possibilité de la confirmer, et fusionner votre branche avec la branche de comparaison (ici, la branche ***master***).
* Si **GitHub** détecte un conflit entre les deux branches, vous devrez au préalable résoudre ce conflit. 
* Lorsque vous n'avez pas de conflit, vous pouvez alors appliquer les modifications en cliquant sur ***"Merge pull request"*** .

    <img src="https://github.com/HugoPineranda/Tutoriel_GitHub/blob/master/images/merge.JPG" height="60%" width="60%">
* Vous pourrez à nouveau commenter votre action avant de cliquer sur ***"Confirm merge"*** .
* Un message apparaît vous confirmant les modifications. Vous avez la possibilité de supprimer la branche sur laquelle les modifications ont été effectuées.
* Retournez dans la branche ***master***, on constate que le fichier ***Readme&#46;md*** a bien été modifié.

    <img src="https://github.com/HugoPineranda/Tutoriel_GitHub/blob/master/images/merge2.JPG" height="60%" width="60%">

---

## <a id="git" style="text-decoration:none">**3. Utilisation en local via Git** </a>

Téléchargez la dernière version de Git [ici](https://git-scm.com/downloads "Télécharger Git") et installez-la.


###  ***Créer un dépôt local:***

* Ouvrez **Git Bash**. Vous pouvez travailler avec CMD ou Terminal, mais il est fortement conseillé d'utiliser l'invité de commande fourni par **Git** car il reconnaît les commandes propres à ce logiciel.

* Pour configurer votre profil, saisir: <br>
`git config --global user.name "Votre Nom"`<br>
Ensuite, saisir: <br>
`git config --global user.email "VotreEmail@VotreEmail.com"`<br>
Un fichier **.gitconfig** a été créé à l'emplacement **C:\Users\VotreNom** contenant votre nom et votre adresse email.
* **Attention:** là où le nom n'a pas d'importance, l'email doit correspondre à l'adresse utilisée pour la création du compte GitHub.
* Pour créer un répertoire dans le même emplacement (ici, nous l'appellerons ***MonProjet***), saisir la commande:<br>
`mkdir ~/MonProjet`<br>
* Pour se déplacer dans le répertoire créé, saisir la commande:<br>
`cd ~/MonProjet`<br>
Le répertoire sur lequel on travaille est maintenant le dossier MonProjet.
* Pour que l'ordinateur reconnaîsse notre répertoire comme dépôt local git, saisir la commande:<br>
`git init`<br>

    <img src="https://github.com/HugoPineranda/Tutoriel_GitHub/blob/master/images/gitInit.JPG" height="60%" width="60%">
Le répertoire **.git** est un dossier caché, il ne s'affichera pas. Nous sommes maintenant par défaut dans la branche ***master*** de notre dépôt.

---
### ***Cloner un dépôt depuis GitHub sur votre machine:*** ###

* Pour créer une copie local à partir d'un dépôt sur GitHub, se rendre sur le dropdown ***Clone or download***, puis copier l'adresse indiquée. Retourner dans **Git Bash**, et saisir la commande:<br>
`git clone <adresse>`<br>
**Attention**, l'adresse doit se terminer par un **.git**.

    <img src="https://github.com/HugoPineranda/Tutoriel_GitHub/blob/master/images/clone.JPG" height="40%" width="40%">

 ---   
### ***Création du fichier Readme&#46;md:***

* Toujours dans l'invité **Git Bash**, saisir la commande:<br>
`touch Readme.md`<br>
Le fichier a été créé dans notre répertoire.
* Pour vérifier si **Git** le détecte, saisir la commande:<br>
`git status`<br>

    <img src="https://github.com/HugoPineranda/Tutoriel_GitHub/blob/master/images/untracked.JPG" height="60%" width="60%">
    
    On remarque que **Git** répertorie notre fichier comme ***untracked***.
* Pour que notre fichier soit détecté, saisir la commande:<br>
`git add Readme.md`
* Ne jamais oublier de consigner ses actions (**commit**), ici on saisira la commande:<br>
`git commit -m "Ajout de Readme.md"`<br>
où le texte entre guillemets décrit l'action effectuée.
* Vérifier qu'il n'y a pas d'erreur en réutilisant la commande `git status`.

---
### ***Connecter un dépôt local avec un dépôt GitHub:*** ###

* Il faut au préalable avoir créé un dépôt sur GitHub.com (dans cet exemple, **sans initialiser avec un Readme**, car nous l'ajouterons nous même à distance plus bas). De préférence, on utilisera le même nom pour le dépôt local et le dépôt sur GitHub.com.
* Saisir la commande:<br> `git remote add origin https://github.com/user/MonProjet.git`<br>
où ***user*** correspond à votre nom d'utilisateur GitHub et ***MonProjet*** correspond au nom de votre dépôt sur le site.<br>
**Git** fait maintenant la liaison entre votre dépôt distant et votre dépôt local.
* Pour vérifier que la liaison a été effectuée, saisir la commande:<br>
`git remote -v`<br>
qui donne la liste des origines distantes connues par votre dépôt local. Votre projet devraît y apparaître en **push** (envoi de données) et en **fetch** (réception de données).

    <img src="https://github.com/HugoPineranda/Tutoriel_GitHub/blob/master/images/connect.JPG" height="60%" width="60%">
* Nous avons maintenant connecté notre dépôt local à notre dépôt distant.

---
### ***Cas d'une liaison avec un fork:***

* Dans ce cas, il est important de configurer également la liaison avec le **fork**. Pour cela, saisir la commande:<br>
`git remote add upstream https://github.com/original-user/MonProjet.git`<br>
où ***original-user*** est le nom d'utilisateur du compte sur lequel vous avez **fork** le dépôt.
* On vérifie avec la commande `git remote -v`: le dépôt sur votre compte est **origin** et le dépôt originel est **upstream**.

---
### ***Envoi de fichiers:*** ###
* Pour envoyer nos fichiers vers le dépôt distant, saisir la commande:<br>
`git push`<br>
Si l'invité nous renvoie un message d'erreur, c'est parce que nous n'avons pas spécifié la branche dans laquelle on travaille. Ici, nous utilisons la branche ***master***. Saisir la commande:<br>
`git push --set-upstream origin master`

    <img src="https://github.com/HugoPineranda/Tutoriel_GitHub/blob/master/images/push.JPG" height="60%" width="60%">
* Si l'on n'est pas déjà connecté, une fenêtre de connexion s'ouvrira. Entrer alors ses identifiants.
* Vérifier sur GitHub: le fichier ***Readme&#46;md*** apparaît, ainsi que le **commit** que nous avons indiqué.

    <img src="https://github.com/HugoPineranda/Tutoriel_GitHub/blob/master/images/ajout.JPG" height="80%" width="80%">

---
### ***Réception de fichiers:*** ###

* Pour mettre à jour les fichiers locaux à partir du dépôt distant, saisir la commande:<br>
`git fetch`
* Si vous voulez directement **merge** les modifications dans votre branche active, saisir plutôt la commande:<br>
`git pull`

---
### ***Créer et manipuler des branches:*** ###

* Pour **créer** une branche, saisir la commande:<br>
`git checkout -b <nom de la branche>`<br>
**Attention**, Git vous switchera automatiquement dans cette branche.

* Pour **supprimer** une branche, saisir la commande:<br>
`git branch -d <nom de la branche>`

* Pour **changer** de branche sur laquelle travailler, saisir la commande:<br>
`git checkout <nom de la branche>`

* Pour **lister** toutes les branches, saisir la commande:<br>
`git branch`<br>
La branche courante s'affiche en **vert**.

* Pour **ajouter à GitHub** la branche créée, saisir la commande:<br>
`git push origin <nom de la branche>`<br>
Ou alors pour ajouter toutes les branches:<br>
`git push --all origin`

* Pour supprimer de GitHub une branche, saisir la commande:<br>
`git push origin :<nom de la branche>`

---
### ***Fusionner deux branches:*** ###

* Pour fusionner une branche avec votre branche active, saisir la commande:<br>
`git merge <nom de la branche>`

---
### ***Modifier localement un fichier:*** ###

* Effectuer les modifications sur le fichier. Dans cet exemple, nous rajouterons simplement une ligne à notre fichier ***"Readme&#46;md"*** .

* **Se placer dans la branche voulue** et saisir la commande:<br>
`git add <nom du fichier>`<br>
Si l'on a modifié plusieurs fichiers et que l'on veut tous les ajouter à notre branche, saisir la commande:<br>
`git add -A`

* **Commit** le fichier avec la commande:<br>
`git commit -m "message"`
* Vérifier que tout est conforme avec la commande:<br>
`git status`

* Envoyer les modifications à **GitHub** avec la commande:<br> 
`git push <nom du dépôt distant> <nom de la branche>`<br>
Ou alors, si cette commande est la dernière commande `push` effectuée:<br>
`git push`
* En basculant sur **GitHub**, on constate que les modifications on bien été prises en compte et le commit est présent, **uniquement** dans la branche sur laquelle nous avons travaillé.
---














