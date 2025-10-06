# Sistema de Boletos - Orquesta Sinfónica Nacional de Bolivia

## Herramientas

| Herramienta | Versión | Uso       |
| ----------- | ------- | --------- |
| Git         | 2.51.0  | Versiones |

## Configuración Inicial

- Descarga Git: [git-scm.com](https://git-scm.com/download/win)
- Verifica: `git --version`
- Configura: `git config --global user.name "Tu Nombre"`
- Configura: `git config --global user.email "tu.email@ejemplo.com"`
- Clona: `git clone https://github.com/sebastianccv/orquesta-tickets.git`
- Entra: `cd orquesta-tickets`

## Flujo de Trabajo

- Actualiza `main`: `git checkout main && git pull origin main`
- Crea rama: `git checkout -b tu-nombre/tarea` (e.g., `sebastianccv/reservas`)
- Edita: (usa VS Code)
- Agrega: `git add .`
- Commit: `git commit -m "Descripción"`
- Sube: `git push -u origin tu-nombre/tarea`
- Pull Request: (GitHub > Pull Requests > New > Base `main`, Compare `tu-nombre/tarea`)
- Actualiza rama: `git checkout tu-nombre/tarea && git merge main`
- Resuelve conflictos: `git add . && git commit && git push`

## Consejos

- No edites `main`
- Commits claros: e.g., "Agrego reservas"
- Sincroniza: `git pull origin main` antes
- Usa GitLens en VS Code
- Issues: crea en GitHub
