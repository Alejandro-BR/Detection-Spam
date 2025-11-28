# 📧 Detection Spam

El objetivo de este proyecto es desarrollar un sistema de clasificación automática capaz de distinguir entre correos electrónicos normales (ham) y correos electrónicos no deseados (spam).

## Obtención de datos

**Fuente del dataset original:** [Spam Mails Dataset](https://www.kaggle.com/datasets/venky73/spam-mails-dataset/data?select=spam_ham_dataset.csv)

**Dataset:** [spam_ham_dataset.csv](/data/spam_ham_dataset.csv)

Parte de los emails `ham` (no spam) proviene del **Enron Corpus**, una base de datos pública de correos reales de empleados de la empresa Enron.

![label](/img/label.png)

El dataset cuenta con 4 columnas y 5171 filas.

El target que se busca predecir es `label_num`, es decir, si un correo es `spam = 1` o `ham = 0`.

| Columnas | Tipo de dato | Descripción |
| :----- | :----- | :----- |
| Unnamed: 0 | int64 | Indice antiguo (desconocido) |
| label | object | `spam` / `ham` |
| text | object | Cuerpo del email |
| label_num | int64 | `spam` = 1 / `ham` = 0 |

## Dataset resultante

El dataset cuenta con 2 columnas y 5171 filas.

El target que se predece es `is_spam`, es decir, si un correo es `spam = 1` o `ham = 0`.

| Columnas | Tipo de dato | Descripción |
| :----- | :----- | :----- |
| text | object | Cuerpo del email |
| is_spam | int64 | `spam` = 1 / `ham` = 0 |

![nube de palabras](/img/nube.png)

## Modelo de machine learning

Después de evaluar todos los modelos, el que tuvo mejores resultados fue el `LinearSVC` con una precisión del **98.65%**, también muy cerca tenemos al `Logistic Regression`, ambos tienen mejores resultado que el resto de algoritmos.

![linear_svc](/img/linear_svc.png) 

![accuracy](/img/accuracy.png) 

## Google Colab

[Cuaderno jupyter](https://colab.research.google.com/drive/1a3b8UWTQ0CzpIkR-b7MzMVBhwbr4EvJl?usp=sharing)

## Creditos:

* [Alejandro Barrionuevo Rosado](https://github.com/Alejandro-BR)
* [Elías Robles Ruiz](https://github.com/eliasrrobles)

Máster de FP en Inteligencia Artifical y Big Data - CPIFP Alan Turing

<img src="./img/alan_turing.png" width="150"/>