# Tablero de equipo, recursos y medicación

Herramienta gratuita y de código abierto para equipos de salud ocupacional y operaciones en petróleo, minería y grandes industrias. Permite cargar integrantes, actividades, tareas, capacitaciones, equipamiento, insumos, presupuesto y el registro de medicación de pacientes, y ver indicadores, tendencias y problemas detectados automáticamente.

Es un solo archivo (`index.html`). No necesita instalación, servidor ni cuenta. Los datos quedan en el navegador de quien la usa.

## Qué incluye

- **Resumen gerencial**: pensado para la gerencia de HSE. Días sin accidentes con días perdidos, resumen ejecutivo en lenguaje simple (qué va bien, qué necesita atención, decisiones sugeridas), frecuencias de eventos, indicadores preventivos frente a su meta con semáforo, seis gráficos y botón para imprimir o guardar en PDF.
- **Tablero operativo**: nueve indicadores con su definición a la vista, tendencias por semana o mes, filtros por turno y rol, y carga por turno junto a la dotación.
- **Eventos HSE**: casi accidentes, lesiones, daño material y ambiental, con acción correctiva y plazo, más las horas trabajadas del sitio para calcular frecuencias. Los eventos no identifican personas.
- **Equipo**: integrantes (por código), capacitaciones y vencimientos.
- **Actividades y tareas**: controles, atenciones, inspecciones y capacitaciones, con seguimiento y calidad del registro.
- **Recursos**: equipamiento y calibraciones, insumos con stock mínimo y vencimiento, capital y presupuesto.
- **Medicación**: pacientes por código, indicaciones, registro de administración y auditoría de adherencia diaria, semanal, mensual y anual.
- **Asistente**: recorre todos los registros con reglas explicables, lista los problemas por prioridad con qué revisar, y prepara una consulta anonimizada para pegar en un asistente de IA.
- **Definiciones y privacidad**: diccionario de indicadores y límites de interpretación.
- **Ajustes**: turnos, roles, tipos de actividad, metas de cada indicador y base de las frecuencias (por millón o por 200.000 horas).

La primera vez abre con datos ficticios. "Empezar en blanco" los borra.

## Cómo usarla

1. Descarga `index.html` y ábrelo con doble clic, o publícalo (ver abajo) y comparte el enlace.
2. En **Ajustes**, define turnos, roles y tipos de actividad de tu equipo.
3. Carga integrantes, luego actividades, tareas, recursos y medicación.
4. Usa **Exportar respaldo** con frecuencia: si se borran los datos del navegador, se pierde la información.

Cada persona que abre el enlace ve solo sus propios datos. Para pasar datos entre dispositivos se usa Exportar e Importar.

## Publicarla con GitHub Pages

1. Crea un repositorio público en GitHub y sube el contenido de esta carpeta.
2. En el repositorio: Settings → Pages → Source: "Deploy from a branch" → rama `main`, carpeta `/ (root)`.
3. En un par de minutos queda disponible en `https://TU-USUARIO.github.io/NOMBRE-DEL-REPO/`. Ese es el enlace para compartir.

## Antes de usar datos reales

Lee [docs/privacidad-y-limites.md](docs/privacidad-y-limites.md). En resumen: usa códigos en lugar de nombres, no es una historia clínica ni un sistema de apoyo a decisiones clínicas, no tiene control de acceso y debe validarse con las áreas de legales, protección de datos y salud ocupacional de cada organización.

## Documentación

- [Diccionario de indicadores](docs/diccionario-kpi.md)
- [Privacidad y límites de interpretación](docs/privacidad-y-limites.md)

## Licencia

MIT. Puedes usarla, adaptarla y compartirla libremente.
