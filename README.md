# Trabajo Práctico 1 - Aprendizaje Automático 2 (AA2)

Este repositorio contiene la resolución del Trabajo Práctico N°1 para la materia **Aprendizaje Automático 2**. El objetivo principal es la implementación y optimización de **Redes Neuronales Feed Forward (MLP)** utilizando **PyTorch** para abordar distintos tipos de problemas: Clasificación Binaria, Clasificación Multiclase y Regresión.

## 📂 Estructura del Proyecto

El proyecto se divide en tres carpetas principales, una por cada problema abordado:

*   **`Problema1/` - Clasificación Binaria**: 
    *   **Dataset**: `healthcare-dataset-stroke-data.csv`.
    *   **Objetivo**: Predicción de accidentes cerebrovasculares basándose en variables clínicas y demográficas.
    *   **Técnicas**: Manejo de desbalance con SMOTE, optimización de hiperparámetros con Optuna.

*   **`Problema2/` - Clasificación Multiclase**:
    *   **Dataset**: Fashion MNIST (archivos `.idx3-ubyte` en `/datasets`).
    *   **Objetivo**: Clasificación de artículos de vestimenta en 10 categorías diferentes.
    *   **Técnicas**: Normalización de imágenes, arquitectura multicapa y evaluación de matrices de confusión.

*   **`Problema3/` - Regresión**:
    *   **Dataset**: `superstore.csv`.
    *   **Objetivo**: Predicción de una variable continua (ventas/ganancias) en un contexto de retail.
    *   **Técnicas**: Preprocesamiento de variables categóricas y numéricas, ajuste de funciones de pérdida de regresión.

*   **`Informe_TP1_AA2.pdf`**: Informe detallado con el análisis de cada problema, decisiones de diseño y conclusiones.

---

## 🛠️ Configuración y Ejecución

### 1. Requisitos Previos
Es necesario contar con Python instalado (recomendado 3.10+). Las dependencias incluyen PyTorch, Pandas, Scikit-Learn y Optuna.

### 2. Creación del Entorno Virtual (venv)
El trabajo fue diseñado para ejecutarse en un entorno virtual configurado a partir del `requirements.txt`.

```powershell
# Crear el entorno virtual
python -m venv venv

# Activar el entorno (Windows)
.\venv\Scripts\activate

# Activar el entorno (Linux/macOS)
source venv/bin/activate
```

### 3. Instalación de Dependencias
Una vez activado el entorno, instale las librerías necesarias:

```bash
pip install -r requirements.txt
```

---

## ⚙️ Configuración de Variables de Entorno (`.env`)

Para facilitar la portabilidad y configuración del proyecto, se recomienda crear un archivo `.env` en la raíz. Aunque los notebooks manejan rutas relativas por defecto, puede definir variables personalizadas.

Para generar el archivo:
1. Cree un archivo llamado `.env` en la carpeta raíz.
2. Agregue las variables que desee configurar, por ejemplo:

```ini
# Configuración de rutas y parámetros
DATA_PATH_P1="./Problema1/healthcare-dataset-stroke-data.csv"
DATA_PATH_P2="./Problema2/datasets/"
DATA_PATH_P3="./Problema3/superstore.csv"
GLOBAL_SEED=20
```

---

## 🚀 Ejecución de Notebooks
Cada carpeta contiene un archivo `.ipynb`. Puede ejecutarlos utilizando Jupyter Notebook o VS Code:

```bash
jupyter notebook
```

---
**Integrantes - Grupo 2**
Materia: Aprendizaje Automático 2
TUIA - 2026
