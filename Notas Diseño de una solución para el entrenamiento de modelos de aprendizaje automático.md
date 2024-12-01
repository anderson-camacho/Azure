# Diseño de una solución para el entrenamiento de modelos de aprendizaje automático

## Objetivos de aprendizaje

- Identificar tareas de aprendizaje automático.
- Elegir un servicio adecuado para entrenar un modelo.
- Seleccionar las opciones de cómputo más eficientes.

---

## Proceso de aprendizaje automático

El aprendizaje automático sigue un flujo estructurado dividido en seis pasos principales:

### 1. **Definir el problema**
   - Identifica qué debe predecir el modelo.
   - Establece criterios para determinar el éxito del modelo.

### 2. **Obtener los datos**
   - Encuentra las fuentes de datos necesarias.
   - Asegúrate de tener acceso adecuado a los datos.

### 3. **Preparar los datos**
   - Explora y analiza los datos disponibles.
   - Limpia y transforma los datos según los requisitos del modelo.

### 4. **Entrenar el modelo**
   - Selecciona un algoritmo adecuado.
   - Ajusta hiperparámetros mediante prueba y error.

### 5. **Integrar el modelo**
   - Implementa el modelo en un punto final para que pueda generar predicciones.

### 6. **Monitorear el modelo**
   - Realiza un seguimiento constante del rendimiento y precisión del modelo.

📌 [Referencia gráfica del proceso](https://learn.microsoft.com/en-us/training/wwl-data-ai/design-machine-learning-model-training-solution/media/machine-learning-process.png)

---

## Tareas comunes de aprendizaje automático

1. **Clasificación:** Predicción de valores categóricos (ejemplo: spam/no spam).
2. **Regresión:** Predicción de valores numéricos continuos (ejemplo: precio de una vivienda).
3. **Previsión de series de tiempo:** Predicción de valores futuros basados en datos históricos (ejemplo: ventas mensuales).
4. **Visión por computadora:** Clasificación o detección de objetos en imágenes.
5. **Procesamiento del lenguaje natural (PNL):** Análisis y extracción de ideas del texto.

---

## Servicios comunes en Azure para entrenamiento de modelos

| Servicio                  | Descripción                                                                                                                                      |
|---------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------|
| **Azure Machine Learning** | Solución integral para entrenar y gestionar modelos. Ofrece una experiencia con UI (Azure Studio) o programación (SDK de Python/CLI).          |
| **Azure Databricks**      | Plataforma para ciencia de datos y análisis con Spark, útil para grandes volúmenes de datos y modelos distribuidos.                            |
| **Azure Synapse Analytics** | Servicio de análisis a escala que soporta modelos en Spark (MLlib) y la integración con Azure Machine Learning.                               |
| **Azure AI Services**     | Modelos preentrenados accesibles mediante API para tareas comunes como detección de objetos, con opción de personalización.                     |

---

## Selección de cómputo: CPU vs GPU

- **CPU:** Adecuada para conjuntos de datos tabulares pequeños. Es más económica.
- **GPU:** Recomendada para datos no estructurados como imágenes o texto. Proporciona mayor potencia y velocidad.

---

### Notas adicionales

- Evalúa siempre la relación costo-beneficio del servicio y el tipo de cómputo según el caso de uso.
- Azure Machine Learning es la opción más flexible para escenarios personalizados, mientras que Azure AI Services es ideal para soluciones rápidas con modelos preentrenados.

---
