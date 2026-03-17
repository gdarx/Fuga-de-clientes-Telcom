# Análisis Fuga de Clientes Telcom
## Contexto
La industria de telecomunicaciones enfrenta una tasa de rotación alta debido a la fuerte competencia y la baja diferenciación de productos. El costo de adquisición de un nuevo cliente es significativamente mayor que el de retención.
## Preparación y Proceso
### Fuente de datos
Se utilizó un dataset de 7,043 registros de clientes con 22 columnas. En el cual se encuentran variables como los tipos de servicios contratados, meses de permanencia, comuna, el monto de pago, etc.
### Herramientas
Python: para la exploración, transformación y limpieza inicial del conjunto del dataset.
Power BI: principalmente para el análisis mediante DAX y visualización de datos.
### ETL
Se encontraron 11 valores nulos en la columna "Cargo Total", y esto es debido a que los clientes poseen 0 meses de permanencia, lo que resulta en que el sistema los registra como valores nulo. Asi que para asegurar la integridad del análisis y no alterar los resultados, reemplacé los valores nulos por 0.
Por otro lado no se encontraron inconsistencias en los tipos de datos ni registros duplicados. Finalmente exporte el conjunto limpio de Python para seguir trabajando en Power BI.
## Análisis y Visualizaciones

## Recomendaciones
