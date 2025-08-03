# 🧠 BreastCancer-MLPClassifier

## Clasificación binaria de tumores mamarios con red neuronal MLP

Este proyecto implementa una red neuronal Multilayer Perceptron (MLP) básica para clasificar tumores como benignos o malignos, usando el dataset [Breast Cancer Wisconsin (Diagnostic)](https://www.kaggle.com/uciml/breast-cancer-wisconsin-data). Se aplican técnicas de preprocesamiento, entrenamiento supervisado y evaluación con enfoque visual e interpretativo.

---

## Técnicas utilizadas

- Normalización de características con `StandardScaler`
- Arquitectura MLP:
  - Capa oculta de 32 neuronas (ReLU)
  - Capa de salida con función sigmoide
- Función de pérdida: `binary_crossentropy`
- Optimizador: `Adam`
- Entrenamiento: 50 épocas con monitoreo de métricas
- Visualización de curvas de pérdida y precisión
- Métricas: accuracy, F1-score, recall, matriz de confusión

---

## Resultados

### Histogramas de entrada  
- La mayoría de las variables presentan distribución aproximadamente normal.  
- Algunas características conservan sesgo leve, lo que puede afectar la modelación.

### Evolución de precisión  
- **Entrenamiento**: Comienza en 99.5% y llega a 100% rápidamente.  
- **Validación**: Fluctúa entre 98–99%, indicando buena generalización con leve variabilidad.

### Evolución de la pérdida  
- **Entrenamiento**: Disminuye hasta ≈0.01, indicando buen ajuste.  
- **Validación**: Tiende a subir ligeramente y se estabiliza en ≈0.06 → posible inicio de sobreajuste.

### Matriz de confusión  
| Predicción       | Casos correctos | Errores         |
|------------------|------------------|------------------|
| Benigno          | 72               | 0 falsos positivos |
| Maligno          | 41               | 1 falso negativo   |

> El modelo clasifica ambos tipos de tumores con alta precisión. La ausencia de falsos positivos es clave en contextos médicos.

---

## Conclusión

La MLP básica demuestra ser efectiva para datos tabulares médicos. Modela relaciones no lineales entre variables y logra alta precisión en la clasificación binaria.

---

## Posibles mejoras

- Regularización (`L2`, `Dropout`) para controlar sobreajuste  
- Ajuste del umbral de clasificación para balancear errores  
- Reducción de dimensionalidad con **PCA**  
- Optimización avanzada con `GridSearchCV` u `Optuna`

---

## 👤 Conéctate conmigo

[![Conectar en LinkedIn](https://img.shields.io/badge/LinkedIn-Conectar-blue?logo=linkedin&style=flat-square)](https://www.linkedin.com/in/daniel-araneda-yasic)

¿Eres reclutador o profesional del sector interesado en proyectos aplicados de Data Science, visualización de datos o inteligencia artificial eficiente?  
Este proyecto refleja mi enfoque técnico y comunicativo, y estoy abierto a oportunidades laborales, colaboración en equipos multidisciplinarios y desarrollo de soluciones prácticas y reproducibles.

📫 No dudes en contactarme para conversar sobre cómo puedo aportar valor desde la intersección entre análisis técnico, creatividad visual y documentación didáctica.



