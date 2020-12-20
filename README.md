# Benvingut a titanic-ml

## Descripció
Aquesta pràctica s'ha realitzat per a l'assignatura de Tipologia i cicle de vida de les dades, del Màster en Ciència de Dades de la Universitat Oberta de Catalunya. Es fa ús de tècniques de machine learning sobre el dataset del titanic.

## Membres de l'equip
La pràctica ha sigut realitzada per Josep Tormo Costa i Oriol Bardés Robles.

## Fitxers
data/train.csv: fitxer original de training.
data/test.csv: fitxer original de test.
code/titanic.Rmd: programa principal. 
data/predictions.csv: fitxer csv amb les prediccions resultants.

## 1. Descripció del dataset

Aquest dataset sobre els passatgers del Titanic està integrat pels conjunts d'entrenament (891 registres) i de prova (418 registres) disponibles a Kaggle:

https://www.kaggle.com/c/titanic/data

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

## 2. Integració i selecció de les dades d'interés

D'entrada es consideraran tots els atributs presents en els conjunts d'entrenament i de prova. Naturalmnet, el conjunt d'entrenament serà usat per a construir el model predictiu 
de la supervivència i el conjunt de prova serà usat per a validar-lo.

Analitzarem en particular la relació dels següents paràmetres en la supervivència dels passatgers:

* Gènere del passatger
* Preu del bitllet
* Classe del bitllet
* Edat del passatger
* Port d'embarcament

Per tant, treballarem tots els camps i registres disponibles en el dataset en la secció corresponent a l'anàlisi de dades, on analitzarem la seva estructura i treballarem 
els valors buits existents en funció del camp. Fruit d'aquesta anàlisi, descartarem el camp de "Cabin" per considerar que no aporta informació relevant al treball. 
