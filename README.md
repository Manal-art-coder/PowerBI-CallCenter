# 📊 Analyse des Performances d'un Centre d'Appel avec Power BI

## 📌 Description du projet
Ce projet vise à analyser les performances d'un centre d'appel à l'aide de Power BI. Il a été réalisé dans le cadre de ma formation au sein de Data Scientest et couvre plusieurs axes d'analyse, notamment la performance du service client, l'évolution des revenus et l'efficacité des managers et employés.

## 🔍 Objectifs
- Explorer et nettoyer les données brutes
- Transformer et modéliser les données avec un **modèle en étoile**
- Créer des indicateurs clés de performance (KPIs)
- Concevoir un **tableau de bord interactif** pour une meilleure prise de décision

## 🗂 Jeu de données
Le projet repose sur plusieurs tables de données :

### **1. Call Charges**  
- **Call Charges 2018 (Min)** : Prix de l'appel par minute en 2018
- **Call Charges 2019 (Min)** : Prix de l'appel par minute en 2019
- **Call Charges 2020 (Min)** : Prix de l'appel par minute en 2020

### **2. Employees**  
- **EmployeeID** : Identifiant unique de l'employé
- **EmployeeName** : Nom de l'employé
- **Site** : Bureau de rattachement
- **ManagerName** : Nom du manager

### **3. Call Type**  
- **CallTypeID** : Identifiant unique du type d'appel
- **CallTypeDesc** : Description du type d'appel

### **4. Call Data (2018-2021)**  
- **CallTimestamp** : Date et heure de l'appel
- **CallType** : Type d'appel
- **CallDuration** : Durée de l'appel en secondes
- **WaitTime** : Temps d'attente avant prise en charge
- **Call Abandoned** : Indicateur d'abandon (supprimé lors du nettoyage)

## 🛠 Préparation et Transformation des Données
1. Suppression de la colonne **Call Abandoned**
2. Création d'une nouvelle colonne **SLA Compliance**
   - **Within SLA** : si le temps d'attente < 35 secondes
   - **Outside SLA** : si le temps d'attente >= 35 secondes
3. Nettoyage des anomalies et outliers
4. Création d'une table Date

## 📊 Axes d'Analyse

### 1️⃣ **Vue Globale du Service Client**
- Nombre total d'appels
- Répartition des appels **Within SLA / Outside SLA** par secteur, bureau, etc.
- Temps moyen d'appel
- KPIs clés pour mesurer la performance

### 2️⃣ **Revenus par Appels**
- Évolution annuelle des revenus
- Revenus par secteur, équipe et période

### 3️⃣ **Performance des Managers et Employés**
- Comparaison des performances des managers
- Temps d'attente moyen par équipe / employé

## 🚀 Comment Utiliser ce Projet ?
1. **Cloner ce dépôt GitHub** :
   ```sh
   git clone https://github.com/Manal-art-coder/powerbi-callcenter.git
   ```
2. **Ouvrir le fichier Power BI** :
   - Télécharger le fichier **.pbix**
   - L'ouvrir avec **Microsoft Power BI Desktop**
3. **Explorer les données et interagir avec les visualisations**

## 📎 Fichiers Disponibles
- `powerbi-callcenter.pbix` : Fichier Power BI avec le modèle et le tableau de bord
- `data/` : Dossier contenant les fichiers CSV utilisés
- `scripts/` : Contient les scripts de transformation Power Query 
- `README.md` : Documentation complète du projet

## 🏆 Résultats et Enseignements
- Mise en place d'un modèle **en étoile** performant
- Nettoyage et transformation efficace des données
- Création de visualisations interactives pour une meilleure prise de décision

## 📢 Contact
Si vous avez des questions ou des suggestions, n'hésitez pas à me contacter via [LinkedIn](https://www.linkedin.com/in/manaljewa/) ou ouvrir une issue sur ce dépôt GitHub.

📌 **Auteur** : Manal JEWA  
📅 **Date** : Février 2025  
💼 **Technologies utilisées** : Power BI, Power Query, DAX, CSV
