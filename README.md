# titanic-ml

## 1. Descripció del dataset

Aquest dataset sobre els passatgers del Titanic està integrat pels conjunts d'entrenament (891 registres) i de prova (418 registres) disponibles a Kaggle.
Els 12 camps usats en el dataset són els següents: 

* PassengerId: identificador numèric de cada passatger embarcat
* Survived: Indica si el passatger va sobreviure o va morir (1 = Survived, 0 = Died)
* Pclass: Indica el tipus de ticket (1 = Primera classe, 2 = Segona classe, 3 = Tercera classe)
* Name: Nom complet del passatger
* Sex: Gènere del passatger (Male/Female)
* Age: Edat del passatger
* SibSp: Número de germans/cònjuges a bord entre els passatgers
* Parch: Número de pares/fills a bord entre els passatgers
* Ticket: Número de ticket del  passatger
* Fare: Preu del ticket del passatger
* Cabin: Número de la cabina assignada al passatger
* Embarked: Port on el passatger ha embarcat (C = Cherbourg, Q = Queenstown, S = Southampton)

L'objectiu d'aquesta anàlisi és desenvolupar un model per predir la supervivència de cadascun dels passatgers del Titanic.
Per tant, el conjunt de test no disposa de la variable Survived.
