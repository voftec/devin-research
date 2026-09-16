# AGENTS.md

Instrucciones para agentes (Devin Cloud) que trabajan en este repositorio.

## Contexto

Este repo se usa principalmente desde Devin en la nube. No requiere build ni dependencias.

## Estructura

- `research/` — investigaciones. Un archivo Markdown por tema.
- `docs/` — documentación derivada de las investigaciones.
- `EVALS/` — evaluaciones. Cada eval en su propia carpeta con `README.md`, casos y resultados.

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

## Convenciones

- Idioma: español.
- Archivos en Markdown, nombres en `kebab-case`.
- Cada PR debe describir qué se investigó/evaluó y por qué.
- No commitear credenciales ni datos sensibles.
