# Data-Driven Decision Making — E-commerce Analytics

Projet de **Data-Driven Decision Making (DDDM)** consacré à l’analyse de données e-commerce et clients afin de produire des indicateurs utiles à la prise de décision, d’explorer les comportements d’achat et de présenter les résultats dans un tableau de bord interactif.

## Objectifs du projet

- Auditer, nettoyer et préparer les données clients et commandes.
- Construire des indicateurs métier, notamment le revenu (`Revenue`), l’âge des clients (`Age`) et les dépenses totales (`Total_Spending`).
- Réaliser une analyse exploratoire (EDA) : statistiques descriptives, distributions, pays et produits les plus performants, corrélations et valeurs aberrantes.
- Étudier les comportements des clients et réaliser une segmentation à l’aide de K-Means.
- Présenter des résultats lisibles dans un dashboard interactif destiné aux équipes de direction, marketing et opérations.

## Fonctionnalités du dashboard

L’application Streamlit propose plusieurs vues :

- **Accueil** : indicateurs clés, principaux pays par revenu et distribution des dépenses clients.
- **Direction** : revenus et volume de commandes par pays.
- **Marketing** : réponses aux campagnes, dépenses par catégorie de produits et distribution de l’âge.
- **Opérations** : produits générant le plus de revenu.
- **Machine Learning** : espace dédié aux résultats de modélisation présentés dans le projet.

## Technologies

- **Python** — analyse et préparation des données
- **Pandas, NumPy, SciPy** — manipulation des données et statistiques
- **Matplotlib, Seaborn, Plotly** — visualisations
- **Scikit-learn** — apprentissage automatique et clustering
- **Streamlit** — dashboard interactif
- **Jupyter Notebook** — exploration, analyse et modélisation

## Structure du dépôt

```text
Data-Driven-main/
└── DDDM Projet/
    ├── analysis_business/
    │   └── notebooks/
    │       └── analysis_business.ipynb
    ├── ml_dashboard/
    │   ├── notebooks/
    │   │   └── ml_modeling.ipynb
    │   └── dashboard/
    │       └── app.py
    ├── reports/
    │   ├── AB_Test_Plan_DDDM.docx
    │   └── presentation_data_story.pdf
    ├── shared_data/
    │   ├── Customers.csv
    │   └── data_Orders.csv
    ├── requirements.txt
    └── README.md
```

## Installation

Prérequis : **Python 3.10 ou plus récent** recommandé.

1. Clonez le dépôt, puis placez-vous dans le dossier du projet :

   ```bash
   git clone <URL_DU_DEPOT>
   cd Data-Driven-main/"DDDM Projet"
   ```

2. (Recommandé) Créez et activez un environnement virtuel :

   **Windows :**
   ```bash
   python -m venv .venv
   .venv\Scripts\activate
   ```

   **Linux / macOS :**
   ```bash
   python3 -m venv .venv
   source .venv/bin/activate
   ```

3. Installez les dépendances :

   ```bash
   pip install -r requirements.txt
   ```

## Lancer le dashboard

Depuis le dossier `DDDM Projet`, exécutez :

```bash
streamlit run ml_dashboard/dashboard/app.py
```

Streamlit affichera l’adresse locale à ouvrir dans le navigateur, généralement `http://localhost:8501`.

> Le dashboard lit les fichiers de données depuis le dossier `shared_data`. Conservez donc cette structure de dossiers lors de l’exécution.

## Explorer les notebooks

Ouvrez Jupyter Notebook ou JupyterLab depuis le dossier `DDDM Projet` :

```bash
jupyter notebook
```

Puis ouvrez :

- `analysis_business/notebooks/analysis_business.ipynb` pour l’analyse métier et l’exploration des données ;
- `ml_dashboard/notebooks/ml_modeling.ipynb` pour la modélisation et la segmentation.

## Rapports

Les livrables disponibles dans `reports/` comprennent le plan de test A/B et une présentation de data storytelling.

## Équipe et contributions

Ce dépôt a été organisé pour faciliter le travail collaboratif sur les volets analyse métier, machine learning et visualisation. Pour contribuer, créez une branche dédiée, effectuez vos modifications, puis ouvrez une Pull Request.

## Licence

Aucune licence n’est spécifiée pour le moment. Sauf indication contraire des auteurs, les droits restent réservés.
