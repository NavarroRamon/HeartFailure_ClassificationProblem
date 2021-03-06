# Heart Failure Prediction a Classification Problem

Los accidentes cardiovasculares son la principal causa de muerte en el mundo. Es importante entender que dados ciertos padecimientos o caracteristicas de cada individuo lo vuelven mas propenso a desarrollar un accidente cardiovascular, dado lo anterior una identificación temprana de un posible riesgo podría marcar una diferencia significatíva.

## Objetivo 
Elaborar un algoritmo predictivo basado en un modelo de clasificación, el cual debe considerar los factores de riesgo más adecuados y estár optimizado para obtener el menor numero de falsos negativos posible. Lo anterior se complementará mediante una interfáz grafica que permita el input de datos y arroje una predicción.

## Descripción del repositorio
| Archivo | Descripcion |
| ------ | ----------- |
|[**data/df_heartfailure.csv**](https://github.com/NavarroRamon/HeartFailure_ClassificationProblem/blob/main/data/df_heartfailure.csv)| Archivo de datos, con el dataset filtrado.|
|[**01_Exploracion.ipynb**](https://github.com/NavarroRamon/HeartFailure_ClassificationProblem/blob/main/01_Exploracion.ipynb)| Contiene la visualización y descripción de los datos antes del procesamiento.|
|[**02_Preprocessing.ipynb**](https://github.com/NavarroRamon/HeartFailure_ClassificationProblem/blob/main/02_Preprocessing.ipynb)| El procedimiento para filtrar los valores que no eran necesarios.|
|[**03_HeartDisease_EDA.html**](https://github.com/NavarroRamon/HeartFailure_ClassificationProblem/blob/main/03_HeartDisease_EDA.html)| Contiene un primer análisis exploratorio de los datos ya filtrados.|
|[**04_ModeloML.ipynb**](https://github.com/NavarroRamon/HeartFailure_ClassificationProblem/blob/main/04_ModeloML.ipynb)| Modelo con validación, caracteristicas de mayor peso, matriz de confusión y reporte de clasificación.|

## Resultados

El modelo implementado fue **Random Forest Classifier**, con el que se obtuvo un **92% de presición para detectar casos negativos** y **89% para casos positivos**. 
<!Los parámetros del modelo se pueden ver en la siguiente tabla>


A partir de la matríz de confusión se observa que la presición tiende a ser mejor cuando se habla de un caso negativo.
<img src="https://cdn.discordapp.com/attachments/843776650495393855/895824902333018142/mc0.png"
     width="400" 
     height="350"
     alt="Confussion matrix"
     style="float: left; margin-right: 100px;" />

Para el problema especifico que se está tratando es posible refinar el modelo para obtener una mayor presición en casos positivos y reducir el numero de falsos negativos, aún si eso implica reducir la presición general del modelo.



## Acerca del Dataset
Se trabajó con un dataset obtenido a través de kaggle el cual consiste en una recopilación de diferentes datasets disponibles de forma independiente. Las características que contiene el data set son:

1. Age: age of the patient [years]
2. Sex: sex of the patient [M: Male, F: Female]
3. ChestPainType: chest pain type [TA: Typical Angina, ATA: Atypical Angina, NAP: Non-Anginal Pain, ASY: Asymptomatic]
4. RestingBP: resting blood pressure [mm Hg]
5. Cholesterol: serum cholesterol [mm/dl]
6. FastingBS: fasting blood sugar [1: if FastingBS > 120 mg/dl, 0: otherwise]
7. RestingECG: resting electrocardiogram results [Normal: Normal, ST: having ST-T wave abnormality (T wave inversions and/or ST elevation or depression of > 0.05 mV), LVH: showing 8. probable or definite left ventricular hypertrophy by Estes' criteria]
9. MaxHR: maximum heart rate achieved [Numeric value between 60 and 202]
10. ExerciseAngina: exercise-induced angina [Y: Yes, N: No]
11. Oldpeak: oldpeak = ST [Numeric value measured in depression]
12. ST_Slope: the slope of the peak exercise ST segment [Up: upsloping, Flat: flat, Down: downsloping]
13. HeartDisease: output class [1: heart disease, 0: Normal]


Referencia: fedesoriano. (September 2021). Heart Failure Prediction Dataset.
Retrieved [25/09/21] from https://www.kaggle.com/fedesoriano/heart-failure-prediction.
