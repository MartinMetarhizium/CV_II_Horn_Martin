
# Clasificación de Cáncer de Pulmón y Colon mediante Deep Learning

Este proyecto implementa distintos modelos de deep learning para clasificar imágenes histopatológicas de tejido pulmonar y colónico en cinco clases, incluyendo distintos tipos de cáncer y tejido benigno.  
Se utilizan modelos personalizados como `VGGStyleModel`, `SimpleCNN`, `TinyCNN`, junto con técnicas como validación cruzada (k-fold), visualizaciones y métricas detalladas.

---

## 📁 Dataset

- **Fuente**: [Kaggle - Lung and Colon Cancer Histopathological Images](https://www.kaggle.com/datasets/andrewmvd/lung-and-colon-cancer-histopathological-images)
- **Clases:**
  - `colon_aca`: Adenocarcinoma de colon  
  - `colon_n`: Tejido benigno del colon  
  - `lung_aca`: Adenocarcinoma de pulmón  
  - `lung_n`: Tejido benigno pulmonar  
  - `lung_scc`: Carcinoma de células escamosas de pulmón

---

## 🧠 Modelos

| Modelo        | Capas            | Accuracy (aprox.) |
|---------------|------------------|-------------------|
| `TinyCNN`     | 1 Conv + 1 FC    | 20%               |
| `SimpleCNN`   | 2 Conv + 2 FC    | >99%              |
| `VGGStyle`    | 5 Conv + 3 FC    |  >99%             |

> Se prueba la capacidad de modelos de distintas complejidades para evaluar la clasifición entre 5 clases del dataset propuesto.

---

## 📊 Evaluación

- **Métricas:** Precisión, Recall, F1-score, Matriz de Confusión  
- **Validación Cruzada (k=5):** para evaluar estabilidad del modelo  
- **Errores tipo I y II:** identificados en el análisis médico

---

## 📈 Visualizaciones

- Distribución de imágenes por clase  
- Curvas de entrenamiento y validación  
- Comparación entre modelos  
- Arquitectura de red y conteo de parámetros

---

## ⚙️ Requisitos

```bash
pip install torch torchvision matplotlib seaborn scikit-learn torchsummary
```

---

## 📦 Estructura

```
├── CNNmodels.ipynb                     # Script principal
└── README.md
```

---

## 🧑‍💻 Autor

**Martín Horn** – Clasificación de imágenes biomédicas con redes convolucionales.
