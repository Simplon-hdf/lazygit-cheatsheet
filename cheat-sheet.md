
# 📌 Cheat-sheet Lazygit

## 📖 Table des Matières

- [🔧 Installation](#-installation)
- [🚀 Utilisation](#-utilisation)
- [⚙️ Configuration](#-configuration)
- [🛠 Fonctionnalités](#-fonctionnalites)
- [📄 Documentation](#-documentation)


🚀 **Boostez votre efficacité avec LazyGit : La gestion Git simplifiée !**

---

## 📌 **LazyGit, votre meilleur allié pour Git**

🔹 **Git est incontournable, mais ses commandes complexes peuvent vite devenir un obstacle.** **LazyGit** supprime ces difficultés en proposant une interface graphique claire, intuitive et ultra-rapide. Finies les commandes interminables : gérez vos commits ✅, fusionnez vos branches 🌿 et naviguez aisément dans l'historique 📜 de votre dépôt grâce à une expérience utilisateur optimisée.

![LazyGit Interface](https://raw.githubusercontent.com/LucasAliasElvennope/test-stash/refs/heads/main/Exemple%20lazygit.png)

🖥️ **LazyGit simplifie et accélère votre workflow Git !** 🚀 Fini les commandes complexes : tout est accessible en quelques touches ou clics. Que vous soyez débutant 🐣 ou développeur confirmé 🧑‍💻, LazyGit vous aide à rester productif tout en réduisant les erreurs.

📌 **Consacrez moins de temps ⏳ à gérer Git, et concentrez-vous sur l’essentiel : votre code !** 💡

---

## 🎯 **Pourquoi adopter LazyGit en entreprise ?**

| ⚡ **Avantage**                           | 🎯 **Bénéfices pour votre équipe**                                       |
|------------------------------------------|-------------------------------------------------------------------------|
| 🚀 **Rapidité accrue**                   | ⏱️ Réduit considérablement le temps consacré à Git, augmentant la productivité. |
| 🖥️ **Interface ergonomique**             | 📊 Permet une vision claire et immédiate de l’état du projet.            |
| 🔥 **Réduction des erreurs**             | 🎯 Présente clairement les modifications, limitant ainsi les risques d’erreur. |
| 🛠️ **Opérations complexes simplifiées**  | ⚙️ Facilite grandement les opérations telles que le rebase, cherry-pick et reset. |
| 🤝 **Collaboration optimisée**           | 🧑‍🤝‍🧑 Renforce la fluidité et l’efficacité du travail collaboratif.      |

> **En entreprise, LazyGit aide votre équipe à se concentrer pleinement sur le développement du produit en éliminant les contraintes liées à la gestion des versions.**


# 💾 Installation de LazyGit

Voici comment installer LazyGit sur différents systèmes d'exploitation.

## 💻 Supports

- [🐧 Linux](#-Installation_sur_Linux)
- [🍎 MacOS](#-Installation_sur_macOS)
- [🌅 Windows](#-Installation_sur_Windows)


## 🐧 Installation sur Linux

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

#### Fedora (via dnf)
Sur Fedora, LazyGit est inclus dans les dépôts par défaut et peut être installé avec dnf.
```sh
sudo dnf install lazygit
```

#### Autres distributions
Pour les autres distributions Linux, vous pouvez vérifier la disponibilité de LazyGit dans votre gestionnaire de paquets habituel (comme `zypper` pour openSUSE ou `nix-env` pour NixOS). Sinon, la méthode d’installation manuelle est toujours une alternative.

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

### Installation manuelle (si indisponible dans les dépôts)
Si LazyGit n'est pas disponible via votre gestionnaire de paquets, vous pouvez télécharger la dernière version et l'installer manuellement :
```sh
LAZYGIT_VERSION=$(curl -s https://api.github.com/repos/jesseduffield/lazygit/releases/latest | grep -Po '"tag_name": "\K[^"]*')
curl -Lo lazygit.tar.gz "https://github.com/jesseduffield/lazygit/releases/download/${LAZYGIT_VERSION}/lazygit_$(uname -s)_$(uname -m).tar.gz"
tar xf lazygit.tar.gz -C /usr/local/bin lazygit
```

## 🍎 Installation sur macOS

### Via Homebrew (recommandé)
```sh
brew install lazygit
```

### Installation manuelle
```sh
LAZYGIT_VERSION=$(curl -s https://api.github.com/repos/jesseduffield/lazygit/releases/latest | grep -Po '"tag_name": "\K[^"]*')
curl -Lo lazygit.tar.gz "https://github.com/jesseduffield/lazygit/releases/download/${LAZYGIT_VERSION}/lazygit_Darwin_x86_64.tar.gz"
tar xf lazygit.tar.gz -C /usr/local/bin lazygit
```

## 🌅 Installation sur Windows

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

Après l’installation, vous pouvez vérifier que LazyGit est bien installé en exécutant :
```sh
lazygit --version
```

Si la commande affiche un numéro de version, alors LazyGit est prêt à être utilisé ! 🎉


## 🚀 Utilisation

Après l'installation, vous pouvez utiliser le projet comme suit :

- **Exécuter en mode développement :**
  ```bash
  npm run dev  # ou yarn dev
  ```
- **Construire pour la production :**
  ```bash
  npm run build  # ou yarn build
  ```
- **Exécuter les tests :**
  ```bash
  npm test  # ou yarn test
  ```

---

## ⚙️💻 Configuration 🚀🎉

 **LazyGit** est hautement personnalisable grâce à des fichiers de configuration **YAML** situés dans <span style="background-color: #CCFFFF; padding: 2px">~/.config/lazygit/</span>.Voici un guide **complet et visuel** pour le configurer efficacement.

### 📂 1️⃣ **Emplacement des fichiers de configuration**

| Fichier                  | 📌 Chemin                                                                                    |
| :----------------------: | :------------------------------------------------------------------------------------------: |
| Linux                    | <span style="background-color: #CCFFFF; padding: 2px">~/.config/lazygit/config.yml</span> |
| macOS                    | <span style="background-color: #CCFFFF; padding: 2px">~/.config/lazygit/config.yml</span> |
| Windows (Git Bash, WSL)  | <span style="background-color: #CCFFFF; padding: 2px">~/.config/lazygit/config.yml</span> |
| Windows (CMD/Powershell) | <span style="background-color: #CCFFFF; padding: 2px">%APPDATA%\lazygit\config.yml</span>  |

🔹 **Windows** : <span style="background-color: #CCFFFF; padding: 2px">APPDATA</span>est généralement <span style="background-color: #CCFFFF; padding: 2px">C:\Users\NomUtilisateur\AppData\Roaming\lazygit\</span>./br

🔹 **WSL** : (Windows Subsystem for linux)suit la même logique que **Linux**(<span style="background-color: #CCFFFF; padding: 2px">~/.config/lazygit/</span>)/br
Si le dossier n'existe pas,crée-le:
```sh

 mkdir -p ~/.config/lazygit

 touch    ~/.config/lazygit/config.yml

```

### **1. Configuration minimale pour bien débuter** 📝

   Si tu veux **commencer simplement**, voici une **configuration de bade** qui améliore l'expérience utilisateur :

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

### **2. Configurer les raccourcis clavier** ⚡⚡⚡

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

### **3.Changer les couleurs pour un terminal plus stylé** 🎨

   Tu veux un **thème ultra fun** pour ton terminal? Ajoute ça dans ton <span style="background-color: yellow; padding: 2px">config.yml</span>

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


---
## 🛠 Fonctionnalités

- ✅ Fonctionnalité 1 - Brève description
- ✅ Fonctionnalité 2 - Brève description
- ✅ Fonctionnalité 3 - Brève description

## 📄 Documentation

Pour une documentation détaillée, veuillez visiter : [Lien vers la documentation](https://votre-lien-documentation.com)



