# Proyecto Integrador 2024

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
- **Acciones**: datos históricos de precios de cierre de acciones obtenidos de [Yahoo Finance](https://finance.yahoo.com)
- **TRM**: tasa representativa del mercado obtenida del [Banco de la República de Colombia](https://www.banrep.gov.co/es/estadisticas/trm)
- **IPC, PIB**: índice de precios al consumidor (IPC) y producto interno bruto (PIB) obtenidos del [DANE (Departamento Administrativo Nacional de Estadística)](https://www.dane.gov.co)

## Principales Conclusiones
1. **Meta de MAE alcanzada**: Se cumplió con la meta de MAE menor a 50 en 10 de 13 acciones, demostrando alta precisión.

2. **Random Forest mejor modelo**: Random Forest superó a LSTM, XGBoost, SARIMAX y ARIMA en precisión, siendo la mejor opción para el mercado colombiano.

3. **Facilidades con Hugging Face**: Subir el modelo a Hugging Face facilita su uso y reduce el tiempo de ejecución, simplificando la implementación.

## Resultados del Modelo Random Forest
- **PFGRUPSURA.CL**: MAE: 253.13, RMSE: 486.71
- **PFBCOLOM.CL**: MAE: 14.44, RMSE: 21.59
- **ISA.CL**: MAE: 31.71, RMSE: 53.53
- **GRUPOARGOS.CL**: MAE: 27.06, RMSE: 55.79
- **CEMARGOS.CL**: MAE: 13.89, RMSE: 28.64
- **CIB**: MAE: 0.02, RMSE: 0.03
- **EC**: MAE: 0.01, RMSE: 0.01
- **ICOLCAP.CL**: MAE: 9.01, RMSE: 14.28
- **PFDAVVNDA.CL**: MAE: 3852.80, RMSE: 4761.81
- **CELSIA.CL**: MAE: 69.55, RMSE: 123.16
- **TERPEL.CL**: MAE: 6.10, RMSE: 9.97
- **GRUPOSURA.CL**: MAE: 45.34, RMSE: 86.35
- **GEB.CL**: MAE: 36.53, RMSE: 84.55
