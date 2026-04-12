# Desarrollo: commits y pull requests

Todo lo siguiente aplica al trabajo en este repositorio. Redacta **siempre en castellano** mensajes de commit, títulos/cuerpos de PR y comentarios de revisión que el equipo espere en español.

## Commits

### Comentarios preemptivos (*pre-emptive commit comments*)

- Referencia: [Preemptive commit comments — Arialdo Martini](https://arialdomartini.wordpress.com/2012/09/03/pre-emptive-commit-comments/).
- **Regla #2 (obligatoria en espíritu):** el mensaje describe **qué hace o en qué estado queda el software** tras el commit (comportamiento o resultado útil para quien lee el historial), **no** la crónica de lo que hizo la persona (“arreglé”, “cambié archivo X”) ni la primera persona del trabajo.
- Cuando encaje el flujo, conviene **pensar o bosquejar el mensaje antes** de terminar el cambio, como intención clara del commit.

### Commits atómicos

- Un commit = **un objetivo cohesivo** y pequeño; evita mezclar refactors masivos con features o doc no relacionada en el mismo commit.

### Conventional Commits

- Usa el formato estándar para el **tipo** visible al inicio, por ejemplo: `feat:`, `fix:`, `docs:`, `chore:`, `refactor:`, `test:`, etc.  
- Referencia: [Conventional Commits](https://www.conventionalcommits.org/).

### Firma GPG

- Los commits en este repositorio deben ir **firmados con GPG** cuando la configuración local del usuario tenga `commit.gpgsign=true` (o el equivalente `git commit -S`). No se desactiva la firma por defecto.

## Pull requests

- **Idioma:** castellano en título y descripción (salvo convención explícita del proyecto en otro idioma).
- **Cantidad de commits:** lo saludable es **como máximo cinco** commits por PR; si hay más, **sugiere** squash o rebase interactivo antes del merge o de la revisión final.
- **Tiempo de revisión:** lo saludable es que el PR se pueda entender en **como máximo ~10 minutos**. Si el avance se **acerca** a ese límite, **sugiere abrir el PR**; si **ya lo superó**, insiste con más fuerza en **fragmentar** el alcance o cerrar un PR parcial.
- **Descripción:** un **resumen en dos líneas** que cubra **todo** lo relevante del PR.
- **Listado de cambios:** **no** incluir por defecto un inventario de archivos o cambios. **Excepción:** si estimas que el PR lleva **más de ~5 minutos** de lectura, puedes añadir un listado **solo** de los **cambios más importantes**, **máximo 5 archivos**, **una línea** de descripción por archivo.

## Rol del asistente

- **Tras cada interacción** en la que el usuario y el asistente hayan trabajado sobre el repositorio, el asistente **sugerirá crear un commit** cuando haya **cambios concretos** en archivos (o un conjunto cohesivo listo para versionar). Incluye un **mensaje propuesto** en castellano, con **Conventional Commits** y el espíritu de la **regla #2** (comportamiento o estado del proyecto, no relato de la sesión). Si la interacción fue solo consultiva y **no** hubo ediciones que deban persistirse, indícalo en **una línea** y omite la sugerencia de commit.
- **Firma GPG:** al ejecutar o sugerir `git commit`, el asistente debe asumir **`commit.gpgsign=true`** (p. ej. `git commit -S` si hace falta forzar firma en un comando concreto). **No** sugieras ni uses `commit.gpgsign=false`, `-c commit.gpgsign=false` ni ningún atajo que desactive la firma. **No** modifiques la configuración de Git del usuario para apagar GPG. Solo si el usuario lo pide **por escrito** y de forma explícita, puedes seguir su instrucción y dejar constancia del trade-off de seguridad.
- Al preparar commits o PRs, aplica estas reglas y recuerda el enlace de **preemptive commits** cuando propongas mensajes.
- Si el usuario va en contra de estos criterios por una razón puntual, respeta su instrucción explícita pero advierte brevemente el trade-off.
