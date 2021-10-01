# Heart Failure Prediction a Classification Problem

Los accidentes cardiovasculares son la principal causa de muerte en el mundo. Es importante entender que dados ciertos padecimientos o caracteristicas de cada individuo lo vuelven mas propenso a desarrollar un accidente cardiovascular, dado lo anterior una identificación temprana de un posible riesgo podría marcar una diferencia significatíva.

## Objetivo 
Elaborar un algoritmo predictivo basado en un modelo de clasificación, el cual debe considerar las carácteristicas más adecuadas y estár optimizado para obtener el menor numero de falsos negativos posible. Lo anterior se complementará mediante una interfáz grafica que permita el input de datos y arroje una predicción.

## Descripción del repositorio
**01_Exploracion.ipynb** contiene la visualización y descripción de los datos antes del procesamiento.

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
