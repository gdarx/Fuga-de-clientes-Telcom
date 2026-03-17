# Análisis Fuga de Clientes Telcom
## Contexto
La industria de telecomunicaciones enfrenta una tasa de rotación alta debido a la fuerte competencia y la baja diferenciación de productos. El costo de adquisición de un nuevo cliente es significativamente mayor que el de retención.
En el dinámico mercado de las telecomunicaciones en Chile, la retención de clientes es un factor crítico para la rentabilidad a largo plazo. Este proyecto analiza el comportamiento de los clientes de una empresa de telecomunicaciones, con datos adaptados al contexto local de la Región del Biobío (Gran Concepción).
Como Ingeniero Comercial, el enfoque de este análisis no es solo descriptivo, sino prescriptivo: identificar los focos de pérdida de ingresos y proponer estrategias comerciales basadas en evidencia.

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
### Fuga crítica en fibra óptica
<img width="345" height="128" alt="image" src="https://github.com/user-attachments/assets/0fcb0913-66de-4fba-90e4-02e15af1ccb5" />

### Valor de los servicios de seguridad

### Fricción en métodos de pago manuales
<img width="772" height="463" alt="image" src="https://github.com/user-attachments/assets/706c3c2d-557c-4e53-854c-09616b7adc9f" />

### Ánalisis de fuga geográfico
#### Concepción
<img width="1110" height="588" alt="image" src="https://github.com/user-attachments/assets/0b05a3ee-205e-4235-a011-ca8866dbed55" />

#### San Pedro de la Paz
<img width="1112" height="591" alt="image" src="https://github.com/user-attachments/assets/40e2e9ae-d3b0-4a01-ad7c-e361e88d7914" />

## Recomendaciones
