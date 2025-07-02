# ✈️ Tunisair Flight Delay Analysis

Ce projet a pour objectif d'explorer les causes possibles des retards des vols enregistrés par la compagnie tunisienne **Tunisair**, à l'aide d'outils d'analyse de données tels que **pandas** et **ydata-profiling**.

## 📊 Objectif

Étudier en profondeur les facteurs contribuant aux retards des vols en :
- Identifiant les corrélations entre variables (retard, statut, etc.)
- Détectant les valeurs manquantes ou aberrantes
- Générant un rapport automatisé avec ydata-profiling

## 🗃️ Données

Le jeu de données contient :
- Des informations sur les vols Tunisair
- Le statut du vol (retardé, à l'heure, annulé)
- Le temps de retard à l'arrivée

## 🔍 Étapes réalisées

### 1. Analyse avec Pandas :
- Chargement des données
- Aperçu général : `head()`, `info()`, `describe()`
- Détection des valeurs manquantes : `isnull().sum()`
- Statistiques descriptives par colonne

### 2. Analyse avec ydata-profiling :
- Rapport généré en HTML interactif
- Corrélations détectées entre statut et retard
- Mise en évidence :
  - D’un fort déséquilibre sur la variable `STATUS`
  - D’un grand nombre de zéros dans `Arrival delay`

## 📌 Résultats clés

- **35,4 %** des vols ont un `Arrival delay` nul
- `STATUS` est très déséquilibré : **73,4 %** d'une même valeur
- Une légère corrélation est observée entre le `STATUS` du vol et le `Arrival delay`

## ⚠️ Problèmes identifiés

- Colonnes déséquilibrées
- Présence de valeurs nulles ou aberrantes
- Zéros à interprétation ambigüe (retard réel ou valeur manquante ?)

## 🛠️ Technologies utilisées

- Python 3.12
- Pandas
- ydata-profiling
- Jupyter Notebook
- Visual Studio Code

## 🧠 Auteur

Projet réalisé par **Cheikh Niang**  
📧 cheikhniang159@gmail.com

---

> _Ce projet fait partie d’un checkpoint d’analyse de données dans le cadre d’un apprentissage autonome ou structuré._
