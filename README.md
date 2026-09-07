# Acompaña+

Estado: preparación inicial, 7 de septiembre de 2026. No hay aplicación implementada todavía.

## Requisitos y documentos

La conversación anterior menciona propuesta, presupuesto, cronograma semanal y modelo de negocio, pero no contiene sus adjuntos. La carpeta sources de esta tarea está vacía. No se han revisado cifras, funcionalidades ni fechas. El modelo de negocio se considera aprobado según la declaración del usuario y no se modifica.

| Fuente pendiente | Revisión que se realizará |
| --- | --- |
| Propuesta | Objetivo, usuarios, alcance, funcionalidades y criterios de aceptación |
| Presupuesto | Moneda, cantidades por valor unitario, totales, costos iniciales y recurrentes, correspondencia con alcance |
| Cronograma | Número de semanas, fechas, entregables, dependencias y evidencia exigida |
| Modelo aprobado | Trazabilidad con requisitos; registrar inconsistencias sin reescribirlo |

Cada requisito tendrá identificador, documento y página de origen, criterio de aceptación, entrega y prueba. Las discrepancias se registrarán con ambas referencias, impacto y propuesta de resolución pendiente. No hay inconsistencias documentales verificadas aún.

## Arquitectura propuesta, pendiente de los documentos

Para una primera versión web: navegador del teléfono → HTTPS → aplicación Python/Django → base de datos.

- Django concentraría reglas de negocio, autenticación, permisos y administración en un único proyecto.
- Plantillas HTML, CSS y JavaScript mínimo para las pantallas. Python se utilizaría en el servidor; no sustituye el HTML del navegador.
- SQLite durante el desarrollo inicial; PostgreSQL para una versión desplegada con varios usuarios.
- Separar configuración, lógica de negocio, interfaz y pruebas. Los módulos funcionales se definirán al leer la propuesta.
- Diseñar textos legibles, controles amplios y navegación sencilla; comprobar las pantallas con personas mayores y en el teléfono real.
- Probar permisos entre usuarios, validaciones, persistencia y los recorridos principales. Usar datos ficticios durante el desarrollo.
- Seleccionar alojamiento, copias de seguridad y servicios externos después de contrastar el presupuesto. No se ha contratado ningún servicio.

Si se exige App Store, tareas en segundo plano, sensores o capacidades nativas, reevaluar el cliente móvil y conservar Python en el servidor mediante una API. No se asumen pagos, IA, geolocalización, alertas médicas ni otras funciones no verificadas.

Django incluye herramientas para modelos, vistas, plantillas y administración: [documentación oficial](https://www.djangoproject.com/start/overview/).

## Colab, entorno local y Xcode

| Herramienta | Uso en el proyecto |
| --- | --- |
| Google Colab | Aprender Python, explorar datos ficticios y probar algoritmos en cuadernos |
| Entorno local | Mantener el proyecto completo, ejecutar servidor y base de datos, probar interfaz y trabajar con Git |
| Codex | Ayudar a editar archivos, explicar cambios y ejecutar verificaciones en el proyecto |
| GitHub | Guardar versiones compartidas, tareas y propuestas de cambio |
| VS Code | Editor opcional; no es obligatorio |
| Xcode | Desarrollo y simulación de aplicaciones Apple en Mac |

Colab no será el servidor permanente: sus recursos y sesiones tienen límites y restricciones. Se pueden cargar cuadernos desde GitHub; editar uno no sincroniza automáticamente todo el proyecto. [FAQ oficial de Colab](https://research.google.com/colaboratory/faq.html).

El simulador de Apple se ejecuta en Mac. Esta tarea está en Windows; eso no impide desarrollar el servidor Python ni probar la web en el navegador. La vista móvil del navegador no sustituye las pruebas en Safari/iPhone. [Xcode y Simulator](https://developer.apple.com/xcode/).

## Flujo de trabajo semanal

1. Elegir un entregable respaldado por el cronograma y abrir una tarea con criterio de aceptación.
2. Actualizar la copia local y crear una rama, por ejemplo entrega/requisitos.
3. Pedir a Codex cambios concretos citando el requisito.
4. Ejecutar las pruebas correspondientes y revisar los archivos modificados.
5. Guardar una versión (commit) y enviarla a GitHub (push).
6. Abrir una propuesta de cambio (pull request), revisar e integrar en main.
7. Guardar evidencia de la entrega: versión, demostración, resultados y pendientes.

Una conversación no equivale a un cambio guardado en GitHub. Deben existir archivos y enviarse sus cambios. Conectar la cuenta tampoco instala automáticamente Python o Git en el equipo. No se ha configurado sincronización ni despliegue automáticos.

Referencia de herramientas: [documentación oficial de Codex](https://developers.openai.com/codex/).

## Plan provisional por entregas

Esta secuencia NO es el cronograma oficial, no fija fechas ni supone que el proyecto dure ocho semanas. Cada fila es un paquete que se asignará a las semanas reales cuando estén disponibles.

| Orden | Entrega | Evidencia para cerrar |
| --- | --- | --- |
| 0 | Modelo de negocio ya aprobado según usuario | Conservar versión original y registrar referencia |
| 1 | Requisitos, presupuesto y cronograma conciliados | Matriz con fuente y página; discrepancias señaladas |
| 2 | Arquitectura y prototipo de pantallas | Recorrido principal validado y decisiones justificadas |
| 3 | Base Python y persistencia | Instalación reproducible y prueba de lectura/escritura |
| 4 | Primer recorrido funcional de la propuesta | Demostración completa y pruebas de aceptación |
| 5 | Resto del alcance priorizado | Criterios del documento satisfechos y trazables |
| 6 | Validación y correcciones | Pruebas en teléfono, accesibilidad y permisos |
| 7 | Entrega final y documentación | Versión etiquetada, guía de uso y limitaciones |

Para cada semana oficial registrar: fecha, entregable textual, requisitos asociados, actividades, dependencia, evidencia, responsable y estado. La referencia anterior a “esta semana” no permite asignar el modelo de negocio a la semana actual.

## Próximos pasos

Adjuntar los cuatro documentos en la tarea para completar la revisión y reemplazar esta planificación provisional por el cronograma real. Confirmar si además del equipo Windows se dispone de un Mac solo cuando el alcance requiera Xcode.

El repositorio app-adulto-mayor es público al momento de la consulta. Esta preparación contiene exclusivamente documentación técnica general; los documentos originales y datos personales no forman parte de ella.
