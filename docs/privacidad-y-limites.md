# Privacidad y límites de interpretación

## Dónde están los datos

Todo se guarda en el almacenamiento local del navegador del dispositivo donde se usa. No hay servidor, base de datos ni cuentas. Nada sale del dispositivo salvo que la persona exporte un respaldo, descargue un CSV o copie la consulta para IA.

Consecuencias prácticas:

- Si se borran los datos del navegador, se pierde la información. Hay que exportar respaldos.
- Los archivos de respaldo y CSV contienen todo lo cargado. Deben guardarse donde la organización lo autorice.
- Dos personas que abren el mismo enlace no comparten datos.

## Sin datos identificables

- Pacientes e integrantes se identifican con un código interno.
- No cargar nombres, documentos, legajos, diagnósticos ni datos de contacto.
- La tabla que relaciona códigos con personas debe quedar en el sistema oficial de la organización, no en esta herramienta.
- Los datos de ejemplo del repositorio son ficticios. No subir datos reales a un repositorio público.

## No es una historia clínica ni apoyo a decisiones clínicas

El módulo de medicación sirve para gestionar y auditar el proceso: qué se indicó, qué se registró y dónde hay vacíos. No reemplaza el registro clínico legal, no valida dosis, no detecta interacciones ni contraindicaciones, y la alerta de alergias es una coincidencia de texto. Toda decisión sobre un paciente corresponde a un profesional habilitado.

## Control de acceso

Esta versión no tiene usuarios ni contraseñas. El resumen individual queda protegido solo por quién tiene acceso al dispositivo. Para un uso con acceso por rol y datos compartidos hace falta una versión con servidor y autenticación, administrada por el área de sistemas de la organización.

## Uso justo de los indicadores

- Cada indicador muestra su definición junto al valor.
- Los indicadores describen procesos, no personas. Un valor bajo abre una pregunta, no cierra una evaluación.
- Las frecuencias de eventos se calculan para el sitio y los eventos se registran sin identificar personas. No se usan como puntaje individual: reflejan diferencias de exposición y de cultura de reporte, no desempeño, y usarlas así desalienta el reporte.
- "Días sin accidentes" es un dato informativo. Convertirlo en objetivo o premio presiona a no reportar.
- La carga por turno se muestra siempre junto a la dotación.
- Cualquier registro se puede corregir. Si alguien señala un dato incorrecto, se corrige antes de sacar conclusiones.

## Consulta a una IA

La consulta que prepara el asistente incluye solo indicadores agregados y tipos de hallazgo con su cantidad, sin códigos de pacientes ni de integrantes. Aun así, conviene revisarla antes de enviarla y usar únicamente los servicios de IA que la organización autorice.

## Antes de usar datos reales

Validar con las áreas de legales, protección de datos y salud ocupacional, y con la normativa de datos personales y de salud del país donde se opera.
