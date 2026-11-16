# Diccionario de indicadores

Todos los indicadores se calculan sobre el período y los filtros elegidos en el tablero, salvo los marcados como "estado actual".

| Indicador | Cómo se calcula | Límites de interpretación |
|---|---|---|
| Actividades registradas | Cantidad de controles, atenciones, inspecciones y capacitaciones registradas en el período. | Mide volumen, no calidad ni esfuerzo. Compararlo siempre con dotación y condiciones del turno. |
| Cumplimiento de tareas | Tareas completadas dentro del plazo ÷ tareas con plazo en el período. | Un valor bajo puede indicar plazos poco realistas o sobrecarga, no falta de compromiso. |
| Seguimiento documentado | Actividades con seguimiento documentado ÷ actividades que requerían seguimiento. | Depende de que se marque correctamente qué requiere seguimiento. |
| Capacitación vigente | Cursos y habilitaciones vigentes hoy ÷ cursos registrados. | Sirve para planificar actualizaciones, no para calificar personas. |
| Calidad del registro | Registros marcados como completos ÷ registros revisados en el período. | Requiere un criterio escrito y compartido de qué es un registro completo. |
| Carga por turno | Actividades del turno ÷ integrantes activos del turno. | Los turnos no son comparables sin considerar dotación, clima, distancias y tipo de operación. |
| Disponibilidad de equipamiento (estado actual) | Equipos en estado operativo ÷ equipos registrados. | No pondera criticidad: un solo equipo crítico fuera de servicio puede pesar más que el porcentaje. |
| Insumos bajo mínimo (estado actual) | Cantidad de insumos con stock actual menor al stock mínimo definido. | El mínimo debe revisarse según consumo real y tiempos de reposición del sitio. |
| Ejecución de presupuesto | Monto ejecutado ÷ monto presupuestado de los meses incluidos en el período. | Sobre o subejecutar no es bueno ni malo por sí mismo; hay que mirar el motivo. |
| Adherencia de medicación | Dosis administradas (incluye demoradas) ÷ dosis esperadas según la indicación. No cuenta medicación a demanda ni dosis futuras. | Una dosis sin registro no prueba que no se administró. Es un indicador de proceso, no una evaluación clínica. |

## Indicadores de eventos HSE

| Indicador | Cómo se calcula | Límites de interpretación |
|---|---|---|
| Frecuencia de eventos registrables | Eventos con tratamiento médico o con días perdidos × base ÷ horas trabajadas. La base (un millón o 200.000 horas) se elige en Ajustes. | Con pocas horas o períodos cortos, un solo evento mueve mucho el valor. Mirar períodos de 12 meses. |
| Frecuencia de eventos con días perdidos | Eventos con días perdidos × base ÷ horas trabajadas. | Un valor bajo sostenido puede indicar buena gestión o bajo reporte; leerlo junto con los casi accidentes. |
| Días perdidos | Suma de los días perdidos de los eventos del período. | Depende del criterio médico de alta; no sirve para comparar gravedad entre sitios distintos. |
| Casi accidentes reportados | Cantidad de casi accidentes registrados en el período. | Más reportes suele ser señal de buena cultura preventiva, no de más riesgo. |
| Acciones correctivas en plazo | Acciones cerradas dentro del plazo ÷ acciones con plazo en el período. | Cerrar en plazo no garantiza que la acción fue eficaz; conviene verificarla en terreno. |
| Días sin accidentes con días perdidos | Días transcurridos desde el último evento con días perdidos registrado. | No usarlo como objetivo ni como premio: presiona a no reportar. |

Las horas trabajadas se cargan por mes. Si el período elegido incluye meses parciales, la frecuencia usa las horas del mes completo, por lo que conviene elegir períodos de meses enteros o de 12 meses.

## Metas y semáforo

Cada indicador preventivo tiene una meta editable en Ajustes (por defecto 90%, y 95% para capacitación).

- **En meta**: el valor iguala o supera la meta.
- **Cerca de la meta**: hasta 10 puntos por debajo.
- **Bajo la meta**: más de 10 puntos por debajo.

La comparación "frente al período anterior" usa un período de la misma duración inmediatamente previo al elegido.

## Reglas del asistente

El asistente no usa un modelo de IA: aplica reglas fijas sobre los registros, para que cada hallazgo se pueda explicar y verificar.

**Medicación**

- Adherencia menor al 80% en los últimos 7 días.
- Dosis esperadas sin registro el día anterior.
- Más dosis registradas en un día que las indicadas.
- Dos indicaciones activas del mismo medicamento para el mismo paciente.
- Indicación activa sin prescriptor.
- Medicamento cuyo nombre coincide con una alergia registrada del paciente (coincidencia de texto; no detecta familias de fármacos ni reacciones cruzadas).
- Administraciones con fecha fuera del período de la indicación.
- Omisiones o rechazos sin motivo.
- Medicamento controlado sin responsable del registro.

**Eventos HSE**

- Acciones correctivas abiertas con plazo vencido.
- Eventos de los últimos 90 días (salvo casi accidentes) sin acción correctiva.
- Menos casi accidentes que lesiones en 90 días.
- Horas trabajadas del mes anterior sin cargar.

**Recursos, equipo y gestión**

- Insumos bajo mínimo, vencidos o que vencen en 30 días.
- Equipos fuera de servicio y calibraciones vencidas o por vencer.
- Cursos vencidos o que vencen en 30 días.
- Tareas vencidas sin completar.
- Seguimientos pendientes de documentar (últimos 90 días).
- Calidad del registro menor al 90% (últimos 30 días).
- Diferencia de carga por persona mayor al 50% entre turnos.
- Rubros de presupuesto sobreejecutados.

Los umbrales están en la función `hallazgos()` de `index.html` y se pueden ajustar.
