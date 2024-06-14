# Proyecto_Integrador

Repositorio de GitHub: [https://github.com/cristlop/Proyecto_Integrador](https://github.com/cristlop/Proyecto_Integrador)

## Descripción
Este repositorio contiene todas las fuentes, datos y el código necesario para reproducir el proyecto de predicción de precios de cierre de acciones en el mercado colombiano utilizando modelos de aprendizaje automático, específicamente XGBoost, Random Forest, LSTM, SARIMAX y ARIMA.

## Contenido del repositorio
- **Notebook principal**: `proyecto_Integrador_2024.ipynb` con todo el flujo del proyecto, desde la carga de datos hasta la evaluación del modelo.
- **Datos**: conjunto de datos utilizados para entrenar y evaluar los modelos.
- **Instrucciones**: pasos detallados para reproducir el proyecto, incluyendo la instalación de dependencias y la configuración del entorno de trabajo.

## Instrucciones para reproducir el proyecto
1. Clonar el repositorio:
    ```bash
    git clone https://github.com/cristlop/Proyecto_Integrador
    ```

2. Navegar al directorio del proyecto:
    ```bash
    cd Proyecto_Integrador
    ```

3. Instalar las dependencias necesarias:
    ```bash
    pip install -r requirements.txt
    ```

4. Ejecutar el notebook principal para reproducir el análisis y entrenamiento del modelo:
    ```bash
    jupyter notebook Proyecto_Integrador_2024.ipynb
    ```

5. Seguir las instrucciones dentro del notebook para entrenar los modelos y generar predicciones.

## Fuentes de Datos
- **Acciones**: Datos históricos de precios de cierre de acciones obtenidos de [Yahoo Finance](https://finance.yahoo.com)
- **TRM**: Tasa Representativa del Mercado (TRM) obtenida del [Banco de la República de Colombia](https://www.banrep.gov.co/es/estadisticas/trm)
- **IPC, PIB**: Índice de Precios al Consumidor (IPC) y Producto Interno Bruto (PIB) obtenidos del [DANE (Departamento Administrativo Nacional de Estadística)](https://www.dane.gov.co)

## Principales Conclusiones
1. **Incapacidad para alcanzar MAE esperado**: a pesar de que el modelo XGBoost obtuvo buenos resultados, no fue posible alcanzar el MAE esperado inferior a 100 COP por cada acción. Solo se logró con 2 de 15.

2. **Modelos alternativos**: entre los diferentes modelos evaluados, XGBoost demostró ser el más efectivo en términos de precisión. Comparado con LSTM, Random Forest, SARIMAX, y ARIMA, fue la mejor opción para la predicción de precios de cierre de acciones en el mercado colombiano.

3. **Desafíos de la volatilidad del mercado**: la alta volatilidad del mercado colombiano se mantiene como un reto importante para alcanzar una mayor precisión en las predicciones.

4. **Beneficios de Hugging Face**: subir el pipeline y el modelo XGBoost a Hugging Face facilita el acceso y uso del modelo preentrenado, reduciendo significativamente el tiempo de ejecución y simplificando el proceso de implementación.
