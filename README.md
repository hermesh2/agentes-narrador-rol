# Agentes del Narrador para campañas de rol

Diez agentes en español para preparar sesiones, consultar escenas y revisar campañas en un proyecto local de Codex. Adaptación portable de los agentes creados para Mago 2026 — El coro de las sombras.

Empieza por la [guía de uso](GUIA-DE-USO.md). Copia los archivos de `.codex/agents/` a la carpeta del mismo nombre de tu campaña y aporta tus escenas y registros de sesión. No hace falta instalar un servidor, un plugin ni skills externas.

| Agente | Función y permisos |
|---|---|
| `resumidor` | Recordatorio breve para dirigir una escena. Solo lectura. |
| `asistente-mesa` | Consulta de escenas, relaciones y continuidad durante la partida. Solo lectura. |
| `revisor-continuidad` | Contrasta cronología, identidades, pistas y consecuencias. Solo lectura. |
| `revisor-jugabilidad` | Revisa decisiones, pistas, obstáculos y ritmo. Solo lectura. |
| `revisor-legibilidad` | Correcciones claras conservando voz y contenido. Solo lectura. |
| `revisor-coherencia-estructural` | Comprueba apartados, cobertura y orden. Solo lectura. |
| `revisor-maquetacion` | Revisa visualmente HTML y PDF; solo escribe capturas e informes nuevos. |
| `gestor-pendientes` | Revisa seguimiento y propone cierres con pruebas. Solo lectura. |
| `revisor-cierre-pendientes` | Verifica y marca únicamente cierres autorizados en el seguimiento. |
| `responsable-compilacion` | Genera y verifica exclusivamente las salidas solicitadas. |

## Qué incluye

- Diez configuraciones TOML, sin modelo fijado ni credenciales.
- Guía de instalación, adaptación y ejemplos antes, durante y después de jugar.
- `AGENTS.ejemplo.md`: normas opcionales de protección que puedes integrar en las de tu campaña.
- `MANIFIESTO.json`: versión, relación de archivos y hashes SHA-256.

Las versiones distribuidas conservan los cometidos y protecciones del proyecto de origen, pero sus instrucciones se han reescrito para no depender de sus nombres, rutas, skills, personajes ni exportadores. Los originales de Mago 2026 permanecen intactos. El paquete no incluye capítulos, ilustraciones, libros de reglas, fichas de PJ, datos privados ni herramientas de compilación. Los agentes de exportación necesitan las herramientas que aporte el proyecto destinatario.

## Comprobación de esta entrega

Se verifican los diez TOML, nombres únicos, permisos, hashes y contenido del ZIP. La instalación y el comportamiento en una campaña externa requieren una prueba en la versión de Codex del destinatario; no se afirma que esa prueba se haya realizado. Si tu entorno limita subagentes o escrituras, esos límites siguen aplicándose.
