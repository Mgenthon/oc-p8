# oc-p8
Le but final du projet est de développer un robot cueilleur de fruit intelligent.
La première étape du projet est dé développer une application Pyspark pour extraire les features d'un set de de donnée disponible sur Kaggle (https://www.kaggle.com/moltean/fruits). Il y a environ 100 000 images pour 13 fruits et légumes.
Dans le notebook, on retrouve le code pour déployer l'application avec Spark 3.0 (Utilisation Pandas_UDF), de la lecture des images au format binary dans un spark dataframe,s à l'extraction de features en utilisant du transfer learning (VGG 16 ImageNet). L'étape suivante est d'entraîner un classifieur (Gradient Boosting le meilleur probablement) sur les features extraites.
Dans les requirements, on retrouve les librairies nécessaires et leur versions pour faire tourner l'appli. Le bootstrap est utilisé sur AWS EMR. Il faut choisir EMR 6.1.0, Spark et Hadoop.
