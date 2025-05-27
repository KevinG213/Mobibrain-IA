
# **Mobibrain: Predicción de Precios de Celulares con IA**

![Banner del Proyecto](/banner.png)

## **Autores**

*  Sofía Pinilla Diaz 2215607
*  Kevin Andres Gallardo Robles 2191918
*  Jenifer Karina Alfonso Carreño 2215109

## **Objetivo**

Desarrollar un sistema de predicción de precios de celulares basado en sus especificaciones técnicas, usando modelos de inteligencia artificial. Adicionalmente, se busca identificar segmentos del mercado mediante técnicas de clustering no supervisado.

## **Dataset**

Se utilizó el **Mobiles Dataset 2025 (Kaggle)**, que contiene 930 registros de dispositivos móviles.
Desafíos del dataset:

* Datos mixtos (texto, números, valores faltantes)
* Formatos inconsistentes
* Variables categóricas (como procesador)

🔗 [Enlace al dataset](https://www.kaggle.com/datasets/abdulmalik1518/mobiles-dataset-2025)

## **Modelos Usados**

### *Regresión (Supervisado):*

* **Decision Tree Regressor** → MAE: 113.08
* **Random Forest Regressor** → MAE: 92.12
* **Support Vector Regressor (SVR)** → MAE: 348.87
* **Redes Neuronales Densas (3 capas)** → MAE: 179.16

### *Clustering (No Supervisado):*

* **K-Means (k=3)**: Agrupación por gama (baja, media, alta)
* **DBSCAN**: Detección de nichos especializados (fotografía, gamer, batería extendida, etc.)

### *Reducción de Dimensionalidad:*

* **PCA (2 componentes)**: usado para visualización de clústeres

## **Preprocesamiento**

* Eliminación de columnas irrelevantes
* One-hot encoding para variables categóricas
* Normalización con StandardScaler

## **Validación**

* Entrenamiento: 80% del dataset
* Validación: 20% restante
* Se aplicó validación cruzada (k-fold) en algunos modelos
* Métrica principal: **MAE (Mean Absolute Error)**

## **Diapositivas**

📄 [Ver presentación en PDF](/diapositivas_ia.pdf)

## **Video**

🎥 [Ver video en YouTube](https://youtu.be/r2CkgOq-1oM?feature=shared)

## **Notebook Acumulativo**

📓 [Notebook en Google Colab](https://colab.research.google.com/drive/15dyaVM-k6vP8yekTtYJQiPsfcyC-8-DJ?usp=sharing)
