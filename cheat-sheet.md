# 📌 Nom du Projet

Une brève description du projet, expliquant son objectif et ses principales fonctionnalités.

## 📖 Table des Matières

- [🔧 Installation](#-installation)
- [🚀 Utilisation](#-utilisation)
- [⚙️ Configuration](#-configuration)
- [🛠 Fonctionnalités](#-fonctionnalites)
- [📄 Documentation](#-documentation)

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

**1.  Démarrage et Navigation de Base:**

- ***Lancement:***  
   - Ouvrez votre terminal  
   - Tapez lazygit et appuyez sur *Entrée*

- ***Navigation dans l'interface:***  
   - Utilisez les *touches fléchées* pour vous déplacer entre les différents panneaux (fichiers, branches, commits, etc.)  
   - La touche *Entrée* sert à entrer dans un panneau ou à exécuter une action  
   - La touche *q* permet de quitter Lazygit

**2. Flux de Travail de Commit Standard:**

- ***Visualisation des changements:***  
   - Dans le panneau "Files" vous verrez les fichiers modifiés  
   - Utilisez *Entrée* sur un fichier pour voir les modifications spécifiques  
  
- ***Ajout de fichiers au staging (indexation):***  
   - Sélectionnez les fichiers à ajouter avec les *touches fléchées*  
   - Appuyez sur *espace* pour les ajouter au staging  
    
- ***Création d'un commit:***  
   - Allez dans le panneau "Commits"  
   - Appuyez sur *c* pour ouvrir l'éditeur de message de commit  
   - Écrivez votre message de commit et enregistrez  

- ***Push des commits:***  
   - Allez dans le panneau "Local branches"  
   - S'il y a une branche distante configurée, appuyez sur *P* pour faire un push

**3. Gestion des Branches:**  
  
- ***Création d'une nouvelle branche:***  
   - Dans le panneau "Local branches", appuyez sur *n*  
   - Entrez le nom de la nouvelle branche  
- ***Changement de branche (checkout):***  
   - Sélectionnez la branche souhaitée  
   - Appuyez sur *Entrée*  
- ***Fusion (merge) de branches:***  
   - Assurez-vous d'être sur la branche dans laquelle vous souhaitez fusionner  
   - Sélectionnez la branche à fusionner  
   - appuyez sur *m* pour réaliser la fusion

**4. Conflits:**  
  
- ***Identification des conflits:***  
   - Lazygit affichera les fichiers en conflit dans "Files"  
- ***Résolution des conflits:***  
   - Utilisez votre éditeur de code pour résoudre les conflits dans les fichiers  
   - Une fois résolus, ajoutez les fichiers modifiés au staging (espace)   
   - Continuez la procédure de merge en validant avec la touche *c* dans le panneau commit    

**1. Onglet Status**

| Touche    | Action                                                        | 
|-----------|---------------------------------------------------------------|
| `e`       | Permet d'ouvrir et modifier le fichier de configuration Lazygit|
| `u`       | Verifie si une misa à jour est disponible                     |
| `Entrer`  | Permet de switch vers les dépots récents                      |
| `Echap`   | Ferme ou annule l'action en cours                             |

**2. Files**

| Touche    | Action                                                        |
|-----------|---------------------------------------------------------------|
| `Espace`  | Permet de staguer ou desstaguer un fichier                    |
| `c`       | Effectuer un commit sur un fichier stagué                     |
| `e`       | Permet d'éditer un fichier dans l'éditeur externe             |
| `s`       | Mettre de côté tous les changements non validés dans le repertoire de travail| 
| `d`       | Permet d'annuler ou supprimer les modifications non validées  |
| `D`       | Permet de réinitialiser les fichiers du répertoire de travail, en annulant les changements locaux et en ramenant les fichiers à l'état du dernier commit|

**3. Local branches**

| Touche    | Action                                                        |
|-----------|---------------------------------------------------------------|
| `Espace`  | Permet de changer de branche en faisant un checkout sur la branche locale sélectionnée|
| `n`       | Permet de créer une nouvelle branche                          |
| `d`       | Supprime une branche locale                                   |
| `r`       | Rebase la branche locale                                      | 
| `g`       | Réinitialiser la branche locale avec plusieurs options (soft, mixed, ou hard)|
| `u`       | Permet d'afficher et de gérer les options de l'upstream pour la branche locale sélectionnée|

**4. Commits**

| Touche    | Action                                                        |
|-----------|---------------------------------------------------------------|
| `r`       | Réécrire le message d'un commit|
| `d`       | Supprimer le commit sélectionné|
| `e`       | Modifier le commit sélectionné|
| `A`       | Amender le dernier commit avec les changements en cours| 
| `Espace`  | Basculer sur un commit spécifique|
| `g`       | Permet de choisir différrentes options de réinitialisation (soft, mixed ou hard reset)|
| `P`       | Push, envoie les commits vers le dépôt distant |

**5. Stash**

| Touche    | Action                                                        |
|-----------|---------------------------------------------------------------|
| `s`       | Place les modifications non validées dans un stash temporaire|
| `d`       | Supprimer stash spécifique|
| `p`       | Applique et supprime le stash|
| `r`       | Renommer le stash| 
| `e`       | Editer un stash dans l'editeur|


## ⚙️ Configuration

Ce projet utilise des variables d'environnement. Créez un fichier `.env` à la racine du répertoire et ajoutez les variables requises :

```env
API_KEY=votre_cle_api_ici
DB_HOST=localhost
PORT=3000
```

Assurez-vous de remplacer les valeurs par vos configurations réelles.

## 🛠 Fonctionnalités

- ✅ Fonctionnalité 1 - Brève description
- ✅ Fonctionnalité 2 - Brève description
- ✅ Fonctionnalité 3 - Brève description

## 📄 Documentation

Pour une documentation détaillée, veuillez visiter : [Lien vers la documentation](https://votre-lien-documentation.com)

