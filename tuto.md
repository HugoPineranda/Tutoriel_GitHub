# **Guide d'utilisation de GitHub**

## **_Sommaire:_**
#### [1. Introduction à GitHub](#intro)
#### [2. Utilisation via la plateforme GitHub.com](#github)
    - Créer un dépôt
    - Ajouter/créer un fichier
    - Créer une branche
    - Effectuer des modifications sur un fichier et les répertorier (Commit)
    - Effectuer une requête d'application des modifications (Pull Request)
    - Appliquer les modifications (Merge)
#### [3. Utilisation en local via Git](#git)
    - Créer un dépôt local
    - Conncter le dépôt local et le dépôt GitHub
    - Créer une branche locale
    - Appliquer des modifications localement
    - Envoyer et récupérer des informations depuis GitHub


## **1. Introduction à GitHub et Git**<a id="intro"></a>
>*Qu'est-ce que GitHub ?*

**GitHub** est le plus grand espace de stockage de travaux collaboratifs au monde. C'est un service en ligne d'hébergement de **repositories**. Il permet la communication facile entre les développeurs et le partage de code.

Il fonctionne avec le logiciel de gestion de versions décentralisées **Git**, développé par Linus Torvald, auteur du noyau Linux.  

>*Pourquoi utiliser GitHub ?*

Le principal atout est le contrôle de version. Si deux personnes travaillent sur le même fichier, il est impossible que leurs données soient perdues. En effet, Git effectue une sauvegarde de chaque modification effectuée. Il est ainsi possible de revenir à une version précedente du produit ou code.

**GitHub** a l'avantage d'être simple à prendre en main, même sans connaissances préalables en programmation. De plus, les utilisateurs conservent 100% de la propriété des projets déposés.

L'avantage de **GitHub** par rapport à **Git** est l'interface visuelle qui est beaucoup plus intuitive; en effet l'utilisation de Git nécessite de passer par un invité de commande type CMD ou, **Git Bash**.


## **2. Utilisation via la plateforme GitHub.com** <a id="github"></a>

### ***Créer un dépôt:***

* Rendez vous su Github.com. Après avoir créé votre compte, Cliquez sur le + en haut à droite, puis sur *"New Repository"*.

    ![](https://github.com/HugoPineranda/Tutoriel_GitHub/tree/master/images/NewRepository.jpg)
* Nommez votre dépôt et ajoutez lui une description.
* Sélectionnez *"Initialize this repository with a README"*, sauf si vous importez un dépôt déjà existant, puis cliquez sur *"Create repository"*.

    ![](https://github.com/HugoPineranda/Tutoriel_GitHub/tree/master/images/NewRepository2.jpg)

Notre dépôt a été créé et contient un fichier, *"Readme.md"* .

### ***Ajouter/créer un fichier:***

Vous avez la possibilité d'uploader un fichier dans votre dépôt ou bien de le créer via l'éditeur GitHub:

![](https://github.com/HugoPineranda/Tutoriel_GitHub/tree/master/images/Edit.jpg)
* Si vous voulez créer un dossier, ajoutez son emplacement lors de la création du fichier. GitHub le détectera automatiquement et le créera.

    ![](https://github.com/HugoPineranda/Tutoriel_GitHub/tree/master/images/SousDossier.jpg)
* Vous pouvez réaliser cette action autant de fois que nécessaire, mais votre dossier ne sera pas créé s'il est vide. Vous devez y ajouter un fichier.

    ![](https://github.com/HugoPineranda/Tutoriel_GitHub/tree/master/images/SousSousDossier.jpg)

### ***Créer une branche:***

Par défaut, le projet "définitif" sera enregistré dans la branche ***master***.

La création de branches permet de travailler sur différentes versions d'un dépôt en même temps. On travaille sur une branche, on l'édite, puis on applique (ou non) à la branche ***master*** les modifications réalisées.

Pour créer une branche à partir de la branche ***master*** :

* Allez dans votre **dépôt** GitHub
* Cliquez sur le menu dropdown "Branch: master"
* Entrez le nom de votre nouvelle branche. Il est fortement conseillé de choisir un nom explicite. Dans cette exemple, nous modifierons le fichier *"Readme.md"*, on appellera donc la branche "Readme-edits". Cliquez ensuite sur "Create branch".
   
    ![](https://github.com/HugoPineranda/Tutoriel_GitHub/tree/master/images/CreateBranch.jpg)
* Vous êtes maintenant dans la branche ***Readme-edits***. Toute modification apportée aux fichiers via GitHub sera appliquée uniquement dans cette branche.
* Pour changer de branche, retournez dans le dropdown menu et sélectionnez une autre branche.

### ***Effectuer des modifications sur un fichier et les répertorier :***

* On continuera avec l'exemple de la modification du fichier *"Readme.md"*.
* Dans votre branche ***Readme-edits***, cliquez sur le fichier *"Readme.md"*, puis sur le bouton *"Edit this file"* symbloisé par un crayon :

    ![](https://github.com/HugoPineranda/Tutoriel_GitHub/tree/master/images/EditFile.jpg)
* Effectuez vos modifications. Dans cet exemple, le fichier contient 2 lignes générées à partir du nom du dépôt/ Nous allons rajouter une troisième ligne "Tutoriel d'utilisation de GitHub" et supprimer la deuxième ligne :

    ![](https://github.com/HugoPineranda/Tutoriel_GitHub/tree/master/images/Ligne3.jpg)
* Dans la fenêtre  ***"Commit Changes"*** , donnez un titre  et une description à votre modification. Cette étape, le **Commit**, est très importante car elle apparaîtra sur **GitHub** et permet le suivi des différentes modifications apportées à un fichier.
* Vous avez ensuite le choix: enregistrer les modifications sur la branche en cours, ou créer une nouvelle branche et faire une ***pull request*** que nous verrons plus tard.
* Cliquez ensuite sur **"Commit Changes"** .

    ![](https://github.com/HugoPineranda/Tutoriel_GitHub/tree/master/images/Commit.jpg)
* On remarquera que le ***Commit*** apparaît dans votre branche ***Readme-edits***, avec l'utilisateur et la date de modification.

    ![](https://github.com/HugoPineranda/Tutoriel_GitHub/tree/master/images/NotifCommit.jpg)
* Par contre, si vous allez dans la branche ***master***, les modifications n'ont pas été appliquées. Pour cela, il faut faire une ***pull request***.

### ***Effectuer une requête d'application des modifications (Pull Request) :***

* ***Pull Request*** est une requête d'application des modifications appliquées à une branche dans une autre. Elle permet aussi de voir les différences entre deux branches en les comparant. Ici, on appliquera les modifications de la branche ***Readme-edits*** vers la branche ***master***.
* Rendez-vous dans l'onglet ***Pull requests*** et cliquez sur ***"New pull request"*** .
   
    ![](https://github.com/HugoPineranda/Tutoriel_GitHub/tree/master/images/PullRequest.jpg)
* Choisissez les deux branches à comparer: `base` sera la branche à laquelle on veut appliquer les modifications (ici, ***master***), et `compare` celle que l'on a déjà modifié (ici, ***Readme-edits***)

    ![](https://github.com/HugoPineranda/Tutoriel_GitHub/tree/master/images/PullRequest2.jpg)
* Plus bas, vous avez accès à la comparaison entre les 2 branches: les additions en vert et les suppressions en rouge.

    ![](https://github.com/HugoPineranda/Tutoriel_GitHub/tree/master/images/Modifs.jpg)
* Si vous êtes satisfait, cliquez sur ***"Create pull request"*** , donnez un titre et une description à votre requête, puis cliquez à nouveau sur ***"Create pull request"*** .
* Votre requête est créée. Les autres utilisateurs peuvent la passer en revue et la commenter dans l'onglet ***Pull requests***.

### ***Appliquer les modifications (Merge)***

* Une fois que vous avez effectué votre requête, vous (ou un autre utilisateur) avez la possibilité de la confirmer, et fusionner votre branche avec la branche de comparaison (ici, la branche ***master***).
* Si **GitHub** détecte un conflit entre les deux branches, vous devrez au préalable résoudre ce conflit. 
* Lorsque vous n'avez pas de conflit, vous pouvez alors appliquer les modifications en cliquant sur ***"Merge pull request"*** .

    ![](https://github.com/HugoPineranda/Tutoriel_GitHub/tree/master/images/Merge.jpg)
* Vous pourrez à nouveau commenter votre action avant de cliquer sur ***"Confirm merge"*** .
* Un message apparaît vous confirmant les modifications. Vous avez la possibilité de supprimer la branche sur laquelle les modifications ont été effectuées.
* Retournez dans la branche ***master***, on constate que le fichier Readme.md a bien été modifié.

    ![](https://github.com/HugoPineranda/Tutoriel_GitHub/tree/master/images/Merge2.jpg)
















## **3. Utilisation en local via Git** <a id="git"></a>



