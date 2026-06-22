# Narrative Assistant

Skill para [Claude](https://claude.ai) que actúa como asistente de guión: genera y pule historias aplicando **11 Leyes Narrativas** basadas en *El Guión* de Robert McKee. El idioma de trabajo es **español**.

## ¿Qué hace?

Cuando le compartes una idea (personaje, setting, concepto), el asistente:

1. Identifica qué falta para cumplir los **4 prerrequisitos mínimos** antes de escribir cualquier escena:
   - Idea Controladora
   - Detonante
   - Objeto de Deseo del protagonista
   - Valor en juego de la escena
2. Pregunta y brainstormea la información faltante, una cosa a la vez, ofreciendo opciones concretas.
3. Nunca escribe una escena sin esos 4 prerrequisitos confirmados.
4. Aplica las 11 leyes activamente como filtro durante la escritura, no como checklist posterior.

## Las 11 Leyes Narrativas

| # | Ley | Pregunta clave |
|---|-----|----------------|
| 1 | Idea Controladora | ¿Cuál es el cambio de valor final y su causa? |
| 2 | El Gap | ¿Qué esperaba el protagonista y qué obtuvo en cambio? |
| 3 | Cambio de Valor | ¿Dónde empieza y termina el valor en juego de esta escena? |
| 4 | Subtext | ¿Qué hay debajo de lo que se dice? |
| 5 | Estructura | ¿En qué acto/secuencia estamos? ¿Qué punto de no retorno o clímax corresponde? |
| 6 | Personaje | ¿Cuál es el objeto de deseo, la necesidad y la contradicción del protagonista? |
| 7 | Detonante | ¿Qué evento rompió el equilibrio inicial? |
| 8 | Negación de la Negación | ¿Qué verdad más profunda recontextualiza todo en el clímax? |
| 9 | Escena Obligatoria | ¿Qué confrontación prometió la historia y cómo se entregará? |
| 10 | Progresión Obligatoria | ¿Esta escena/acto es más difícil y tiene más consecuencias que el anterior? |
| 11 | Elenco como Sistema | ¿Qué revela cada secundario que el protagonista no puede mostrar solo? |

El texto completo de cada ley está en [`references/leyes.md`](references/leyes.md).

## Estructura del repo

```
SKILL.md            # Definición del skill (instrucciones para Claude)
references/
  leyes.md           # Texto completo de las 11 leyes narrativas
```

## Instalación

Copia esta carpeta dentro de tu directorio de skills de Claude (por ejemplo `~/.claude/skills/narrative-assistant`) para que quede disponible como `/narrative-assistant`, o súbela como skill de proyecto siguiendo la documentación de [Claude Skills](https://docs.claude.com/claude-code).

## Uso

El skill se activa automáticamente cuando el usuario pide crear una historia, desarrollar un personaje, escribir una escena, construir una estructura dramática o menciona términos como protagonista, antagonista, escena, acto, detonante, clímax, conflicto o arco dramático.
