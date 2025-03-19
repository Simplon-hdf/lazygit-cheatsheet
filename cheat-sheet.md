<<<<<<< Updated upstream
# Cheat-sheet Lazygit
=======
# 📌 Cheat-sheet Lazygit
>>>>>>> Stashed changes


## 📖 Table des Matières

- [🔧 Installation](#-installation)
- [🚀 Utilisation](#-utilisation)
- [⚙️ Configuration](#-configuration)
- [🛠 Fonctionnalités](#-fonctionnalites)
- [📄 Documentation](#-documentation)
- [✅ Tests](#-tests)
- [📜 Licence](#-licence)
- [📬 Contact](#-contact)


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

## 🔧 Installation

Pour configurer le projet localement, suivez ces étapes :

1. **Cloner le référentiel :**
   ```bash
   git clone https://github.com/votre-utilisateur/nom-du-projet.git
   ```
2. **Accéder au répertoire du projet :**
   ```bash
   cd nom-du-projet
   ```
3. **Installer les dépendances :**
   ```bash
   npm install  # ou yarn install
   ```
4. **Démarrer le serveur de développement :**
   ```bash
   npm start  # ou yarn start
   ```

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

## ✅ Tests

Pour exécuter les tests, utilisez la commande suivante :
```bash
npm test  # ou yarn test
```
Assurez-vous que tous les tests passent avant le déploiement.

