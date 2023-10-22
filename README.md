# CEIA - UBA - Procesamiento de Lenguaje Natural
Año 2023

Docente: Rodrigo Cárdenas

**Alumno: Santiago Gonzalez Achaval**

## Presentación

En este repositorio se encuentran los desafíos realizados durante la cursada de la materia Procesamiento del Lenguaje Natural de la Especialización en Inteligencia Artificial de la UBA.



## Conceptos aplicados
- Vectorización: Frecuencias, One Hot Encoding, TF-IDF
- Similaridad Coseno
- Steamer / Lematizador
- Tokenización
- Modelos de Deep Learning
- Redes Neuronales Recurrentes
- LSTM - GRU
- Embeddings
- Beam Search
- Balanceo de Dataset (OverSampling / Undersampling)
- Data augmentation
- Modelo Encoder-Decoder

## Librerías utilizadas
- numpy
- nltk
- gradio
- sklearn
- stanza
- spacy_stanza
- tensorflow
- keras
- seaborn
- matplotlib
- pickle
- pandas
- nlpaug
- gensim
- gdown

## Lenguaje

Python

## Embeddings pre-entrenados
- GenSim - Word2Vec
- Glove
- Fasttext

## Desafío 1 - Vectorización y Similaridad entre documentos:
En este desafío se programan manualmente las funciones para obtener el vocabulario de un corpus y vectorizar por OneHot encoding, Vector de frecuencia y TF-IDF.
Tambien se realiza la similitud coseno entre un string ingresado por el usuario y los datos del corpus.


[Link al Desafío 1](https://github.com/SantiagoGonzalezAchaval/procesamiento_lenguaje_natural/blob/main/clase_1/ejercicios/1a%20-%20vectorizacion.ipynb)

## Desafío 2 - Búsqueda en Corpus y Bot de preguntas y respuestas predeterminadas:

En este desafío se toma como corpus un artículo de Wikipedia que habla sobre el futbol (hhttps://en.wikipedia.org/wiki/History_of_association_football), se limpia y preprocesa, y se utilizan librerías de NLTK para tokenizar el corpus.
Luego se programa una función que recibe una pregunta del usuario y busca en el corpus el documento que tiene mas similaridad coseno con el texto ingresado (utilizando vectorización TF-IDF) y lo devuelve.

[Link al Desafío 2 - NLTK](https://github.com/SantiagoGonzalezAchaval/procesamiento_lenguaje_natural/blob/main/clase_2/ejercicios/Bot_Santi.ipynb)


## Desafío 3 - Embeddings:


El objetivo de este desafío fue utilizar un corpus base para crear embeddings de palabras basados en ese contexto.
Utilizamos un dataset de fake news que se preprocesó y se utilizó la libreria Gensim (Word2Vec) para entrenar el modelo generador de Embeddings. 

[Link al Desafío 3 - EMBEDDINGS](https://github.com/SantiagoGonzalezAchaval/procesamiento_lenguaje_natural/blob/main/clase_3/ejercicios/Gensim%20Santi.ipynb)

## Desafío 4 - Predicción de próximas palabras:

El objetivo de este desafio era predecir la proxima palabra en una frase. Se utilizo un dataset de libros escritos por Hernandez. El mismo fue procesado y formateado en secuencia de 4 palabras donde las 3 primeras se utilizaban como referencia y la ultima se intentaba predecir.
Con ese set de datos se entrenó un modelo de Red Neuronal Recurrente para que devuelva un vector softmax con la probabilidad de cada una de las palabras del vocabulario.
El modelo no tuvo un buen resultado general, mas que nada por no contar con suficientes datos y recursos computacionales mejores.


[Link al Desafío 4 - PROXIMA PALABRA](https://github.com/SantiagoGonzalezAchaval/procesamiento_lenguaje_natural/blob/main/clase_4/ejercicios/predicci%C3%B3n_palabra.ipynb)

## Desafío 5 - Análisis de Sentimientos:

En este desafío se analizaron críticas de compradores de ropa para clasificar el comentario del 1 al 5 en cuanto a la satisfacción del cliente.
Se utilizó el dataset "clothing_ecommerce_reviews.csv" que contiene criticas con clasificaciones del 1 al 5. Este se limpió, se preprocesó y se tokenizó, para armar secuencias de entrada a un modelo de Red Neuronal Recurrente.
Dentro de cada notebook se comparan modelos que entrenan sus propios embeddings contra modelos que utilizan embeddings pre-entrenados por Fasttext.
El dataset se encuentra gravemente desbalanceado por lo que los resultados no fueron muy buenos. Se podria mejorar el resultado balanceando el dataset o utilizando una funcion de perdida que compense en cierta medida este desbalance.

[Link al Desafío 5 - CLASIFICACION DE SENTIMIENTOS DE 1 A 5](https://github.com/SantiagoGonzalezAchaval/procesamiento_lenguaje_natural/blob/main/clase_5/ejercicios/5%20-%20clothing_ecommerce_reviews.ipynb)

## Desafío 6 - Bot Conversacional:

En este desafío se construye un Bot conversacional que responde preguntas del usuario. Se utilizan como base los datos del challenge ConvAI2 (Conversational Intelligence Challenge 2) de conversaciones en inglés (http://convai.io/data/). Se preprocesa y se limpian los datos, y se entrena un modelo Encoder-Decoder que utiliza los embeddigns pre-entrenados de Glove.

[Link al Desafío 6 - BOT CONVERSACIONAL](https://github.com/SantiagoGonzalezAchaval/procesamiento_lenguaje_natural/blob/main/clase_6/ejercicios/6-%20bot_qa.ipynb)

# Contacto
santigonzalezachaval@gmail.com
