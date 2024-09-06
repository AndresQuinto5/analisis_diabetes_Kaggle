# Proyecto de Predicción de Diabetes

## Descripción
Este proyecto utiliza técnicas de aprendizaje automático para predecir la probabilidad de diabetes en pacientes, basándose en diversos factores de salud. Se implementan y comparan varios modelos de clasificación, incluyendo Regresión Logística, Árboles de Decisión, Random Forest, SVM, XGBoost y Gradient Boosting.

## Dataset
El proyecto utiliza el conjunto de datos de Diabetes de los Indios Pima, que incluye las siguientes características:

- Pregnancies: Número de embarazos
- Glucose: Nivel de glucosa en sangre
- BloodPressure: Presión arterial
- SkinThickness: Grosor del pliegue cutáneo
- Insulin: Nivel de insulina
- BMI: Índice de Masa Corporal
- DiabetesPedigreeFunction: Función de pedigrí de diabetes
- Age: Edad
- Outcome: Variable objetivo (0 = No diabetes, 1 = Diabetes)

El dataset se encuentra en el archivo `diabetes.csv` en la raíz del proyecto.

## Entorno de Desarrollo
Este proyecto utiliza un entorno Conda. El archivo `environment.yml` se encuentra en la raíz del directorio y contiene todas las dependencias necesarias.

## Instalación y Configuración

1. Clona este repositorio:
   ```
   git clone https://github.com/tu_usuario/prediccion-diabetes.git
   cd prediccion-diabetes
   ```

2. Crea y activa el entorno Conda:
   ```
   conda env create -f environment.yml
   conda activate Kaggle
   ```

3. Verifica que Jupyter Notebook esté instalado en el entorno:
   ```
   jupyter notebook
   ```

## Cómo Ejecutar el Proyecto

1. Abre Jupyter Notebook desde la línea de comandos:
   ```
   jupyter notebook
   ```

2. Navega hasta el notebook `diabetes.ipynb` y ábrelo.

3. Ejecuta todas las celdas del notebook en orden.

## Estructura del Proyecto

- `diabetes.ipynb`: Notebook principal con todo el código del proyecto.
- `diabetes.csv`: Dataset utilizado para el análisis y modelado.
- `environment.yml`: Archivo de configuración del entorno Conda.
- `EDA.md`: Resultados del Análisis Exploratorio de Datos.
- `ML_results.md`: Resultados detallados de los modelos de Machine Learning.
- `README.md`: Este archivo.

## Resultados

Los resultados detallados del proyecto se pueden encontrar en los siguientes archivos:

- [Análisis Exploratorio de Datos (EDA)](EDA.md)
- [Resultados de Machine Learning](ML_results.md)

### Resumen de Resultados

El mejor modelo en términos de ROC AUC fue XGBoost, con un valor de 0.8389. Sin embargo, la Regresión Logística mostró un buen equilibrio entre rendimiento e interpretabilidad.

## Conclusiones Principales

1. La glucosa en sangre, el IMC y la edad son los predictores más importantes de diabetes.
2. Existe un trade-off entre precisión y recall en los modelos más complejos.
3. Se recomienda un enfoque de dos etapas: usar Regresión Logística como modelo principal y XGBoost para casos inciertos.
4. Es necesario recopilar más datos, especialmente de casos positivos de diabetes, para mejorar el rendimiento del modelo.

## Próximos Pasos

1. Validar los modelos con conjuntos de datos independientes.
2. Explorar la incorporación de variables adicionales como historial familiar y marcadores genéticos.
3. Implementar un sistema de monitoreo y actualización continua del modelo.

## Contribuciones

Las contribuciones son bienvenidas. Por favor, abre un issue para discutir cambios mayores antes de hacer un pull request.

## Licencia

Este proyecto está bajo la licencia MIT. Ver el archivo [LICENSE](LICENSE) para más detalles.

