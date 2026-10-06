# Guía de uso de los agentes del Narrador

### Instalar los agentes en otra campaña

El paquete distribuible contiene diez agentes preparados para Codex y adaptados para trabajar con los documentos de otra campaña. Incluye instrucciones y ejemplos; las aventuras, ilustraciones, fichas privadas y herramientas de exportación se aportan por separado.

1. Descarga y descomprime el paquete. En GitHub puedes descargar el repositorio desde **Code → Download ZIP**.
2. Abre la carpeta de tu campaña como proyecto local en Codex. Copia los diez archivos TOML del paquete a `.codex/agents/` dentro de esa carpeta. Si ya tienes agentes con esos nombres, conserva una copia y compara sus instrucciones antes de sustituirlos.
3. Facilita las escenas, fichas y reglas que quieras consultar. Añade un índice o README que indique cuáles son las fuentes actuales. Si tu proyecto tiene `AGENTS.md`, conserva sus normas; el paquete ofrece un ejemplo separado que puedes adaptar.
4. Inicia una conversación nueva en ese proyecto y pide que utilice uno de los agentes por su nombre. Si no aparece disponible, comprueba la carpeta, el nombre del archivo y el campo `name`; consulta la ayuda de tu versión de Codex. Pegar sus instrucciones en otro asistente puede servir como orientación, pero no instala el agente ni reproduce sus permisos.

### Pedir ayuda antes, durante y después de la sesión

Una petición útil indica **agente, escena o archivo, objetivo y estado real de la partida**. Por ejemplo: «Usa el resumidor para preparar la escena de la clínica. Los PJ rescataron al testigo, conservan su libreta y todavía no han avisado a su contacto. Resume entradas, decisiones, pistas y salidas; cita las fuentes».

Antes de jugar, usa **resumidor** para recuperar la situación y **revisor-jugabilidad** para comprobar pistas, alternativas y decisiones. Durante la partida, pide a **asistente-mesa** una consulta concreta: «¿Qué sabe este PNJ de lo ocurrido y qué puede revelar? Separa hechos, sospechas y secretos del Narrador». Al terminar, facilita el cierre real y pide a **revisor-continuidad** que localice las consecuencias que afectan a las próximas escenas.

Para editar el material, **revisor-legibilidad** propone correcciones de claridad y **revisor-coherencia-estructural** comprueba apartados y orden. **Gestor-pendientes** propone qué tareas están resueltas; **revisor-cierre-pendientes** puede marcar únicamente cierres verificados cuando le autorices expresamente a actualizar la lista. **Responsable-compilacion** genera la salida solicitada con el exportador que tenga tu proyecto; **revisor-maquetacion** comprueba visualmente esa salida cuando dispone de un visor y puede guardar capturas e informes.

Puedes combinar consultas: «Usa revisor-continuidad y revisor-jugabilidad para revisar esta escena y reúne sus propuestas». El agente principal coordina ese encargo, contrasta sus fuentes y entrega una síntesis. Pedir una revisión entrega propuestas; para incorporarlas indica expresamente qué cambios autorizas.

### Adaptarlos a tu mesa

Indica el sistema, la edición, las reglas propias y las fichas que realmente utilizas. Los agentes no incluyen un reglamento ni sustituyen los libros de juego. Añade el estado de la partida: una escena escrita describe lo que podría ocurrir, y el registro de sesión indica lo que ocurrió.

Los agentes de consulta trabajan en lectura. Los de compilación, maquetación y cierre tienen permisos de escritura limitados por su cometido; necesitan un encargo que autorice esa salida o actualización. Antes de sobrescribir, deben conservar copias verificadas. Revisa las fuentes citadas y los límites declarados: una comprobación de archivos no equivale a una revisión visual y una propuesta no se convierte por sí sola en canon.

Si compartes una respuesta con los jugadores, solicita una versión sin secretos y revísala antes de mostrarla. Para otra campaña, aporta sus documentos y convenciones: las versiones distribuibles no necesitan conocer los personajes ni las carpetas de Mago 2026.

## Referencia técnica

La instalación y el formato TOML se basan en la [documentación oficial de agentes personalizados de Codex](https://learn.chatgpt.com/docs/agent-configuration/subagents), consultada el 7 de octubre de 2026. No se fija un modelo: cada agente hereda la configuración disponible.
