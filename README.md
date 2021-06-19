# House Prices - Advanced Regression Techniques
Par Manon Giraud

## Résumé des notebooks
Ces deux notebooks contiennent le travail effectué pour la compétition Kaggle House Prices - Advanced Regression Techniques.
Dans le premier, l'analyse exploratoire, avec analyse univariée et bivariée, et les graphiques associés, ainsi que la transformation des données.
Dans le deuxième, la modélisation : le choix des hyperparamètres pour la forêt en utilisant Optuna, et l'examen des modèles obtenus.

## Comment l'utiliser
Pour prédire SalePrice sur de nouvelles données :
1 - Importer ces données dans un dataframe
2 - Utiliser la fonction transforme_donnes du premier notebook, qui prend comme unique paramètre donnees (les données importées dans 1-)
3 - Tronquer les données transformées en ne sélectionnant que les colonnes de la liste imp_vars, dans le deuxième notebook.
        Exemple : donnees = donnees[imp_vars]
4 - Utiliser la fonction predict de l'objet rf sur les données tronquées. Le résultat sera un objet vecteur contenant toutes les valeurs prédites.
        Exemple : resultat = rf.predict(donnees)
