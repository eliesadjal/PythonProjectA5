# PythonProjectA5


LE DATASET



Le dataset nous provient du département « statistics and data modeling » de l’université de Strathclyde à Glasgow (Ecosse). Ce dataset est en fait une fraction d’un jeu de données tenu par un centre de la NASA basé en Australie.

Il est composé de 6435 fractions d’images satellites (appelées Neighbourhoods (NBH)) décomposées en 9 pixels (3x3) chacune.

 Chaque COLONNE du dataset représente les 9 pixels de chaque neighbourhood, dans chacune des 4 bandes spectrales.
	Il y aura donc 9x4 = 36 COLONNES dans le dataset
  
  À ces dernières s’ajoutent une 37ème COLONNE


La 37ème COLONNE est appelée « Classification Label ». Elle représente en fait la classe du pixel central.
Très concrètement, cette classe est le type de sol qui peut être observé sur la portion d’image contenu dans le pixel central de chaque Neighbourhood. Il y a 6 types de sols observables selon notre dataset : 

	1 : Terre rouge
	2 : Culture du coton
	3 : Sol gris
	4 : Sol gris humide
	5 : Sol avec des chaumes de végétation	
	6 : Classe de mélange (tous les types présents)
	7 : Sol gris très humide
  
  
  
  
  
  L'OBJECTIF
  
  
  
  
  
  

L’objectif de ce projet réside dans la 37ème colonne que nous venons d’introduire. En effet, c’est un travail de classification qui nous est suggéré ici. 
Concrètement nous voulons, en nous basant sur les « valeurs » des pixel d’un même neighbourhood dans chacune des 4 bande spectrale, prédire quel type de sol est capturé dans pixel central. C’est à dire prédire le « classification Label ».







CONCLUSION




Ce Dataset était assez complexe et nous a demandé un travail de recherche pour sa compréhension. Cependant il était intéressant à étudier. Faire parler ses données n’était pas forcément évident car nous ne savions pas instinctivement quelle analyse était vraiment pertinente en regard de notre problème. Nous avons quand même pu obtenir des résultats assez concluants.


RandomForestRegressor : 88.27%
Support Vector Regression (SVR) : 69.20%
Gaussian Naive Bayes : 79.56%
Decision Tree Classifier : 83.77%

Feature la plus importante : Valeur du pixel central dans la 4ème bande spectrale.



