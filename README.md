# **Práctica de LLM Engineering – Guillermo Barrio**

Esta es la memoria de la práctica de LLM Engineering de Guillermo Barrio. En esencia, la práctica consiste en la creación de un dataset sintético a partir de uno que contiene datos electorales, todos públicos, para con el hacer el finetuning de dos modelos pre entrenados: T5 y Gemma2-9b.

He intentado sin mucho éxito hacer el RAG necesario para que el modelo ya ‘finetuneado’ tenga el contecto adecuado. 

**Todos los procesos que he seguido se describen en esta memoria de la práctica, Practica_LLM_Engineering_Guillermo-Barrio.pdf, que se recomienda leer primero.**

En el repositorio de GitHub se encuentran los ficheros que se pueden subir a él, y son los siguientes:

-	Notebooks utilizados para generar el dataset sintético, dividido en tres niveles: **Generador_dataset_nivel1.ipynb, Generador_dataset_nivel2.ipynb, Generador_dataset_nivel3.ipynb, Unificador_Dataset.ipynb**

-	Datasets sintéticos de cada nivel: **dataset_preguntas_nivel1.jsonl, dataset_preguntas_nivel2.jsonl, dataset_nivel3.jsonl**

-	Carpeta con los datasets ya unificados y divididos entre train, test y validación: **dataset_t5_final**

-	Notebooks utilizados en el finetuning de los modelos pre entrenados: **Fine_Tuning_T5.ipynb, Fine_Tuning_T5_ajustado.ipynb, Unsloth_Gemma-2-9b.ipynb**

-	Notebooks con el intento parcialmente fallido del sistema de RAG: **RAG_Gemma_2-9b.ipynb, RAG_Gemma2_Muy-Simple.ipynb**

En la **carpeta de mi Google Drive** en este enlace:

https://drive.google.com/drive/folders/17xqEubwo6Y5BiRf1eG1WmQd4-GFiMC10?usp=sharing

se encuentran todos los ficheros anteriores, además de otros que, por su tamaño, no hemos podido subir al repositorio:

-	Dataset original de los datos electorales: **df_elecciones_19.csv**

-	Carpetas del modelo T5 tras el finetuning: **t5_electoral_safe_20260203-1558, t5_electoral_safe_20260203-1558_final_eval**

-	Carpetas del modelo Gemma2 tras el finetuning: **modelo-Gemma_2-9b_finetuned, modelo-Gemma_2-9b_finetuned-8bit, modelo-Gemma_2-9b_finetuned-4bit,** aunque las dos primeras se grabaron con defectos, por lo que, de cara al RAG hemos utilizado el 4 bit.

-	Ficheros relacionados con el sistema de RAG fallido: **la carpeta electoral_rag_system, electoral_knowledge_base.pkl, electoral_knowledge_base.faiss**

-	Otros ficheros como el material de clase, las imágenes en formato .pmg de los errores del finetuning del modelo Gemma2, o ficheros .json, creados por el código ademá de los .jsonl, que no intervienen de todas formas en la práctica.

Gracias!

