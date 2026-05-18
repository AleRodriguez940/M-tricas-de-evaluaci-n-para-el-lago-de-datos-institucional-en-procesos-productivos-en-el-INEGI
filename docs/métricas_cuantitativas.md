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

---

# 11. Tasa de Crecimiento de Datos

## Fórmula

$$
C_{datos} = \frac{D_f - D_i}{D_i} \times 100
$$

## Componentes

| Componente | Descripción |
|---|---|
| $C_{datos}$ | Tasa de crecimiento de datos |
| $D_f$ | Volumen final de datos |
| $D_i$ | Volumen inicial de datos |

## Explicación de la fórmula

La fórmula calcula el porcentaje de crecimiento del volumen de información almacenada dentro del Lago de Datos Institucional.

Primero se resta el volumen inicial respecto al volumen final de datos. Posteriormente, el resultado se divide entre el volumen inicial y se multiplica por 100 para obtener un porcentaje.

Un valor elevado indica un crecimiento acelerado de información institucional.

## Explicación de la métrica

El INEGI genera continuamente grandes cantidades de información estadística y geoespacial provenientes de censos, encuestas y registros administrativos.

Esta métrica permite evaluar:
- crecimiento institucional de datos,
- necesidades futuras de almacenamiento,
- capacidad de escalabilidad,
- y planeación de infraestructura tecnológica.

También ayuda a prevenir:
- saturación de almacenamiento,
- problemas de rendimiento,
- y limitaciones operativas futuras.

---

# 12. Índice de Automatización de Procesos

## Fórmula

$$
A_{procesos} = \frac{P_a}{P_t} \times 100
$$

## Componentes

| Componente | Descripción |
|---|---|
| $A_{procesos}$ | Nivel de automatización |
| $P_a$ | Procesos automatizados |
| $P_t$ | Total de procesos |

## Explicación de la fórmula

La fórmula calcula el porcentaje de procesos institucionales que han sido automatizados mediante el uso del Lago de Datos.

El número de procesos automatizados se divide entre el total de procesos existentes y posteriormente se multiplica por 100.

Un porcentaje mayor representa un nivel más alto de automatización institucional.

## Explicación de la métrica

Actualmente muchos procesos relacionados con integración y análisis de información requieren actividades manuales.

Esta métrica permite medir qué tanto contribuye la plataforma a:
- reducir tareas repetitivas,
- optimizar operaciones,
- disminuir errores humanos,
- y mejorar tiempos de procesamiento.

Una mayor automatización favorece:
- eficiencia institucional,
- productividad,
- y aprovechamiento tecnológico.

---

# 13. Tiempo de Recuperación ante Fallos

## Fórmula

$$
TRF = T_{recuperacion} - T_{falla}
$$

## Componentes

| Componente | Descripción |
|---|---|
| $TRF$ | Tiempo de recuperación ante fallos |
| $T_{recuperacion}$ | Momento en que el sistema se recupera |
| $T_{falla}$ | Momento en que ocurre la falla |

## Explicación de la fórmula

La fórmula calcula el tiempo que tarda la plataforma en volver a operar correctamente después de una interrupción o falla.

El tiempo de recuperación se obtiene restando el momento en que ocurrió la falla respecto al momento en que el sistema vuelve a estar disponible.

Mientras menor sea el resultado, mayor será la capacidad de recuperación tecnológica.

## Explicación de la métrica

El Lago de Datos Institucional debe garantizar continuidad operativa para múltiples unidades administrativas.

Esta métrica ayuda a evaluar:
- resiliencia tecnológica,
- capacidad de respuesta,
- estabilidad operativa,
- y disponibilidad institucional.

Reducir el tiempo de recuperación permite:
- minimizar interrupciones,
- evitar retrasos operativos,
- y mantener acceso continuo a la información.

---

# 14. Índice de Uso de Recursos Computacionales

## Fórmula

$$
U_{recursos} = \frac{R_{utilizados}}{R_{totales}} \times 100
$$

## Componentes

| Componente | Descripción |
|---|---|
| $U_{recursos}$ | Nivel de uso de recursos |
| $R_{utilizados}$ | Recursos utilizados |
| $R_{totales}$ | Recursos disponibles |

## Explicación de la fórmula

La fórmula calcula el porcentaje de recursos computacionales utilizados respecto al total disponible.

Los recursos utilizados se dividen entre los recursos totales y posteriormente se multiplica por 100.

Un valor elevado indica un mayor consumo de infraestructura tecnológica.

## Explicación de la métrica

Esta métrica permite monitorear el uso de:
- CPU,
- memoria,
- almacenamiento,
- y capacidad de procesamiento.

Es importante porque ayuda a:
- optimizar infraestructura,
- prevenir saturaciones,
- mejorar rendimiento,
- y planear expansión tecnológica futura.

---

# 15. Tasa de Consultas Exitosas

## Fórmula

$$
Q_{exito} = \frac{Q_e}{Q_t} \times 100
$$

## Componentes

| Componente | Descripción |
|---|---|
| $Q_{exito}$ | Tasa de consultas exitosas |
| $Q_e$ | Consultas ejecutadas correctamente |
| $Q_t$ | Total de consultas realizadas |

## Explicación de la fórmula

La fórmula calcula el porcentaje de consultas ejecutadas exitosamente dentro de la plataforma.

Las consultas exitosas se dividen entre el total de consultas realizadas y posteriormente se multiplica por 100.

Un porcentaje alto representa mejor estabilidad y funcionamiento operativo.

## Explicación de la métrica

El Lago de Datos será utilizado constantemente para:
- búsquedas,
- análisis,
- consultas estadísticas,
- y acceso a información geoespacial.

Esta métrica permite identificar:
- fallas operativas,
- errores de consulta,
- problemas de integración,
- y limitaciones técnicas.

Una mayor tasa de éxito mejora:
- productividad,
- confianza institucional,
- y eficiencia analítica.

---

# 16. Índice de Integridad de Datos

## Fórmula

$$
I_{integridad} = \frac{D_{integros}}{D_{totales}} \times 100
$$

## Componentes

| Componente | Descripción |
|---|---|
| $I_{integridad}$ | Nivel de integridad |
| $D_{integros}$ | Datos completos y válidos |
| $D_{totales}$ | Total de datos evaluados |

## Explicación de la fórmula

La fórmula calcula el porcentaje de información que permanece completa, consistente y sin corrupción.

Los datos íntegros se dividen entre el total de datos evaluados y posteriormente se multiplica por 100.

Un valor alto representa mayor confiabilidad institucional.

## Explicación de la métrica

La integridad de datos es fundamental para garantizar resultados estadísticos precisos.

Esta métrica ayuda a detectar:
- registros incompletos,
- corrupción de información,
- inconsistencias,
- y errores de almacenamiento.

Mantener alta integridad fortalece:
- calidad analítica,
- confiabilidad institucional,
- y toma de decisiones basada en datos confiables.

---

# 17. Consumo Promedio de Almacenamiento

## Fórmula

$$
A_{promedio} = \frac{A_{total}}{n}
$$

## Componentes

| Componente | Descripción |
|---|---|
| $A_{promedio}$ | Consumo promedio de almacenamiento |
| $A_{total}$ | Almacenamiento total utilizado |
| $n$ | Número de procesos o datasets |

## Explicación de la fórmula

La fórmula calcula el promedio de almacenamiento utilizado por cada conjunto de datos o proceso institucional.

El almacenamiento total se divide entre el número total de elementos evaluados.

Mientras menor sea el consumo promedio, mayor será la optimización de recursos.

## Explicación de la métrica

Esta métrica ayuda a controlar el crecimiento de almacenamiento institucional.

También permite:
- optimizar recursos tecnológicos,
- identificar consumo excesivo,
- planear expansión de infraestructura,
- y reducir costos operativos.

---

# 18. Índice de Actualización de Datos

## Fórmula

$$
A_{datos} = \frac{D_{actualizados}}{D_{totales}} \times 100
$$

## Componentes

| Componente | Descripción |
|---|---|
| $A_{datos}$ | Nivel de actualización |
| $D_{actualizados}$ | Datos actualizados |
| $D_{totales}$ | Total de datos registrados |

## Explicación de la fórmula

La fórmula calcula el porcentaje de información que se encuentra actualizada dentro de la plataforma.

Los datos actualizados se dividen entre el total de registros existentes y posteriormente se multiplica por 100.

Un valor alto indica mayor vigencia de la información.

## Explicación de la métrica

El INEGI requiere información estadística y geoespacial constantemente actualizada.

Esta métrica ayuda a evaluar:
- vigencia de información,
- mantenimiento de datasets,
- actualización institucional,
- y confiabilidad operativa.

Mantener datos actualizados favorece:
- análisis precisos,
- decisiones oportunas,
- y calidad institucional.

---

# 19. Tasa de Errores en Procesamiento

## Fórmula

$$
E_{procesamiento} = \frac{Errores}{Procesos} \times 100
$$

## Componentes

| Componente | Descripción |
|---|---|
| $E_{procesamiento}$ | Tasa de errores |
| $Errores$ | Número de errores detectados |
| $Procesos$ | Total de procesos ejecutados |

## Explicación de la fórmula

La fórmula calcula el porcentaje de errores detectados durante la ejecución de procesos institucionales.

El número de errores se divide entre el total de procesos ejecutados y posteriormente se multiplica por 100.

Mientras menor sea el resultado, mayor será la estabilidad operativa.

## Explicación de la métrica

Esta métrica permite identificar problemas relacionados con:
- integración de información,
- automatización,
- procesamiento,
- y transformación de datos.

Reducir errores favorece:
- calidad institucional,
- estabilidad tecnológica,
- eficiencia operativa,
- y confiabilidad analítica.

---

# 20. Índice de Eficiencia Operacional

## Fórmula

$$
E_{operacional} = \frac{Resultados}{Recursos}
$$

## Componentes

| Componente | Descripción |
|---|---|
| $E_{operacional}$ | Nivel de eficiencia operacional |
| $Resultados$ | Productos o resultados obtenidos |
| $Recursos$ | Recursos utilizados |

## Explicación de la fórmula

La fórmula calcula qué tan eficientemente se utilizan los recursos disponibles para generar resultados institucionales.

Los resultados obtenidos se dividen entre los recursos utilizados.

Un valor mayor representa mejor aprovechamiento operativo.

## Explicación de la métrica

Esta métrica permite evaluar:
- productividad institucional,
- optimización tecnológica,
- eficiencia de procesos,
- y aprovechamiento de infraestructura.

También ayuda a identificar:
- desperdicio de recursos,
- procesos ineficientes,
- y oportunidades de mejora organizacional.




