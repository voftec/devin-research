# MCP

Servidores MCP del proyecto. Incluye **Playwright MCP** (`@playwright/mcp`) para que el agente navegue, haga clic, complete formularios y saque capturas de páginas web.

## Devin Desktop / Devin CLI (local)

No hay que hacer nada: al abrir el repo se carga `.devin/mcp_config.json` automáticamente (config a nivel proyecto). Requisitos: Node.js 18+ (`npx` descarga el servidor la primera vez).

- Claves personales: `.devin/mcp_config.local.json` (ignorado por git).
- Config global (todos los proyectos): `~/.config/devin/mcp_config.json` (`%APPDATA%\devin\mcp_config.json` en Windows).

## Devin Cloud

Los MCP se configuran a nivel organización en **Settings → MCP Marketplace** (https://app.devin.ai/settings/mcp-marketplace). Agregá un servidor personalizado con el mismo contenido de `MCP/mcp_config.json` (la entrada `playwright`).

## Otros clientes (Cursor, Claude Desktop, VS Code)

Copiá el bloque `playwright` de `MCP/mcp_config.json` al archivo de configuración MCP del cliente; el formato `mcpServers` es el mismo.

## Instrucciones para el agente

- Usar Playwright MCP para verificar UI y flujos web dentro de `EVALS/`.
- Guardar capturas en `EVALS/<nombre-eval>/resultados/`.
- Modo headless por defecto; agregar `"--headed"` a `args` para ver el navegador.
- Nunca guardar credenciales en `mcp_config.json`; usar `mcp_config.local.json` o variables de entorno.
