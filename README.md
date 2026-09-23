# ICN292_LAB3_Flores_Antonia

Repositorio correspondiente al Laboratorio 3 de la asignatura **Sistemas de Información para la Gestión (ICN292)**.

## Integrante

- **Nombre:** Antonia Flores
- **Rol:** 202360567-0
- **Semilla:** S = 368

## Descripción

El laboratorio consiste en la implementación de un flujo de procesamiento de solicitudes de devolución utilizando n8n.

El desarrollo considera un flujo principal de triage que recibe solicitudes mediante un webhook, evalúa las reglas de negocio y asigna cada solicitud a una de las siguientes rutas:

- APROBACION
- REVISION
- RECHAZO
- INVALIDA

Para la semilla utilizada en el laboratorio se trabajó con los siguientes parámetros:

- **U = $48.000**
- **D = 7 días**

Además, el flujo consulta una API pública para obtener el valor de la UF, registra los resultados en una Data Table y envía una notificación mediante Gmail.

También se implementó un segundo workflow encargado de generar un resumen de las solicitudes procesadas, incluyendo la cantidad de solicitudes por ruta, los montos asociados y la tasa de aprobación automática.

## Archivos principales

- `ICN292-Lab3-Flores-Antonia.pdf`: informe del laboratorio.
- `ICN292-Lab3-Flores-Antonia.tex`: código fuente del informe.
- `ICN292-Lab3-Flores-Antonia-triage.json`: workflow principal de clasificación.
- `ICN292-Lab3-Flores-Antonia-emisor.json`: workflow utilizado para enviar solicitudes al webhook.
- `ICN292-Lab3-Flores-Antonia-resumen.json`: workflow de resumen programado.
- `evidencias/`: capturas utilizadas para respaldar el funcionamiento de los workflows.

## Resultados

En la ejecución utilizada como evidencia se procesaron 15 solicitudes:

- Aprobación: 3
- Revisión: 5
- Rechazo: 7
- Inválida: 0

La tasa de aprobación automática obtenida fue de **20,00 %**.

## Herramientas utilizadas

- n8n
- Gmail
- Data Tables de n8n
- API pública de indicadores económicos de Chile
- LaTeX
- GitHub

## Observación

La Parte C del laboratorio no fue desarrollada completamente. Las pruebas y resultados presentados en este repositorio corresponden a las partes efectivamente implementadas y verificadas.
