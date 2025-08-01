# Introducción al Aprendizaje Automático – Trabajo Práctico Final

Este repositorio contiene el trabajo práctico final realizado para la materia **Introducción al Aprendizaje Automático**, correspondiente al plan de estudios de la **Licenciatura en Ciencia de Datos** de la **Universidad Nacional de San Martín (UNSAM)**, cursada durante el año 2024.

---

## 📌 Título del trabajo

**Clasificación de Gliomas con Técnicas de Aprendizaje Automático**

---

## 📋 Descripción

El objetivo principal del trabajo fue desarrollar un modelo capaz de clasificar dos tipos de gliomas (tumores cerebrales):  
- **Gliomas de Bajo Grado (LGG)**  
- **Glioblastoma Multiforme (GBM)**  

Para ello se utilizaron datos genéticos y clínicos de pacientes, aplicando técnicas de aprendizaje automático para construir y comparar modelos predictivos.

---

## 📂 Contenido del repositorio

- `dataset TCGA_InfoWithGrade.csv`: dataset utilizado, que contiene 839 registros con información genética y clínica sobre pacientes con gliomas.
- `Trabajo Práctico Clasificación Gliomas.pdf`: informe completo con el desarrollo del trabajo.
- `Presentación TP Clasificación Gliomas.pdf`: presentación en formato PDF utilizada para exponer el trabajo final.

---

## 🧪 Dataset

El dataset fue obtenido del **National Cancer Institute (EE.UU.)** e incluye información como:
- Edad, género y etnia de los pacientes
- Tipo de glioma (target binario: LGG o GBM)
- Presencia o ausencia de mutaciones en genes específicos: `IDH1`, `TP53`, `ATRX`, `PTEN`, `EGFR`, `CIC`, entre otros

---

## 🧠 Modelos y técnicas utilizadas

- Árboles de decisión con diferentes combinaciones de atributos
- Random Forest
- Regresión logística (comparativa)
- Benchmark con dummy classifier

Se evaluaron distintas métricas para comparar el rendimiento: **Accuracy, Recall y Precisión**, priorizando la **minimización de falsos negativos** (especialmente importante para la detección del tipo más agresivo: GBM).

---

## 🔍 Resultados

- El gen **IDH1** se destacó como el mejor predictor individual del tipo de glioma.
- El modelo seleccionado fue un **árbol de decisión utilizando únicamente la mutación de IDH1**, por su buena capacidad de recall y simplicidad.
- Se propuso como trabajo futuro repetir el análisis excluyendo IDH1 para explorar el aporte de otros genes.

---

## 👩‍💻 Herramientas utilizadas

- **Python** y librerías: `pandas`, `scikit-learn`, `matplotlib`, `seaborn`
- **Jupyter Notebooks**

---

## ✏️ Autoría

**Micaela Floridia**  
Licenciatura en Ciencia de Datos – UNSAM  
Trabajo en conjunto con Vanessa Galeano y Leandro Villanueva (grupo conformado por compañeros de cursada de la materia)

---

## 📎 Licencia

Este repositorio fue desarrollado con fines académicos y no comerciales.
