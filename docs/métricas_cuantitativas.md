# 📈 Métricas Cuantitativas 

Las métricas cuantitativas permiten medir de manera numérica el desempeño, eficiencia y beneficios obtenidos mediante la implementación del Lago de Datos Institucional dentro del INEGI.

Cada métrica se presenta en el siguiente orden: explicación de la métrica, fórmula con tabla de componentes y explicación de la fórmula.

---

## 1. Tiempo promedio de acceso a datos

### Explicación de la métrica

Se trabaja constantemente con grandes volúmenes de información estadística y geoespacial. Medir el tiempo promedio de acceso permite evaluar si el Lago de Datos mejora la velocidad de consulta y disponibilidad de información para las unidades administrativas. Una reducción en este tiempo acelera procesos institucionales, mejora la productividad y facilita la toma de decisiones oportuna.

### Fórmula

$$
T_{acceso} = \frac{\sum_{i=1}^{n} t_i}{n}
$$

### Componentes

| Componente | Descripción |
|:----------:|-------------|
| $T_{acceso}$ | Tiempo promedio de acceso a los datos |
| $t_i$ | Tiempo individual de cada consulta $i$ |
| $n$ | Número total de consultas realizadas |

### Explicación de la fórmula

Se suman todos los tiempos individuales registrados en las consultas realizadas y se divide entre el número total de consultas. Mientras menor sea el resultado, mayor es la eficiencia de acceso.

---

## 2. Índice de reducción de duplicidad de datos

### Explicación de la métrica

Uno de los problemas identificados es la existencia de múltiples repositorios independientes con versiones repetidas de la misma información. La duplicidad genera inconsistencias, mayor consumo de almacenamiento y problemas de calidad. Esta métrica evalúa qué tanto mejora la organización y centralización de información dentro del Lago de Datos.

### Fórmula

$$
R_{dup} = \frac{D_i - D_f}{D_i} \times 100
$$

### Componentes

| Componente | Descripción |
|:----------:|-------------|
| $R_{dup}$ | Porcentaje de reducción de duplicidad |
| $D_i$ | Cantidad inicial de registros duplicados |
| $D_f$ | Cantidad final de registros duplicados |

### Explicación de la fórmula

Se resta la cantidad final de datos duplicados respecto a la cantidad inicial, se divide entre la cantidad inicial y se multiplica por 100. Un valor alto indica mayor eliminación de información redundante.

---

## 3. Disponibilidad de la plataforma

### Explicación de la métrica

El Lago de Datos busca convertirse en una plataforma transversal utilizada por múltiples unidades administrativas. Las interrupciones frecuentes retrasan procesos, disminuyen la productividad y aumentan la dependencia entre áreas. Una alta disponibilidad garantiza continuidad operativa y acceso constante a la información institucional.

### Fórmula

$$
D_{plat} = \frac{T_{activo}}{T_{total}} \times 100
$$

### Componentes

| Componente | Descripción |
|:----------:|-------------|
| $D_{plat}$ | Porcentaje de disponibilidad |
| $T_{activo}$ | Tiempo en que la plataforma estuvo operativa |
| $T_{total}$ | Tiempo total del período evaluado |

### Explicación de la fórmula

El tiempo activo de funcionamiento se divide entre el tiempo total evaluado y se multiplica por 100. Un valor cercano al 100% indica alta estabilidad operativa. El umbral mínimo aceptable es de 99.5%.

---

## 4. Tiempo de procesamiento ETL

### Explicación de la métrica

Los procesos ETL permiten extraer, transformar y cargar información proveniente de distintas fuentes. Se trabaja con grandes cantidades de información estadística y geoespacial proveniente de múltiples sistemas. Optimizar el tiempo ETL acelera la integración de información, mejora los tiempos de análisis y optimiza la generación de productos estadísticos.

### Fórmula

$$
T_{ETL} = T_{fin} - T_{inicio}
$$

### Componentes

| Componente | Descripción |
|:----------:|-------------|
| $T_{ETL}$ | Tiempo total del proceso ETL |
| $T_{fin}$ | Momento de finalización del proceso |
| $T_{inicio}$ | Momento de inicio del proceso |

### Explicación de la fórmula

Se obtiene restando el momento de inicio respecto al momento de finalización del procesamiento. Un menor tiempo ETL indica mayor eficiencia en los procesos de integración de datos.

---

## 5. Índice de interoperabilidad de datos

### Explicación de la métrica

Otro de los principales problemas es la existencia de silos de información. Esta métrica evalúa qué tan bien pueden compartir información las distintas áreas del Instituto, facilitando el trabajo colaborativo, la reutilización de datos y la integración de análisis estadísticos y geoespaciales.

### Fórmula

$$
I_{interop} = \frac{D_{integrados}}{D_{totales}} \times 100
$$

### Componentes

| Componente | Descripción |
|:----------:|-------------|
| $I_{interop}$ | Nivel de interoperabilidad |
| $D_{integrados}$ | Número de datasets integrados correctamente |
| $D_{totales}$ | Total de datasets existentes en el lago |

### Explicación de la fórmula

El número de datasets integrados se divide entre el total de datasets existentes y se multiplica por 100. Un porcentaje mayor representa mejor integración institucional y menor existencia de silos de información.

---

## 6. Índice de calidad de datos

### Explicación de la métrica

La calidad de datos es fundamental para garantizar resultados estadísticos confiables. Esta métrica ayuda a identificar inconsistencias, errores, datos incompletos y problemas de validez en los registros individuales. Mejorar la calidad fortalece la confianza institucional y la toma de decisiones basada en información fiable.

### Fórmula

$$
ICD = \frac{D_{correctos}}{D_{totales}} \times 100
$$

### Componentes

| Componente | Descripción |
|:----------:|-------------|
| $ICD$ | Índice de calidad de datos |
| $D_{correctos}$ | Registros válidos, consistentes y sin errores |
| $D_{totales}$ | Total de registros evaluados |

### Explicación de la fórmula

Los datos correctos se dividen entre el total de registros evaluados y se multiplica por 100. Un valor alto representa mayor precisión y confiabilidad de la información. Se recomienda un umbral mínimo de 95% para los datasets.

---

## 7. Índice de integridad referencial de datos

### Explicación de la métrica

En un lago de datos que integra fuentes heterogéneas como censos, encuestas y cartografía, es crítico que las relaciones entre entidades se mantengan sin corrupción. Un registro de vivienda debe poder vincularse correctamente con su AGEB, municipio y entidad federativa. Esta métrica detecta rupturas en esas cadenas de referencia que afectarían la confiabilidad de los análisis integrados. A diferencia del índice de calidad, que evalúa la validez de registros individuales, esta métrica se enfoca en la consistencia de los vínculos entre datasets.

### Fórmula

$$
I_{integ} = \frac{R_{validas}}{R_{totales}} \times 100
$$

### Componentes

| Componente | Descripción |
|:----------:|-------------|
| $I_{integ}$ | Índice de integridad referencial |
| $R_{validas}$ | Relaciones entre tablas o datasets sin inconsistencias |
| $R_{totales}$ | Total de relaciones evaluadas |

### Explicación de la fórmula

Las relaciones válidas entre entidades del lago se dividen entre el total de relaciones evaluadas y se multiplica por 100. Un valor cercano al 100% indica que las cadenas de referencia entre datasets se mantienen íntegras y sin rupturas.

---

## 8. Tasa de incidentes de seguridad

### Explicación de la métrica

Se administra información sensible y estratégica de carácter estadístico y geoespacial. Es importante monitorear continuamente accesos no autorizados, vulnerabilidades, intentos de ataque y fallas de seguridad. Esta métrica fortalece la gobernanza y protección de los datos institucionales, y permite identificar tendencias de riesgo a lo largo del tiempo.

### Fórmula

$$
I_{seg} = \frac{N_{incidentes}}{T_{periodo}}
$$

### Componentes

| Componente | Descripción |
|:----------:|-------------|
| $I_{seg}$ | Tasa de incidentes de seguridad por unidad de tiempo |
| $N_{incidentes}$ | Número de incidentes detectados en el período |
| $T_{periodo}$ | Duración del período evaluado (días, semanas o meses) |

### Explicación de la fórmula

El número de incidentes detectados se divide entre la duración del período evaluado. El resultado expresa la frecuencia de incidentes por unidad de tiempo. Mientras menor sea el valor, mayor es el nivel de seguridad institucional.

---

## 9. Retorno de inversión (ROI)

### Explicación de la métrica

Esta es una de las métricas más importantes. Permite determinar si la implementación del Lago de Datos realmente genera valor para el INEGI, considerando reducción de costos operativos, ahorro de tiempo, automatización de procesos y optimización del análisis de información. Un ROI positivo justifica la continuidad y expansión de la inversión institucional.

### Fórmula

$$
ROI = \frac{B_{total} - C_{total}}{C_{total}} \times 100
$$

### Componentes

| Componente | Descripción |
|:----------:|-------------|
| $ROI$ | Retorno de inversión expresado en porcentaje |
| $B_{total}$ | Beneficios totales obtenidos (monetarios y operativos cuantificados) |
| $C_{total}$ | Costos totales de implementación y operación |

### Explicación de la fórmula

Se restan los costos totales a los beneficios obtenidos, el resultado se divide entre los costos totales y se multiplica por 100. Un ROI positivo indica que la inversión genera valor institucional neto. Los beneficios incluyen reducción de costos operativos, ahorro en tiempo de procesos y disminución de errores cuantificados económicamente.

---

## 10. Tasa de crecimiento del volumen de datos

### Explicación de la métrica

Se generan continuamente grandes cantidades de información estadística y geoespacial con cada ciclo censal, encuesta o actualización cartográfica. Esta métrica permite evaluar el crecimiento institucional de datos, las necesidades futuras de almacenamiento y la capacidad de escalabilidad. También ayuda a prevenir saturación de infraestructura y limitaciones operativas futuras.

### Fórmula

$$
TC_{datos} = \frac{V_f - V_i}{V_i} \times 100
$$

### Componentes

| Componente | Descripción |
|:----------:|-------------|
| $TC_{datos}$ | Tasa de crecimiento del volumen de datos |
| $V_f$ | Volumen final de datos almacenados |
| $V_i$ | Volumen inicial de datos almacenados |

### Explicación de la fórmula

Se resta el volumen inicial al volumen final, el resultado se divide entre el volumen inicial y se multiplica por 100. Un valor elevado indica crecimiento acelerado de información institucional que debe anticiparse en la planeación de infraestructura.

---

## 11. Índice de automatización de procesos

### Explicación de la métrica

Actualmente muchos procesos relacionados con integración y análisis de información requieren actividades manuales. Esta métrica mide qué tanto contribuye la plataforma a reducir tareas repetitivas, minimizar errores humanos y mejorar tiempos de procesamiento. Una mayor automatización favorece la eficiencia y el aprovechamiento tecnológico institucional.

### Fórmula

$$
A_{proc} = \frac{P_{automatizados}}{P_{totales}} \times 100
$$

### Componentes

| Componente | Descripción |
|:----------:|-------------|
| $A_{proc}$ | Nivel de automatización de procesos |
| $P_{automatizados}$ | Procesos ejecutados sin intervención manual |
| $P_{totales}$ | Total de procesos institucionales evaluados |

### Explicación de la fórmula

El número de procesos automatizados se divide entre el total de procesos existentes y se multiplica por 100. Un porcentaje mayor representa un nivel más alto de automatización institucional.

---

## 12. Tiempo de recuperación ante fallos (TRF)

### Explicación de la métrica

El Lago de Datos debe garantizar continuidad operativa para múltiples unidades administrativas. Esta métrica evalúa la resiliencia tecnológica, la capacidad de respuesta ante interrupciones y la estabilidad operativa de la plataforma. Reducir el tiempo de recuperación minimiza el impacto de fallas sobre los procesos institucionales.

### Fórmula

$$
TRF = T_{recuperacion} - T_{falla}
$$

### Componentes

| Componente | Descripción |
|:----------:|-------------|
| $TRF$ | Tiempo de recuperación ante fallos |
| $T_{recuperacion}$ | Momento en que el sistema vuelve a operar correctamente |
| $T_{falla}$ | Momento en que ocurrió la interrupción |

### Explicación de la fórmula

Se resta el momento de inicio de la falla al momento de recuperación del sistema. Mientras menor sea el resultado, mayor es la resiliencia tecnológica de la plataforma.

---

## 13. Índice de uso de recursos computacionales

### Explicación de la métrica

Esta métrica permite monitorear el uso de CPU, memoria, almacenamiento y capacidad de procesamiento de la infraestructura del lago. Es importante porque ayuda a optimizar recursos, prevenir saturaciones, mejorar el rendimiento y planear la expansión tecnológica futura. Un valor muy alto señala riesgo de saturación; un valor muy bajo puede indicar subutilización de infraestructura costosa.

### Fórmula

$$
U_{rec} = \frac{R_{utilizados}}{R_{disponibles}} \times 100
$$

### Componentes

| Componente | Descripción |
|:----------:|-------------|
| $U_{rec}$ | Porcentaje de uso de recursos computacionales |
| $R_{utilizados}$ | Recursos efectivamente utilizados (CPU, memoria, almacenamiento) |
| $R_{disponibles}$ | Recursos totales disponibles en la infraestructura |

### Explicación de la fórmula

Los recursos utilizados se dividen entre los recursos totales disponibles y se multiplica por 100. Se recomienda mantener el valor entre 60% y 85% para garantizar rendimiento óptimo sin riesgo de saturación.

---

## 14. Tasa de consultas exitosas

### Explicación de la métrica

El Lago de Datos será utilizado constantemente para búsquedas, análisis, consultas estadísticas y acceso a información geoespacial. Esta métrica permite identificar fallas operativas, errores de consulta, problemas de integración y limitaciones técnicas que afectan la experiencia y productividad de las personas usuarias.

### Fórmula

$$
Q_{exit} = \frac{Q_{exitosas}}{Q_{totales}} \times 100
$$

### Componentes

| Componente | Descripción |
|:----------:|-------------|
| $Q_{exit}$ | Tasa de consultas ejecutadas exitosamente |
| $Q_{exitosas}$ | Consultas completadas sin error |
| $Q_{totales}$ | Total de consultas realizadas en el período |

### Explicación de la fórmula

Las consultas exitosas se dividen entre el total de consultas realizadas y se multiplica por 100. Un porcentaje alto representa mejor estabilidad y funcionamiento operativo de la plataforma.

---

## 15. Índice de actualización de datasets

### Explicación de la métrica

Se requiere información estadística y geoespacial constantemente actualizada para sus procesos de análisis y generación de productos. Esta métrica evalúa la vigencia de la información disponible en el lago, el mantenimiento de datasets y la confiabilidad operativa de la plataforma, favoreciendo análisis precisos y decisiones oportunas.

### Fórmula

$$
IA_{datos} = \frac{D_{actualizados}}{D_{totales}} \times 100
$$

### Componentes

| Componente | Descripción |
|:----------:|-------------|
| $IA_{datos}$ | Porcentaje de datasets actualizados |
| $D_{actualizados}$ | Datasets que corresponden a la versión o fecha más reciente |
| $D_{totales}$ | Total de datasets registrados en el lago |

### Explicación de la fórmula

Los datasets actualizados se dividen entre el total de datasets registrados y se multiplica por 100. Un valor alto indica mayor vigencia de la información disponible en la plataforma.

---

## 16. Tasa de errores en procesamiento

### Explicación de la métrica

Esta métrica permite identificar problemas relacionados con integración de información, automatización, procesamiento y transformación de datos. Reducir la tasa de errores favorece la calidad institucional, la estabilidad tecnológica y la confiabilidad analítica de los productos estadísticos y geoespaciales generados.

### Fórmula

$$
E_{proc} = \frac{N_{errores}}{P_{ejecutados}} \times 100
$$

### Componentes

| Componente | Descripción |
|:----------:|-------------|
| $E_{proc}$ | Tasa de errores en procesamiento |
| $N_{errores}$ | Número de errores detectados durante la ejecución |
| $P_{ejecutados}$ | Total de procesos ejecutados en el período |

### Explicación de la fórmula

El número de errores se divide entre el total de procesos ejecutados y se multiplica por 100. Mientras menor sea el resultado, mayor es la estabilidad operativa de la plataforma.

---

## 17. Coeficiente de variación de estimadores muestrales

### Explicación de la métrica

Esta métrica es específica del contexto estadístico y aplica a las estimaciones generadas a partir de microdatos de encuestas como ENOE, ENIGH o ENSANUT almacenadas en el lago. Permite evaluar la precisión estadística de los resultados y garantizar que los análisis derivados del lago cumplan los estándares metodológicos del Instituto. El INEGI establece que estimaciones con $CV > 15\%$ requieren nota metodológica de uso y deben interpretarse con cautela.

### Fórmula

$$
CV = \frac{s}{\bar{x}} \times 100
$$

### Componentes

| Componente | Descripción |
|:----------:|-------------|
| $CV$ | Coeficiente de variación expresado en porcentaje |
| $s$ | Desviación estándar del estimador |
| $\bar{x}$ | Media del estimador |

### Explicación de la fórmula

La desviación estándar del estimador se divide entre su media y se multiplica por 100. El resultado indica la precisión relativa de las estimaciones derivadas de encuestas por muestreo. Valores menores indican estimaciones más precisas y confiables.

---

## 18. Índice de cobertura geográfica

### Explicación de la métrica

Esta métrica es exclusiva del contexto geoespacial. Evalúa si el lago contiene la totalidad de las unidades del Marco Geoestadístico Nacional: entidades federativas, municipios, localidades, AGEBs y manzanas. Una cobertura incompleta limitaría la capacidad de realizar análisis territoriales integrales, afectando la generación de estadísticas regionales y municipales.

### Fórmula

$$
ICG = \frac{U_{presentes}}{U_{oficiales}} \times 100
$$

### Componentes

| Componente | Descripción |
|:----------:|-------------|
| $ICG$ | Índice de cobertura geográfica |
| $U_{presentes}$ | Unidades geoestadísticas presentes en el lago |
| $U_{oficiales}$ | Total de unidades publicadas en el Marco Geoestadístico Nacional |

### Explicación de la fórmula

Las unidades geoestadísticas presentes en el lago se dividen entre el total oficial publicado y se multiplica por 100. Un valor cercano al 100% indica que el lago representa de forma completa el territorio nacional conforme al Marco Geoestadístico Nacional vigente.

---

## 19. Tasa de adopción por unidad administrativa

### Explicación de la métrica

Esta métrica complementa la percepción cualitativa de adopción con un dato objetivo y verificable. Permite identificar áreas que aún no utilizan la plataforma, orientar estrategias de capacitación diferenciada y medir el avance real de la implementación a lo largo del tiempo en toda la estructura del Instituto.

### Fórmula

$$
TAU = \frac{UA_{activas}}{UA_{totales}} \times 100
$$

### Componentes

| Componente | Descripción |
|:----------:|-------------|
| $TAU$ | Tasa de adopción por unidad administrativa |
| $UA_{activas}$ | Unidades administrativas con al menos una persona usuaria activa en el período |
| $UA_{totales}$ | Total de unidades administrativas del Instituto |

### Explicación de la fórmula

Las unidades administrativas con actividad registrada en el lago se dividen entre el total de unidades del Instituto y se multiplica por 100. Una tasa alta indica penetración real de la plataforma en la operación institucional.

---

## 20. Índice de eficiencia de almacenamiento

### Explicación de la métrica

En un lago de datos que integra fuentes tan diversas como censos, cartografía vectorial, microdatos de encuestas y registros administrativos, es común que una proporción del almacenamiento se ocupe en archivos temporales, versiones obsoletas o duplicados no detectados. A diferencia de una métrica de consumo total, esta evalúa la calidad del uso del espacio, no solo su cantidad, lo que permite optimizar infraestructura y reducir costos operativos.

### Fórmula

$$
IEA = \frac{A_{util}}{A_{fisico}} \times 100
$$

### Componentes

| Componente | Descripción |
|:----------:|-------------|
| $IEA$ | Índice de eficiencia de almacenamiento |
| $A_{util}$ | Almacenamiento utilizado por datos únicos y válidos |
| $A_{fisico}$ | Almacenamiento físico total consumido |

### Explicación de la fórmula

El almacenamiento ocupado por datos únicos y válidos se divide entre el almacenamiento físico total consumido y se multiplica por 100. Un valor alto indica que la mayoría del espacio se usa en información útil, con baja proporción de datos redundantes, temporales o corruptos.



