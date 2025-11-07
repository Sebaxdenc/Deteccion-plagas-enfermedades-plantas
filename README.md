# Sistema de IA para Detección de Enfermedades en Plantas

## Propósito del Proyecto

Este proyecto desarrolla un **sistema completo de inteligencia artificial** para la **detección automática de enfermedades en plantas** utilizando técnicas avanzadas de **deep learning** y **computer vision**. El objetivo es crear una herramienta práctica que pueda ayudar a agricultores y especialistas a identificar enfermedades en cultivos de manera rápida y precisa.

### Objetivos Principales
-  **Clasificación automática** de enfermedades en plantas usando imágenes
-  **Comparación de arquitecturas** de deep learning (CNN, Ensembles)
-  **Análisis exhaustivo** del rendimiento y robustez de los modelos
-  **Desarrollo de pipeline** completo desde datos hasta modelo productivo

## Dataset Utilizado

**TensorFlow Plant Village Dataset**
   - URL: https://www.tensorflow.org/datasets/catalog/plant_village
   - ~54,000 imágenes de plantas
   - 38 clases, 14 especies diferentes

## Estructura del Proyecto

```
ENTREGA3IA/
├──  NOTEBOOKS PRINCIPALES
│   ├── 01_preparacion_datos.ipynb       # Exploración y preprocessing
│   ├── 02_modelos_baseline.ipynb        # Modelos baseline (CNN, RF, SVM)
│   ├── 03_evaluacion_final.ipynb      
├──  NOTEBOOKS ANÁLISIS
│   ├── analisis_exploratorio_plantas.ipynb
├──  CONFIGURACIÓN
│   ├── requirements.txt                 # Dependencias del proyecto
│   ├── README.md                       # Este archivo
├──  DATOS
│   └── data/PlantDisease/              # Dataset Plant Village (~54k imágenes)

```

##  Aspectos Clave para la Ejecución

###  Configuración Inicial

 **Instalar dependencias**:
   ```bash
   pip install -r requirements.txt
   ```

###  Ejecución del Pipeline Completo

**ORDEN OBLIGATORIO** - Ejecutar notebooks secuencialmente:

```bash
# 1. Preparación de datos 
jupyter notebook 01_preparacion_datos.ipynb

# 2. Modelos baseline 
jupyter notebook 02_modelos_baseline.ipynb

# 4. Evaluación final
jupyter notebook 03_evaluacion_final.ipynb
```

##  Pipeline de Desarrollo

### 1. **Preparación de Datos** (01_preparacion_datos.ipynb)
-  **Exploración exhaustiva** del dataset Plant Village (~54k imágenes)
-  **Preprocessing avanzado**: redimensionado, normalización, augmentación
-  **Análisis estadístico** de distribución de clases y especies
-  **División estratificada** en train/validation/test (70/15/15)

### 2. **Modelos Baseline** (02_modelos_baseline.ipynb)  
-  **CNN Simple**: arquitectura básica para establecer baseline
-  **Random Forest**: modelo tradicional con características extraídas
-  **SVM**: Support Vector Machine para comparación
-  **Evaluación comparativa** con métricas estándar

### 3. **Evaluación Final** (03_evaluacion_final.ipynb)
-  **Análisis comparativo** completo de todos los modelos
-  **Interpretabilidad**: mapas de activación y análisis de errores
-  **Comparación con literatura** científica y estado del arte
-  **Recomendaciones para producción** y deployment


### Dataset Plant Village
-  **Total**: ~54,000 imágenes de alta calidad
-  **Clases**: 38 clases (14 especies, múltiples enfermedades)
-  **Especies**: Tomate, Papa, Pimiento, Manzana, Cereza, etc.
-  **Balance**: Moderadamente desbalanceado (manejable con técnicas apropiadas)

### Métricas de Evaluación
1.  **Accuracy**: Precisión general del modelo
2.  **F1-Score Macro**: Rendimiento balanceado por clase
3.  **Precision/Recall**: Crítico para aplicación médica
4.  **Matriz de Confusión**: Análisis detallado de errores

### Impacto y Aplicaciones
-  **Agricultura de precisión**: Detección temprana de enfermedades
-  **Apps móviles**: Herramienta para agricultores en campo
-  **Sistemas IoT**: Integración con cámaras automáticas
-  **Educación**: Herramienta de aprendizaje para estudiantes de agronomía

## 👨‍💻 Autores

**Sebastián Medina**
**Samuel De Ossa**
**Alejandro Sepulveda Posada**
Proyecto desarrollado para la materia de **Inteligencia Artificial**  
Universidad: Eafit 

---
