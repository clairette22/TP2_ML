# TP2 Machine Learning - Installation

## Prérequis généraux

- Python 3.7 ou supérieur
- pip (gestionnaire de paquets Python)

## Installation de l'environnement virtuel et des dépendances

### Étape 1 : Créer l'environnement virtuel

Ouvrez un terminal PowerShell dans le dossier du projet et exécutez :

```bash
python -m venv .venv
```

Cette commande crée un dossier `.venv` contenant l'environnement virtuel isolé.

### Étape 2 : Activer l'environnement virtuel

**Sur Windows (PowerShell) :**
```bash
.\.venv\Scripts\Activate.ps1
```

**Sur Windows (Command Prompt) :**
```bash
.venv\Scripts\activate.bat
```

**Sur macOS/Linux :**
```bash
source .venv/bin/activate
```

Une fois activé, vous verrez `(.venv)` au début de votre ligne de commande.

### Étape 3 : Installer les dépendances

Avec l'environnement virtuel activé, installez les prérequis :

```bash
pip install -r prerequis.txt
```

Cela installera les librairies suivantes :
- **pandas** : manipulation et analyse de données
- **numpy** : calculs numériques
- **matplotlib** : création de graphiques
- **seaborn** : visualisations statistiques
- **scikit-learn** : apprentissage automatique

## Vérification de l'installation

Pour vérifier que tout est correctement installé :

```bash
pip list
```

## Désactiver l'environnement virtuel

Quand vous avez terminé, tapez simplement :

```bash
deactivate
```

## Notes importantes

- Ne commitez **pas** le dossier `.venv` dans votre système de contrôle de version (il doit être dans `.gitignore`)
- Chaque fois que vous ouvrez un nouveau terminal, n'oubliez pas d'activer l'environnement virtuel
- Pour mettre à jour les dépendances, modifiez `prerequis.txt` et réexécutez `pip install -r prerequis.txt`
