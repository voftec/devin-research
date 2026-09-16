# AGENTS.md

Instrucciones para agentes (Devin Cloud y Devin Desktop) que trabajan en este repositorio.

## Contexto

Este repo se usa desde Devin en la nube y desde Devin Desktop/CLI. No requiere build ni dependencias.

## Estructura

- `research/` — investigaciones. Un archivo Markdown por tema.
- `docs/` — documentación derivada de las investigaciones.
- `EVALS/` — evaluaciones. Cada eval en su propia carpeta con `README.md`, casos y resultados.
- `MCP/` — configuración e instrucciones de MCP (Playwright). `.devin/mcp_config.json` es la copia que Devin Desktop carga solo.

### Estructura formal de `docs/`

```
docs/
  README.md        # índice de la documentación
  guias/           # cómo hacer X paso a paso
  referencia/      # especificaciones, definiciones, glosario
  decisiones/      # ADRs: NNNN-titulo.md (contexto, decisión, consecuencias)
  informes/        # informes finales derivados de research/ y EVALS/
```

Cada documento empieza con un encabezado:

```markdown
# Título
- Estado: borrador | revisado | final
- Fecha: AAAA-MM-DD
- Fuente: enlace a research/ o EVALS/ correspondiente
```

## MCP

- Playwright MCP está disponible para navegar y verificar UI; usarlo en las evaluaciones de `EVALS/` y guardar capturas en `resultados/`.
- Ver `MCP/README.md` para configuración en Cloud, Desktop u otros clientes.

## Convenciones

- Idioma: español.
- Archivos en Markdown, nombres en `kebab-case`.
- Cada PR debe describir qué se investigó/evaluó y por qué.
- No commitear credenciales ni datos sensibles.
