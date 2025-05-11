# IA en Marketing - Análisis de Ventas con API

<a target="_blank" align="center">
  <img align="center" height="450" width="1000" alt="GIF" src="https://github.com/IVANMORAG/facial-point-detection/blob/main/recursos/Facial-Point-detector.gif">
</a>

<br>

## Descripción
Este proyecto utiliza técnicas de inteligencia artificial para analizar un dataset de ventas, aplicando clustering (K-Means) y reducción de dimensionalidad (PCA y Autoencoders) para segmentar clientes y predecir patrones de compra. Se ha desarrollado una API para exponer los resultados del análisis, permitiendo a los usuarios interactuar con los datos procesados, como la segmentación de clientes basada en ventas, cantidad ordenada, precio y más. El dataset utilizado proviene de un archivo CSV de ventas y se procesa para identificar clusters óptimos.

## Características
- **Análisis de Datos**: Limpieza y exploración de un dataset de ventas con Pandas y visualización con Plotly.
- **Clustering**: Implementación de K-Means para segmentar clientes en grupos basados en su comportamiento de compra.
- **Reducción de Dimensionalidad**: Uso de PCA y Autoencoders para visualizar y reducir la complejidad de los datos.
- **API**: Exposición de los resultados del análisis a través de una API (por ejemplo, con Flask).
- **Visualización**: Gráficos interactivos (barras, líneas, 3D scatter) para interpretar los clusters y tendencias.

## Tecnologías Utilizadas
- **Lenguajes**: Python
- **Librerías**:
  - Pandas, NumPy (manipulación de datos)
  - Matplotlib, Plotly, Seaborn (visualización)
  - TensorFlow/Keras (Autoencoders)
  - Scikit-learn (K-Means, PCA, StandardScaler)
- **Herramientas**: Google Colab (desarrollo inicial), Git (control de versiones)

## Requisitos
- Python 3.8+
- Dependencias listadas en `requirements.txt`
- Dataset `sales_data_sample.csv` en la ruta especificada o configurada
- Entorno de ejecución (puede requerir GPU para Autoencoders si se entrena)

## Instalación
1. Clona el repositorio:
   ```bash
   git clone https://github.com/tu-usuario/ai-marketing-api.git
   cd ai-marketing-api
   ```

2. Crea y activa un entorno virtual:
    ```bash
    python -m venv mi_entorno
    source mi_entorno/bin/activate  # En Windows: mi_entorno\Scripts\activate
   ```

3. Instala las dependencias:
    ```bash
    pip install -r requirements.txt
    ```

4. Coloca el dataset sales_data_sample.csv en la carpeta adecuada (por ejemplo, data/).

5. Configura ngrok con tu dominio personalizado en app.py (variable NGROK_DOMAIN).

## Uso

1. Inicia la API:
   ```bash
   python app.py
   ```

2. Accede a los endpoints de la API (por ejemplo, http://localhost:5000/clusters para obtener los clusters).


## Contribuciones

Las contribuciones son bienvenidas. Por favor, sigue estos pasos:
Haz un fork del repositorio.

1. Crea una rama para tu feature (git checkout -b feature/nueva-funcionalidad).

2. Realiza tus cambios y haz commit (git commit -m "Añadir nueva funcionalidad").

3. Envía un pull request.

## Licencia

Este proyecto está bajo la Licencia MIT. Consulta el archivo LICENSE para más detalles.

## Autor

* Iván Mora
Creado en 2025 como proyecto de reconocimiento facial.


### Notas Adicionales

- El archivo `requirements.txt` debe generarse con `pip freeze > requirements.txt` después de instalar las dependencias.

