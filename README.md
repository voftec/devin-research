# Devin-research

Repositorio plantilla de investigación y evaluación para Devin (Cloud y Desktop).

## Cómo usarlo

- **Como template**: botón **Use this template → Create a new repository** en GitHub (crea una copia limpia sin historial).
- **Clonar**: `git clone https://github.com/voftec/devin-research.git`
- **Descargar ZIP**: **Code → Download ZIP**, o `curl -L https://github.com/voftec/devin-research/archive/refs/heads/main.zip -o devin-research.zip`

## Devin Desktop / CLI

1. Cloná el repo y abrí la carpeta en Devin Desktop (o corré `devin` dentro de ella).
2. Devin lee automáticamente `AGENTS.md` (reglas del proyecto) y `.devin/mcp_config.json` (MCP de Playwright).
3. Requisitos: Node.js 18+ para que `npx` levante el servidor MCP la primera vez.

## Devin Cloud

Creá una sesión sobre este repo; Devin lee `AGENTS.md`. Los MCP se agregan en Settings → MCP Marketplace (ver `MCP/README.md`).

## Estructura

- `AGENTS.md` — instrucciones para Devin (y otros agentes) al trabajar en este repo.
- `research/` — notas e investigaciones.
- `docs/` — documentación.
- `EVALS/` — evaluaciones (casos, resultados y criterios).
- `MCP/` — configuración e instrucciones de los servidores MCP (Playwright).
- `.devin/mcp_config.json` — MCP cargado automáticamente por Devin Desktop/CLI.
