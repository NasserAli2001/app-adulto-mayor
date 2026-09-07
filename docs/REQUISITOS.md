# Requisitos de Acompaña+

P = Propuesta de Investigación del 23 de agosto de 2026. M = Modelo de Negocio del 24 de agosto, incluido el Canvas. C = cronograma, Sheet1. B = presupuesto. Referencias por secciones y celdas, sin atribuir páginas no verificadas.

El objetivo es un prototipo móvil para adultos de 60 años o más con estabilidad cognitiva que requieren apoyo en desplazamientos y diligencias. Incluye pruebas técnicas y de usabilidad, sin intervención clínica (P §§1.1, 3, 4). La familia puede solicitar por el beneficiario (M §2). El número de participantes se define con el asesor antes de las pruebas (P §4.2).

## Matriz de trazabilidad

Los criterios concretos son diseño propuesto para hacer comprobables los requisitos, sujeto a consulta de usuarios.

| ID | Requisito y fuente | Criterio de aceptación propuesto | Evidencia |
| --- | --- | --- | --- |
| R01 | Perfil y datos básicos; P §§3.2, 4.6 | Guardar y recuperar beneficiario con datos mínimos sin duplicación al reintentar | S9 |
| R02 | Autenticación y acceso; P §§4.6, 8.4 | Familia ajena no puede leer ni modificar servicios de otra; sesión cerrada pierde acceso | S9, S12–14 |
| R03 | Solicitud; P §§3, 5; M §2 | Adulto o familiar autorizado indica fecha, hora, origen, destino y diligencia; confirma una sola solicitud | S10 |
| R04 | Asignación y confirmación; P §3.2; M §§2, 4.1 | Operador asigna acompañante habilitado; solicitante ve confirmación | S10–11 |
| R05 | Seguimiento y registros; P §4.6; M §2 | Estados autorizados quedan fechados y persisten tras reiniciar | S11–12 |
| R06 | Reporte automático a la familia; M §2 | Al finalizar se genera un resumen único visible solo para familiares vinculados | S12 |
| R07 | Planes free/premium; P §4.7; M §5 | Mostrar modalidad de demostración sin inventar precios, cupos ni cobrar | S11–12 |
| R08 | Nube; P §4.6; B Servicios Técnicos A6:B6 | Registro guardado desde un equipo puede consultarse en otro con autorización | S9, S13 |
| R09 | Accesibilidad; P §§2, 5; M §2 | Textos ampliados, controles legibles, etiquetas y errores claros; recorrido probado en Android | S8, S13–15 |
| R10 | Pruebas técnicas; P §§4.4–4.5, 5 | Casos principales y negativos con resultados y correcciones vinculadas | S11–14 |
| R11 | Usabilidad y confidencialidad; P §§4.2–4.3, 8 | Instrumento y procedimiento revisados antes de aplicarlos; resultados anonimizados | S13–15 |
| R12 | Informe y anexos; P §§5, 10 | Matriz, diagramas, casos, instrumento, resultados, guía y limitaciones completos | S16 |

## Recorrido y permisos propuestos

Adulto o familiar vinculado inicia sesión, selecciona beneficiario, solicita servicio y consulta confirmación. Operador asigna al acompañante. Este ve solo sus asignaciones y registra inicio y finalización. La familia autorizada consulta el resumen final.

Estados propuestos: solicitada → asignada → en curso → completada. Cancelación previa al inicio con motivo e historial; cambios posteriores requieren regla explícita. No permitir saltos ni edición libre de servicios finalizados.

Los vínculos familiares requieren autorización; conocer un identificador no otorga acceso. Usar cuentas y acompañantes de demostración. Una marca simulada de verificación no equivale a una verificación real.

## Límites y decisiones pendientes

- Sin diagnósticos, recomendaciones clínicas, emergencias ni garantía de seguridad física (P §8; M §4.2).
- Seguimiento inicial por estados; GPS continuo no está especificado.
- Reporte inicial dentro de la app; el canal externo, notificaciones push o WhatsApp requieren definición y presupuesto.
- Transporte figura “parcial” en la tabla del modelo e integrado en su §8. Concretar coordinación, prestación y pago; registrar necesidad no equivale a proveer transporte.
- Mantener los planes aprobados. Cupo gratuito, significado de “ilimitado”, duración, tarifas, comisión y capacidad necesitan definición antes de programar cobros o restricciones reales.
- Operación física y contratación se distinguen del prototipo. Las pruebas académicas no deben implicar desplazamientos de riesgo (P §8.1).
- B2B, licenciamiento y cobros se conservan como visión comercial; no son entregables funcionales explícitos de las 16 semanas.
