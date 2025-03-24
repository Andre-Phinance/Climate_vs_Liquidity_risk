# Projet d'Analyse Financière et Climatique

## Aperçu
Ce projet explore la relation entre les ratios financiers de grandes banques canadiennes et des variables climatiques au fil du temps. Les banques analysées sont :
- Royal Bank of Canada (RY.TO)
- Toronto-Dominion Bank (TD.TO)
- Bank of Nova Scotia (BNS.TO)

Les variables climatiques étudiées incluent :
- Niveau moyen de la mer (Sea_Lvl_M)
- Moyenne des degrés-jours de refroidissement (CDD_M)
- Précipitations maximales sur 5 jours (Rx5Day_M)
- Température au 10e centile (T10_M)
- Température au 90e centile (T90_M)
- Vitesse du vent au 90e centile (WP90_M)

## Méthodologie
- **Collecte des données** : Les données financières ont été obtenues via `yfinance`, tandis que les données climatiques proviennent d'un fichier Excel.
- **Traitement des données** : Les valeurs manquantes dans les ratios financiers ont été remplies à l'aide d'une moyenne mobile basée sur les périodes t-1 et t+1. Les données climatiques mensuelles ont été agrégées en moyennes trimestrielles.
- **Analyse** : Des modèles de régression linéaire et log-linéaire ont été utilisés pour évaluer l'impact des variables climatiques sur les ratios financiers tels que le **Cash Ratio**, le **Quick Ratio** et le **Current Ratio**.

## Outils et Bibliothèques
Les outils et bibliothèques suivants ont été utilisés dans ce projet :
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `plotly`
- `statsmodels`
- `scipy`
- `sklearn`
- `yfinance`

## Visualisations
Le projet inclut plusieurs visualisations :
- Graphiques de séries temporelles montrant les tendances des ratios financiers et des variables climatiques.
- Courbes de régression log-linéaire ajustées pour illustrer les relations modélisées.

## Résultats
Les résultats comprennent des résumés des modèles de régression avec :
- Coefficients
- Valeurs p (p-values)
- R² (coefficient de détermination)
- Erreur quadratique moyenne (MSE)

Ces métriques permettent d'évaluer la relation entre les variables climatiques et les ratios financiers.

## Comment Exécuter le Code
1. Assurez-vous que toutes les bibliothèques listées ci-dessus sont installées (`pip install -r requirements.txt` si un fichier `requirements.txt` est fourni).
2. Placez les fichiers de données (Excel pour les données climatiques et financières) dans l’environnement local pour bien exécuter le code.
3. Exécutez le notebook Jupyter ou le script Python pour lancer l'analyse.

## Avertissement
Ce projet est une étude basée sur des données historiques. Les résultats doivent être interprétés avec prudence et ne constituent pas une prédiction des performances futures.
