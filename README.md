# 📧 Detection Spam

El proyecto trata de construir un modelo de Machine Learning capaz de clasificar si un email es spam o no.

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
