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
A pesar de ser un servicio de más calidad, los clientes de Fibra Óptica se van el doble que los de ADSL (41.9% vs 19%). Esto sugiere problemas de calidad de servicio o precios no competitivos en este segmento.
### Valor de los servicios de seguridad
<img width="473" height="277" alt="image" src="https://github.com/user-attachments/assets/578939cd-52a6-407b-9704-3a19f201587a" />
Los servicios adicionales reducen drásticamente la fuga, por ejemplo: Probabiliad de fuga de clientes con servicio técnico (15,17%) y sin (41,6%).
### Fricción en métodos de pago manuales
<img width="772" height="463" alt="image" src="https://github.com/user-attachments/assets/706c3c2d-557c-4e53-854c-09616b7adc9f" />
El método Transferencia/Webpay muestra una tasa de fuga alarmante del 45.3%. Esto sugiere que los clientes que deben realizar un pago manual mes a mes tienen más oportunidades de reconsiderar su permanencia o simplemente olvidar el pago y ser cortados.
### Ánalisis de fuga geográfico
Existe una disparidad geográfica en la fidelidad de los clientes. Concepción (32.0%) y San Pedro de la Paz (31.7%) presentan las tasas de fuga más altas, superando el promedio general de la empresa (26.5%).
#### Concepción
<img width="889" height="500" alt="image" src="https://github.com/user-attachments/assets/8c258101-0138-4946-898c-a5ba8174bcb7" />
#### San Pedro de la Paz
<img width="888" height="494" alt="image" src="https://github.com/user-attachments/assets/0180b5c9-a8d1-41cb-9fa1-0df0e3cb68b1" />

## Recomendaciones
Los clientes que se van pagan un promedio de $37,220, lo cual es un 21.5% más que los que se quedan ($30,632). Se recomienda ajustar los planes de fibra para que el salto de precio desde el ADSL no sea tan drástico.

Incluir servicios como Seguridad Online y Servicio Técnico como beneficio estandár en los planes de Fibra Óptica. Además, al momento de una llamada por soporte o consulta, ofrecer estos servicios de manera gratuita por unos meses para aumentar el "stickness" del cliente y dificultar su salida hacia la competencia.

Implementar una campaña de incentivos, ya sea como un pequeño descuento mensual o meses de streaming gratuito, para los clientes que migren su pago manual a la modalidad de  pago automático (PAC/PAT). Esto "automatiza" la lealtad y reduce la fricción del cobro mensual.

Realizar una auditoría técnica y de servicio al cliente específica en Concepción y San Pedro de la Paz para identificar si la fuga se debe a problemas de cobertura, interrupciones del servicio o una oferta más agresiva de la competencia local.
