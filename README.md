# Análisis de Segmento de Cliente para La Tienda "El Mercado"
<p>
Este proyecto consiste en un análisis detallado del segmento de clientes de la tienda "El Mercado" utilizando técnicas de análisis RFM (Recency, Frequency, Monetary) y análisis de cohortes. El análisis se realizó utilizando Looker Studio para la visualización y Google Sheets para los cálculos y manipulación de datos.
</p>

## Metodología
### Preparación de Datos
1.**Importación de Datos**: Se utilizaron tablas importadas en Google Sheets a través de la función IMPORTANGE.

2.**Limpieza de Datos:**
Eliminación de datos nulos, que representaban menos del 1% del total y no eran relevantes para el análisis RFM.

- Remoción de valores duplicados con la fórmula UNIQUE.

- Exclusión de transacciones sin ID de cliente (aproximadamente 200 registros, el 1% del total) para garantizar la coherencia en el análisis posterior.

- No se consideraron IDs con valor 0 o clientes con año de nacimiento anterior a 1923 para mantener la integridad de los datos.

3.**Integración de Datos**:
Unión de tablas utilizando funciones como INDICE + COINCIDIR y BUSCARV.

**Creación de Nuevas Variables:**
- Variables derivadas como edad, mes de última compra, año de última compra, etc.

- Desarrollo de tablas dinámicas para categorizar variables como grupo de edad, estado civil, nivel de educación, etc. Cada variable fue además representada gráficamente.

## Análisis RFM
- **Cálculo de Cuartiles**: Uso de la fórmula CUARTILE para identificar segmentos de clientes.

**Segmentación de Clientes:**
- Clasificación en 4 categorías basadas en la matriz RFM.

- Cálculo del puntaje total RFM y asignación de un segmento de cliente específico.
<img width="412" alt="Captura de pantalla 2023-10-23 161140" src="https://github.com/Yesi0/Analisis-de-Datos-segmentacions-clientes/assets/125078076/23e8c994-e2ff-4e0d-abef-c04f6160ca9f">

## Análisis de Cohortes
- **Preparación de la Tabla de Cohortes:**
- Uso de QUERY y BUSCARV para segmentar clientes por mes de registro.

- Creación de variables de tiempo con la fórmula TEXT para aislar año y mes.

- **Análisis Estadístico:**
Cálculo de medidas de tendencia central (moda, promedio y mediana) para los períodos de tiempo analizados.

- **Retención de Clientes:**
Análisis del porcentaje de retención por cohorte visualizado mediante una tabla dinámica con mapa de calor.

<img width="409" alt="Captura de pantalla 2023-10-23 162146" src="https://github.com/Yesi0/Analisis-de-Datos-segmentacions-clientes/assets/125078076/56198da6-1703-461f-8442-44d4083fdbcd">

## Visualizaciones
Las visualizaciones se crearon en Looker Studio para representar los datos de manera comprensible y ofrecer insights valiosos sobre el segmento de clientes de "El Mercado".
Para ver el informe completo en Looker Studio, link [AQUI ](https://lookerstudio.google.com/s/ucHIaMikHsQ)
Calculos en google Sheets [AQUI ](https://docs.google.com/spreadsheets/d/1n5zhB27EtlrdLryIRFz9riCwSNQVysyb0U7EgieKT7o/edit?usp=sharing)

## Análisis de Clientes y Respuesta a Estrategias de Marketing

### Análisis RFM y Segmentación de Clientes

- **Segmentación de Clientes**: Identificación de cuatro segmentos clave: Clientes Estrella, Clientes Frecuentes, Clientes Potenciales y Clientes Inactivos.

- **Distribución de Clientes e Ingresos:** Los Clientes Estrella y Frecuentes generan la mayor parte de los ingresos, a pesar de ser menos en número.

- **Análisis de Recencia y Frecuencia:** Los Clientes Estrella muestran una alta frecuencia y baja recencia, indicando lealtad hacia "El Mercado".


### Resultados Generales y Respuesta a Campañas de Marketing

- **Compras en Línea vs. en Tienda:** Predominio de las compras en tienda sobre las en línea.

- **Transacciones y Registros de Clientes**: Tendencia decreciente en nuevas transacciones y registros de clientes.

- **Respuesta a Campañas de Marketing:** Falta de correlación entre el tamaño del segmento de clientes y las respuestas a las campañas.

### Análisis de Productos

- **Tendencias de Ventas en el Tiempo:** El 2022 muestra un aumento significativo en las ventas en comparación con años anteriores.

- **Ventas por Producto:** Dominio de los vinos en las ventas e ingresos totales, con otras categorías quedando atrás.

###  Análisis de Cohortes y Retención de Clientes

- **Tendencias de Retención de Clientes:** Alta retención en el primer mes de registro, seguida de una disminución significativa a lo largo del tiempo en todas las cohortes.

## Recomendaciones Generales

- Optimizar la experiencia de compra tanto en tienda como en línea.
Innovar y diversificar la oferta de productos, especialmente dado el éxito de los vinos.

- Implementar un sistema para recoger y actuar basados en el feedback de los clientes.

## Conclusiones Generales

- Necesidad de reactivar clientes inactivos y convertir clientes potenciales.
Importancia de abordar la disminución en la retención de clientes después del primer mes de registro.

- Priorizar la adaptación basada en el feedback del cliente para un crecimiento sostenido.

- Este análisis y las estrategias resultantes son fundamentales para entender el comportamiento del cliente y adaptar las prácticas comerciales de "El Mercado" de manera efectiva.

