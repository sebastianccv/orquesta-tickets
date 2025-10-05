# Sistema de Boletos - Orquesta Sinfónica Nacional de Bolivia

¡Hola, Los Pequeños! Este es el repositorio para nuestro sistema de boletos (`https://github.com/sebastianccv/orquesta-tickets`). Aquí construiremos la compra de boletos online/presencial, con gestión de asientos y QR. Este `README.md` guía cómo usar Git para colaborar sin conflictos.

## Herramientas

| Herramienta | Versión | Uso                                  |
| ----------- | ------- | ------------------------------------ |
| Git         | 2.51.0  | Control de versiones para el código. |

## Configuración Inicial

1. **Instalar Git**:

   - Descarga: [git-scm.com](https://git-scm.com/download/win).
   - Verifica: `git --version` (debe mostrar 2.51.0).

2. **Configurar Nombre/Correo**:

   - Usa tu correo de GitHub:
     ```bash
     git config --global user.name "Tu Nombre"
     git config --global user.email "tu.email@ejemplo.com"
     ```

3. **Autenticación (HTTPS)**:

   - Crea un Personal Access Token (PAT) en GitHub > Settings > Developer settings > Personal access tokens > Tokens (classic) > Permisos `repo`.
   - Usa tu username y PAT al hacer `git push` o `git pull`.

4. **Clonar Repo**:
   - Clona: `git clone https://github.com/sebastianccv/orquesta-tickets.git`
   - Entra: `cd orquesta-tickets`

## Flujo de Trabajo

Usamos ramas personales y Pull Requests (PR) para evitar conflictos.

1. **Actualizar `main`**:

   - Sincroniza: `git checkout main && git pull origin main`
   - _Trae los últimos cambios de GitHub._

2. **Crear Rama**:

   - Usa tu nombre: `git checkout -b tu-nombre/tarea` (e.g., `sebastianccv/reservas`)
   - _Crea una rama para tu trabajo._

3. **Editar y Commit**:

   - Edita en VS Code.
   - Agrega: `git add .`
   - Commit: `git commit -m "Descripción corta"`
   - _Guarda cambios localmente._

4. **Subir Rama**:

   - Push: `git push -u origin tu-nombre/tarea`
   - _Sube tu rama a GitHub._

5. **Crear Pull Request**:

   - En GitHub, ve a Pull Requests > New pull request > Base: `main`, Compare: `tu-nombre/tarea`.
   - Describe y asigna revisores.
   - _Propón tus cambios para revisión._

6. **Actualizar tu Rama**:
   - Si otros mergean a `main`: `git checkout tu-nombre/tarea && git merge main`
   - Resuelve conflictos manualmente, luego: `git add . && git commit && git push`
   - _Mantiene tu rama actualizada._

## Consejos

- **No edites `main`**: Usa ramas personales.
- **Commits claros**: E.g., "Agrego endpoint reservas".
- **Sincroniza seguido**: Pull de `main` antes de trabajar.
- **Usa GitLens**: Extensión de VS Code para ver cambios.
- **Issues**: Crea Issues en GitHub para tareas.

¡A colaborar, Los Pequeños! Pregunta a Sebastian (@sebastianccv) si hay dudas.
