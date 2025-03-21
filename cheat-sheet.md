
# 📌 Cheat-sheet Lazygit

## 📖 Table des Matières

- [🔧 Installation](#-installation-de-lazygit)
- [🚀 Utilisation](#-utilisation)
- [⚙️ Configuration](#configuration-principale)
- [🛠 Fonctionnalités](#-principales-fonctionnalités)

---
🧐 **Git, l’outil indispensable des développeurs… mais pas toujours facile à maîtriser !**  

---

## 📌 **LazyGit : l’outil qui va changer votre façon d’utiliser Git**  

🔹 **Git est essentiel, mais soyons honnêtes : ses commandes peuvent vite devenir un casse-tête.** Avec **LazyGit**, tout devient plus fluide grâce à une interface claire, intuitive et ultra-rapide. Plus besoin de retenir des commandes interminables : en quelques clics, vous gérez vos commits 📝, fusionnez vos branches 🌿 et explorez l’historique 📖 de votre dépôt avec une facilité déconcertante.  

![LazyGit Interface](https://raw.githubusercontent.com/LucasAliasElvennope/test-stash/refs/heads/main/Exemple%20lazygit.png)  

🖥️ **LazyGit, c’est l’allié parfait pour simplifier et accélérer votre workflow Git !** ⚡ Que vous soyez débutant 🐣 ou développeur chevronné 🏆, il vous aide à rester efficace et à réduire les erreurs.  

---

## 🎯 **Pourquoi adopter LazyGit en entreprise ?**  

| ✅ **Avantages**                           | 🎯 **Ce que ça change pour vous**                                         |
|-------------------------------------------|--------------------------------------------------------------------------|
| ⚡ **Un gain de temps énorme**            | ⏩ Fini les commandes interminables, tout se fait plus rapidement.       |
| 🖥️ **Une interface claire et intuitive**  | 👀 Visualisez immédiatement l’état de votre projet et vos branches.      |
| 🛑 **Moins d’erreurs**                    | 🔍 Affichage précis des modifications pour éviter les mauvaises manipulations. |
| 🔄 **Des opérations complexes simplifiées** | 🎛️ Rebase, cherry-pick, reset… accessibles en quelques clics.            |
| 🤝 **Une meilleure collaboration**        | 💬 Travail en équipe plus fluide, moins de conflits Git.                 |

> **Avec LazyGit, votre équipe peut enfin se concentrer sur l’essentiel : coder, sans se battre avec Git.**  


## 💾 **Installation de LazyGit**

Voici comment installer LazyGit sur différents systèmes d'exploitation.

## 💻 Différents Supports/Systèmes d'exploitations

- [🐧 Linux](#-comment-installer-lazygit-sur-linux)
- [🍎 MacOS](#-comment-installer-lazygit-sur-macos)
- [🌅 Windows](#-comment-installer-lazygit-sur-windows)



## 🐧 Comment installer LazyGit sur Linux

### Via le gestionnaire de paquets (recommandé)
L'utilisation d'un gestionnaire de paquets est la méthode la plus simple et sécurisée pour installer LazyGit, car elle garantit une mise à jour automatique et une gestion des dépendances.

#### Debian/Ubuntu
Sur les distributions basées sur Debian, LazyGit est disponible via un PPA (Personal Package Archive) qui permet d'accéder aux dernières versions.
```sh
sudo add-apt-repository ppa:lazygit-team/release
sudo apt update
sudo apt install lazygit
```

#### Arch Linux (via pacman)
Les utilisateurs d'Arch Linux peuvent l'installer directement depuis les dépôts officiels avec pacman.
```sh
sudo pacman -S lazygit
```

## ❗Installation via npm, pnpm et yarn

LazyGit peut également être installé en tant que dépendance via les gestionnaires de paquets JavaScript. Cette méthode est utile si vous souhaitez l'intégrer à un projet spécifique.

#### Via npm
```sh
npm install -g lazygit
```

#### Via pnpm
```sh
pnpm add -g lazygit
```

#### Via yarn
```sh
yarn global add lazygit
```

Note : Si l'installation échoue en raison de permissions insuffisantes, vous pouvez essayer d'exécuter la commande avec `sudo` :
```sh
sudo npm install -g lazygit
sudo pnpm add -g lazygit
sudo yarn global add lazygit
```
⚠️ Attention, l'utilisation de `sudo` avec les gestionnaires de paquets JavaScript peut parfois causer des conflits. Il est recommandé d'utiliser `nvm` (Node Version Manager) ou d'ajuster les permissions de votre répertoire global `npm` pour éviter d'avoir besoin des droits administrateurs.

## 🍎 Comment installer LazyGit sur macOS

### Via Homebrew (recommandé)
```sh
brew install lazygit
```

## 🌅 Comment installer LazyGit sur Windows

### Via Scoop (recommandé)
```powershell
scoop install lazygit
```

### Via Chocolatey
```powershell
choco install lazygit
``` 

### Installation manuelle
1. Télécharger la dernière version depuis [GitHub](https://github.com/jesseduffield/lazygit/releases/latest)
2. Extraire l’archive et ajouter le binaire `lazygit.exe` à votre `PATH`.

## ✅ Vérification de l'installation

Pour vérifier que LazyGit est bien installé,essayez d'exécuter la commande suivante :
```sh
lazygit --version
```

Si la commande affiche un numéro de version, alors LazyGit est prêt à être utilisé ! 🎉



## 🚀 Utilisation 

### 1. Démarrage et Navigation de Base:

#### 🚀 Lancement:  
   - Ouvrez votre terminal  
   - Tapez lazygit et appuyez sur _Entrée_

#### ⌨️ Navigation dans l'interface:  
   - Utilisez les touches fléchées pour vous déplacer entre les différents panneaux (fichiers, branches, commits, etc.)  
   - La touche _Entrée_ sert à entrer dans un panneau ou à exécuter une action  
   - La touche _q_ permet de quitter Lazygit

### 2. Flux de Travail de Commit Standard:

#### 👁️‍🗨️ Visualisation des changements:  
   - Dans le panneau "Files" vous verrez les fichiers modifiés  
   - Utilisez _Entrée_ sur un fichier pour voir les modifications spécifiques  
  
#### 📥 Ajout de fichiers au staging (indexation):  
   - Sélectionnez les fichiers à ajouter avec les touches fléchées  
   - Appuyez sur _espace_ pour les ajouter au staging  
    
#### 📝 Création d'un commit:  
   - Allez dans le panneau "Commits"  
   - Appuyez sur _c_ pour ouvrir l'éditeur de message de commit  
   - Écrivez votre message de commit et enregistrez  

#### ⬆️ Push des commits:  
   - Allez dans le panneau "Local branches"  
   - S'il y a une branche distante configurée, appuyez sur _P_ pour faire un push

### 3. Gestion des Branches:  
  
#### ➕ Création d'une nouvelle branche:  
   - Dans le panneau "Local branches", appuyez sur _n_  
   - Entrez le nom de la nouvelle branche  
#### 🔄 Changement de branche (checkout):  
   - Sélectionnez la branche souhaitée  
   - Appuyez sur _Entrée_  
#### 🔀 Fusion (merge) de branches:  
   - Assurez-vous d'être sur la branche dans laquelle vous souhaitez fusionner  
   - Sélectionnez la branche à fusionner  
   - appuyez sur _m_ pour réaliser la fusion

### 4. Conflits:  
  
#### ⚠️ Identification des conflits:  
   - Lazygit affichera les fichiers en conflit dans "Files"  
#### 🛠️ Résolution des conflits:  
   - Utilisez votre éditeur de code pour résoudre les conflits dans les fichiers  
   - Une fois résolus, ajoutez les fichiers modifiés au staging (espace)   
   - Continuez la procédure de merge en validant avec la touche _c_ dans le panneau commit    

## 🔎 Onglet Status

| Touche    | Action                                                        | 
|-----------|---------------------------------------------------------------|
| `e`       | ✏️Permet d'ouvrir et modifier le fichier de configuration Lazygit|
| `u`       | 🔄Verifie si une mise à jour est disponible                     |
| `Entrer`  | ⬆️Permet de switch vers les dépots récents                      |
| `Echap`   | ❎Ferme ou annule l'action en cours                             |

## 🔎 Files

| Touche    | Action                                                        |
|-----------|---------------------------------------------------------------|
| `Espace`  | 📥Permet de staguer ou desstaguer un fichier                    |
| `c`       | 📝Effectuer un commit sur un fichier stagué                     |
| `e`       | ✏️Permet d'éditer un fichier dans l'éditeur externe             |
| `s`       | 🗂️Mettre de côté tous les changements non validés dans le repertoire de travail| 
| `d`       | ❎Permet d'annuler ou supprimer les modifications non validées  |
| `D`       | 🔄Permet de réinitialiser les fichiers du répertoire de travail, en annulant les changements locaux et en ramenant les fichiers à l'état du dernier commit|

## 🔎 Local branches

| Touche    | Action                                                        |
|-----------|---------------------------------------------------------------|
| `Espace`  | 🔀Permet de changer de branche en faisant un checkout sur la branche locale sélectionnée|
| `n`       | ➕Permet de créer une nouvelle branche                          |
| `d`       | 🗑️Supprime une branche locale                                   |
| `r`       | 🔄Rebase la branche locale                                      | 
| `g`       | 🔄Réinitialiser la branche locale avec plusieurs options (soft, mixed, ou hard)|
| `u`       | 🌐Permet d'afficher et de gérer les options de l'upstream pour la branche locale sélectionnée|

## 🔎 Commits

| Touche    | Action                                                        |
|-----------|---------------------------------------------------------------|
| `r`       | ✏️Réécrire le message d'un commit|
| `d`       | 🗑️Supprimer le commit sélectionné|
| `e`       | 🖋️Modifier le commit sélectionné|
| `A`       | 🔧Amender le dernier commit avec les changements en cours| 
| `Espace`  | 🔎Basculer sur un commit spécifique|
| `g`       | 🔄Permet de choisir différrentes options de réinitialisation (soft, mixed ou hard reset)|
| `P`       | ⬆️Push, envoie les commits vers le dépôt distant |

## 🔎 Stash

| Touche    | Action                                                        |
|-----------|---------------------------------------------------------------|
| `s`       | 💾Place les modifications non validées dans un stash temporaire|
| `d`       | 🗑️Supprimer stash spécifique|
| `p`       | ✅Applique et supprime le stash|
| `r`       | ✏️Renommer le stash| 
| `e`       | 🖋️Editer un stash dans l'editeur|



## Configuration principale


 **LazyGit** est hautement personnalisable grâce à des fichiers de configuration **YAML** situés dans _~/.config/lazygit/_.Voici un guide **complet et visuel** pour le configurer efficacement.

### 📂  Emplacement des fichiers de configuration

| Fichier                  | 📌 Chemin                     |
| :----------------------: | :---------------------------: |
| Linux                    | _~/.config/lazygit/config.yml_|
| macOS                    | _~/.config/lazygit/config.yml_|
| Windows (Git Bash, WSL)  | _~/.config/lazygit/config.yml_|
| Windows (CMD/Powershell) | _%APPDATA%\lazygit\config.yml_|

🔹 **Windows** : _APPDATA_ est généralement _C:\Users\NomUtilisateur\AppData\Roaming\lazygit\_

🔹 **WSL** : (Windows Subsystem for linux)suit la même logique que **Linux** _~/.config/lazygit/_
Si le dossier n'existe pas,crée-le:
```sh

 mkdir -p ~/.config/lazygit

 touch    ~/.config/lazygit/config.yml

```

### 📝 1. Configuration minimale pour bien débuter 📝


#### Exemple de configuration simple :

``` yaml

gui:
  showIcons: true  # Afficher des icônes sympas 🎨
  theme:
    lightTheme: false  # Mode sombre activé 🌙
    activeBorderColor: [blue, bold]  # Bordure active en bleu 🔵
    inactiveBorderColor: [white]  # Bordure inactive en blanc ⚪
  mouseEvents: false  # Désactiver la souris pour un usage full clavier ⌨️

git:
  paging:
    colorArg: always  # Garde les couleurs dans les logs Git 🌈
    pager: delta --dark  # Utiliser Delta pour des diffs stylés 😍


```

### ⚡ 2. Configurer les raccourcis clavier ⚡


   Tu veux **accélérer ton travail** avec des **touches personnalisées**? Voici un bon setup 👇
 

#### Exemple de configuration simple :

``` yaml

# Modifie les touches de raccourcis et les options Git
keybindings:
  universal:
    quit: "q"  # Quitter avec "q" 🏃
    refresh: "r"  # Rafraîchir avec "r" 🔄
    return: "<esc>"  # Retourner en arrière avec "Échap" ⬅️
    optionMenu: "m"  # Ouvrir un menu avec "m" 📜
  commits:
    moveDownCommit: "<down>"  # Aller au commit suivant 🔽
    moveUpCommit: "<up>"  # Aller au commit précédent 🔼
    amendToCommit: "A"  # Modifier le dernier commit 🛠️


```

### 🎨 3.Changer les couleurs pour un terminal plus stylé 🎨

   Tu veux un **thème ultra fun** pour ton terminal? Ajoute ça dans ton _config.yml_


#### Exemple de configuration simple :

``` yaml

gui:
  theme:
    activeBorderColor: [cyan, bold]  # Bordures actives en cyan ✨
    inactiveBorderColor: [gray]  # Bordures inactives en gris 🕶️
    selectedLineBgColor: [black]  # Fond noir pour l'élément sélectionné 🖤
    selectedRangeBgColor: [blue]  # Fond bleu pour une sélection multiple 🔵
    unstagedChangesColor: [yellow]  # Modifications non indexées en jaune 🌟
    stagedChangesColor: [green]  # Modifications indexées en vert 🍀

```

### 🏆 4.Gérer tes branches comme un(e) boss 🏆
    
   Ajoute cette config pour **travailler plus facilement avec tes branches** : 

#### Exemple de configuration simple :

```yaml

git:
  branchLogCmd: "git log --graph --oneline --decorate --all"  # Affiche un log graphique 🌳
  merging:
    autoFastForward: true  # Auto fast-forward quand possible 🔄
  pull:
    mode: "rebase"  # Utiliser `git pull --rebase` pour un historique propre 🚀
  push:
    autoPush: true  # Push automatique après un commit 📤


```

### 📜 5.Personnaliser la vue des commits 📜

   Si tu veux voir tes commits avec un affichage plus **clair et coloré**,ajoute cette ligne : 

```yaml

git:
  commit:
    signOff: true  # Ajouter un "Signed-off-by" automatiquement ✍️
    verbose: true  # Voir les changements avant validation 👀
  log:
    showGraph: true  # Activer l’affichage en graphe 🏗️
    allBranchesLogCmd: "git log --graph --oneline --decorate --all --color"  # Log coloré 🌈


```

### 🎯 En résumé 🎯

   Voici un bon **combo** de configuration pour : 

  ✅ **Un thème visuel amélioré**  
  ✅ **Des raccourcis clavier personnalisés**  
  ✅ **Une gestion des branches optimisée**  
  ✅ **Un affichage plus clair des commits**


  💡 **Tu peux tester cette configuration en modifiant ton** _/.config/lazygit/config.yml_


---

## 🌟 Principales fonctionnalités


### ✅ **Gestion simplifiée des commits**

- ⚡ Création rapide et intuitive
- ✏️ Modification simple des messages
- 📅 Historique visuel clair et interactif
- ♻️ Possibilité d'amender facilement les commits récents

### 🌿 **Branches sans prise de tête**

- 🌱 Création, renommage et suppression facile
- 🔄 Changement rapide entre branches
- 🔀 Fusion et rebase fluides et intuitifs

### 📁 **Fichiers et changements visibles en un coup d'œil**

- ➕ Gestion claire du staging
- 📝 Visualisation rapide et lisible des modifications
- 🔧 Résolution facilitée des conflits de fusion

### ☝️ **Interaction optimisée avec les dépôts distants**

- 📤 Envoi (push) rapide vers les remotes
- 📥 Récupération (pull) claire et simplifiée
- 📡 Support pratique des multiples remotes

### 🎨 **Interface utilisateur conviviale**

- 🖥️ Affichage interactif en panneaux clairs
- 🎛️ Expérience utilisateur fluide et intuitive
- 🔖 Navigation rapide et efficace

## 🛠️ Fonctionnalités avancées

- 🔍 Support intégré pour visualiser les différences clairement
- 📊 Historique interactif et lisible des logs
- 🔑 Simplification des tâches répétitives et complexes




