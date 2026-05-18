# 📈 Métricas Cuantitativas

Las métricas cuantitativas permiten medir de manera numérica el desempeño, eficiencia y beneficios obtenidos mediante la implementación del Lago de Datos Institucional dentro del INEGI.

---

# 1. Tiempo Promedio de Acceso a Datos

## Fórmula

$$
T_{acceso} = \frac{\sum_{i=1}^{n} t_i}{n}
$$

## Componentes

| Componente | Descripción |
|---|---|
| $T_{acceso}$ | Tiempo promedio de acceso a los datos |
| $t_i$ | Tiempo individual de cada consulta |
| $n$ | Número total de consultas realizadas |

## Explicación de la fórmula

La fórmula calcula el promedio de tiempo que tarda el sistema en responder consultas de información. Para ello, se suman todos los tiempos individuales registrados en las consultas realizadas y posteriormente se divide entre el número total de consultas.

Mientras menor sea el resultado obtenido, mayor será la eficiencia de acceso a los datos.

## Explicación de la métrica

Esta métrica es importante porque el INEGI trabaja constantemente con grandes volúmenes de información estadística y geoespacial. Actualmente existen procesos centralizados y silos de información que provocan retrasos en el acceso a los datos.

Medir el tiempo promedio de acceso permite evaluar si el Lago de Datos Institucional realmente mejora la velocidad de consulta y disponibilidad de información para las unidades administrativas.

Una reducción en este tiempo ayuda a:

- acelerar procesos institucionales,
- mejorar la productividad,
- optimizar análisis estadísticos,
- y facilitar la toma de decisiones basada en información disponible en tiempo oportuno.

---

# 2. Índice de Reducción de Duplicidad de Datos

## Fórmula

$$
R_{duplicidad} = \frac{D_i - D_f}{D_i} \times 100
$$

## Componentes

| Componente | Descripción |
|---|---|
| $R_{duplicidad}$ | Porcentaje de reducción de duplicidad |
| $D_i$ | Cantidad inicial de datos duplicados |
| $D_f$ | Cantidad final de datos duplicados |

## Explicación de la fórmula

La fórmula calcula el porcentaje de reducción de datos duplicados dentro de la plataforma.

Primero se resta la cantidad final de datos duplicados respecto a la cantidad inicial. Posteriormente, el resultado se divide entre la cantidad inicial y se multiplica por 100 para obtener un porcentaje.

Un valor alto indica una mayor eliminación de información redundante.

## Explicación de la métrica

Actualmente, uno de los problemas identificados en el contexto del INEGI es la existencia de múltiples repositorios independientes que contienen versiones repetidas de la misma información.

La duplicidad genera:

- inconsistencias,
- mayor consumo de almacenamiento,
- dificultad para compartir información,
- y problemas en la calidad de datos.

Esta métrica permite evaluar qué tanto mejora la organización y centralización de la información dentro del Lago de Datos Institucional.

---

# 3. Disponibilidad de la Plataforma

## Fórmula

$$
Disponibilidad = \frac{T_{activo}}{T_{total}} \times 100
$$

## Componentes

| Componente | Descripción |
|---|---|
| $T_{activo}$ | Tiempo en que la plataforma estuvo funcionando |
| $T_{total}$ | Tiempo total evaluado |

## Explicación de la fórmula

La fórmula calcula el porcentaje de tiempo en el que la plataforma permanece operativa.

Para ello, el tiempo activo de funcionamiento se divide entre el tiempo total evaluado y posteriormente se multiplica por 100.

Entre mayor sea el porcentaje obtenido, mayor será la estabilidad de la plataforma.

## Explicación de la métrica

Esta métrica es importante debido a que el Lago de Datos Institucional busca convertirse en una plataforma transversal utilizada por múltiples unidades administrativas.

Si la plataforma presenta interrupciones frecuentes:

- se retrasan procesos,
- disminuye la productividad,
- y aumenta la dependencia entre áreas.

Una alta disponibilidad garantiza continuidad operativa, acceso constante a la información y mayor confianza institucional.

---

# 4. Tiempo de Procesamiento ETL

## Fórmula

$$
T_{ETL} = T_{fin} - T_{inicio}
$$

## Componentes

| Componente | Descripción |
|---|---|
| $T_{ETL}$ | Tiempo total del proceso ETL |
| $T_{fin}$ | Hora de finalización del proceso |
| $T_{inicio}$ | Hora de inicio del proceso |

## Explicación de la fórmula

La fórmula calcula el tiempo total requerido para ejecutar un proceso ETL.

Se obtiene restando el tiempo de inicio respecto al tiempo final del procesamiento.

Un menor tiempo ETL indica mayor eficiencia en los procesos de integración de datos.

## Explicación de la métrica

Los procesos ETL permiten extraer, transformar y cargar información proveniente de distintas fuentes.

En el contexto del INEGI, esta métrica es importante porque la institución trabaja con grandes cantidades de información estadística y geoespacial provenientes de múltiples sistemas.

Optimizar el tiempo ETL permite:

- acelerar la integración de información,
- mejorar tiempos de análisis,
- reducir retrasos operativos,
- y optimizar la generación de productos estadísticos.

---

# 5. Índice de Interoperabilidad de Datos

## Fórmula

$$
I_{interop} = \frac{D_{integrados}}{D_{totales}} \times 100
$$

## Componentes

| Componente | Descripción |
|---|---|
| $I_{interop}$ | Nivel de interoperabilidad |
| $D_{integrados}$ | Número de datasets integrados |
| $D_{totales}$ | Total de datasets existentes |

## Explicación de la fórmula

La fórmula calcula el porcentaje de conjuntos de datos que pueden interoperar correctamente dentro de la plataforma.

El número de datasets integrados se divide entre el total de datasets existentes y posteriormente se multiplica por 100.

Un porcentaje mayor representa mejor integración institucional.

## Explicación de la métrica

Uno de los principales problemas identificados en el contexto institucional es la existencia de silos de información.

Esta métrica permite evaluar qué tan bien pueden compartir información las distintas áreas del Instituto.

Una mayor interoperabilidad ayuda a:

- facilitar el trabajo colaborativo,
- reutilizar información,
- integrar análisis estadísticos y geoespaciales,
- y mejorar la comunicación entre unidades administrativas.

---

# 6. Velocidad de Transferencia de Datos

## Fórmula

$$
V_{transferencia} = \frac{Datos\ transferidos}{Tiempo}
$$

## Componentes

| Componente | Descripción |
|---|---|
| $V_{transferencia}$ | Velocidad de transferencia |
| $Datos\ transferidos$ | Cantidad de información enviada |
| $Tiempo$ | Tiempo requerido para la transferencia |

## Explicación de la fórmula

La fórmula calcula la velocidad promedio con la que la información es transferida entre sistemas.

La cantidad de datos enviados se divide entre el tiempo utilizado para la transferencia.

Entre mayor sea el resultado, mayor será la capacidad de transmisión de información.

## Explicación de la métrica

El Lago de Datos Institucional manejará grandes volúmenes de información estadística y geoespacial.

Por ello, medir la velocidad de transferencia es importante para garantizar:

- comunicación eficiente entre sistemas,
- procesamiento oportuno,
- intercambio rápido de información,
- y reducción de tiempos de espera.

---

# 7. Volumen de Datos Procesados

## Fórmula

$$
V_{datos} = \sum_{i=1}^{n} d_i
$$

## Componentes

| Componente | Descripción |
|---|---|
| $V_{datos}$ | Volumen total de datos procesados |
| $d_i$ | Cantidad de datos procesados por operación |

## Explicación de la fórmula

La fórmula calcula el volumen total de información procesada por la plataforma.

Para ello, se suman todos los conjuntos de datos procesados durante un periodo determinado.

Un mayor volumen indica mayor capacidad de procesamiento institucional.

## Explicación de la métrica

El INEGI trabaja constantemente con información masiva proveniente de censos, encuestas y datos geoespaciales.

Esta métrica permite evaluar si la infraestructura tecnológica puede soportar el crecimiento y demanda institucional.

También ayuda a identificar necesidades futuras relacionadas con almacenamiento y procesamiento.

---

# 8. Índice de Calidad de Datos

## Fórmula

$$
C_{datos} = \frac{Datos\ correctos}{Datos\ totales} \times 100
$$

## Componentes

| Componente | Descripción |
|---|---|
| $C_{datos}$ | Nivel de calidad de datos |
| $Datos\ correctos$ | Datos válidos y consistentes |
| $Datos\ totales$ | Total de datos evaluados |

## Explicación de la fórmula

La fórmula calcula el porcentaje de datos que cumplen criterios de calidad.

Los datos correctos se dividen entre el total de registros evaluados y posteriormente se multiplica por 100.

Un valor alto representa mayor precisión y confiabilidad.

## Explicación de la métrica

La calidad de datos es fundamental para garantizar resultados estadísticos confiables.

Esta métrica ayuda a identificar:

- inconsistencias,
- errores,
- datos incompletos,
- y problemas de integridad.

Mejorar la calidad de datos fortalece la confianza institucional y mejora la toma de decisiones.

---

# 9. Tasa de Incidentes de Seguridad

## Fórmula

$$
I_{seguridad} = \frac{Incidentes}{Periodo}
$$

## Componentes

| Componente | Descripción |
|---|---|
| $I_{seguridad}$ | Tasa de incidentes de seguridad |
| $Incidentes$ | Número de incidentes detectados |
| $Periodo$ | Tiempo evaluado |

## Explicación de la fórmula

La fórmula calcula el promedio de incidentes de seguridad detectados durante un periodo específico.

Mientras menor sea el valor obtenido, mayor será el nivel de seguridad institucional.

## Explicación de la métrica

El INEGI administra información sensible y estratégica.

Por ello, es importante monitorear continuamente:

- accesos no autorizados,
- vulnerabilidades,
- intentos de ataque,
- y fallas de seguridad.

Esta métrica ayuda a fortalecer la gobernanza y protección de los datos institucionales.

---

# 10. Retorno de Inversión (ROI)

## Fórmula

$$
ROI = \frac{Beneficios - Costos}{Costos} \times 100
$$

## Componentes

| Componente | Descripción |
|---|---|
| $ROI$ | Retorno de inversión |
| $Beneficios$ | Beneficios obtenidos |
| $Costos$ | Inversión realizada |

## Explicación de la fórmula

La fórmula calcula el porcentaje de ganancia o beneficio obtenido respecto a la inversión realizada.

Primero se restan los costos a los beneficios obtenidos. Posteriormente, el resultado se divide entre los costos y se multiplica por 100.

Un ROI positivo indica que la inversión genera beneficios institucionales.

## Explicación de la métrica

Esta es una de las métricas más importantes del proyecto.

Permite determinar si la implementación del Lago de Datos Institucional realmente genera valor para el INEGI.

Los beneficios pueden reflejarse en:

- reducción de costos,
- ahorro de tiempo,
- automatización de procesos,
- mejora operativa,
- y optimización del análisis de información.




