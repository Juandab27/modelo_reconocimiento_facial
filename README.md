# 🧠 Modelo de Reconocimiento Facial

<p align="center">
Proyecto de clasificación facial utilizando Transfer Learning con MobileNetV2 y TensorFlow
</p>

---

## 📖 Descripción

Este proyecto implementa un sistema de **reconocimiento/clasificación facial** utilizando **Deep Learning** y la técnica de **Transfer Learning** con el modelo preentrenado **MobileNetV2**.

El modelo fue entrenado para identificar diferentes clases/personas a partir de imágenes organizadas en carpetas, utilizando `ImageDataGenerator` para el procesamiento y aumento de datos.

El proyecto incluye:

* 📂 Preparación y carga de dataset
* 🧠 Construcción del modelo con MobileNetV2
* 🔄 Entrenamiento con callbacks (EarlyStopping, ReduceLROnPlateau)
* 📊 Evaluación con métricas de clasificación
* 📈 Matriz de confusión y reporte detallado

---

## 🛠️ Tecnologías Utilizadas

* Python
* TensorFlow / Keras
* MobileNetV2 (Transfer Learning)
* NumPy
* Matplotlib
* Scikit-learn

---

# 📂 Estructura del Proyecto

```bash
Reconocimiento_Facial/
│
├── Reconocimiento_facial.ipynb
├── dataset/
│   ├── dataser/
│   │   ├── nombre1/
│   │   ├── nombre2/
│   │   └── ...
│   ├── pruebas/
│   │   ├── nombre1/
│   │   ├── nombre2/
│   │   └── ...
│
├── requirements.txt
└── README.md
```

---

# 🚀 Instalación y Ejecución

## 1️⃣ Clonar el repositorio

```bash
git clone https://github.com/TU_USUARIO/reconocimiento_facial.git
```

---

## 2️⃣ Entrar a la carpeta del proyecto

```bash
cd reconocimiento_facial
```

---

## 3️⃣ Instalar dependencias

```bash
pip install -r requirements.txt
```

Si no tienes el archivo `requirements.txt`, instala manualmente:

```bash
pip install tensorflow numpy matplotlib scikit-learn
```

---

## 4️⃣ Ejecutar el Notebook

```bash
jupyter notebook
```

Luego abre:

```
Reconocimiento_facial.ipynb
```

Ejecuta las celdas en orden para entrenar y evaluar el modelo.

---

# 🧠 Arquitectura del Modelo

El proyecto utiliza **MobileNetV2** como base preentrenada (ImageNet), eliminando la capa superior y agregando:

* GlobalAveragePooling2D
* Capas Dense
* Dropout para regularización
* Capa final con activación Softmax

Se aplicó Transfer Learning para mejorar el rendimiento con menor cantidad de datos y tiempo de entrenamiento.

---

# 📊 Evaluación

El modelo se evalúa utilizando:

* Classification Report
* Confusion Matrix
* Accuracy
* Métricas por clase

---

# 👨‍💻 Autor

Proyecto desarrollado en equipo como parte del curso de Inteligencia Artificíal.

Mi rol en el proyecto:
- Responsable del desarrollo técnico y entrenamiento del modelo

---
