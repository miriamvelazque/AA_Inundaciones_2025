# Predicción del Tipo de Afectación en Zonas Inundables – Proyecto de Aprendizaje Automático

Este repositorio documenta el desarrollo de un modelo de clasificación supervisada para identificar el tipo de afectación (total o parcial) en zonas inundables, utilizando variables geoespaciales, ambientales y sociales.

---

## 🎯 Objetivo del Proyecto

Desarrollar un modelo de clasificación binaria que permita distinguir entre zonas inundables **totalmente afectadas** y aquellas **parcialmente afectadas**, a partir de variables ambientales y sociales extraídas de fuentes públicas.


### Objetivos específicos:
- Integrar datos públicos sobre zonas inundables, curvas de nivel y factores sociales relevantes para el modelado supervisado.
- Extraer características relevantes para el modelado supervisado.
- Entrenar y evaluar modelos de clasificación con métricas como precisión, recall y F1-score.
- Presentar resultados visuales e interpretables que aporten valor al análisis territorial.

---

```
## 📁 Estructura del Repositorio

AA_Inundaciones_2025/ ├── data/ │ ├── raw/ # Datos originales (.csv, .geojson, .tiff) │ └── processed/ # Dataset limpio para modelado ├── notebooks/ │ ├── 01_EDA.ipynb # Análisis exploratorio │ └── 02_Modelos.ipynb # Modelado supervisado ├── src/ │ ├── features/ # Funciones para ingeniería de variables │ └── models/ # Entrenamiento y evaluación ├── reports/ │ └── figures/ # Gráficos generados ├── environment.yml # Entorno reproducible ├── README.md # Documentación del proyecto
```

## 📊 Dataset

Se utilizaron datos públicos provenientes de:

- DU-Tech (datos.gob.ar)
- RENABAP (01/10/2025)
- Curvas de nivel (.geojson)
- Datos meteorológicos (.csv)

Los archivos originales se encuentran en `data/raw/` y el dataset procesado para modelado en `data/processed/`.

---

## 🧪 Modelado y Evaluación

> *Esta sección será completada en la Entrega 3.*

- Algoritmos utilizados: *(por definir)*
- Librería principal: `scikit-learn`
- Métricas evaluadas: Accuracy, Precision, Recall, F1-score
- Visualizaciones: Matriz de confusión, curvas ROC, importancia de variables

---

## 📌 Entregas

Este proyecto se desarrolló en tres entregas:

1. **Entrega 1**: Formulación del objetivo y contexto del problema
2. **Entrega 2**: Descripción del dataset y origen de los datos
3. **Entrega 3**: Presentación del modelo, análisis exploratorio y resultados

La entrega final incluye este repositorio, los notebooks, los datasets, el video explicativo y la documentación completa.

---

## ✍️ Autora

**Miriam Velazquez**  
Estudiante de la Tecnicatura de Ciencias de Datos e Inteligencia Artificial  
Politécnico Malvinas Argentinas

---

## ⚠️ Nota Académica

Este proyecto es original y cumple con las pautas del parcial. No se permite el plagio ni la copia de trabajos previos. Cualquier similitud con otros proyectos es mera coincidencia.

---

<small>Proyecto basado en la plantilla <a href="https://drivendata.github.io/cookiecutter-data-science/" target="_blank">Cookiecutter Data Science</a>.</small>
tar resultados visuales e interpretables que aporten valor al análisis territorial.
