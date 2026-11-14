# Prompts

Aquí van **todos los prompts que lanzaste** para hacer el ejercicio, en el orden en que los
lanzaste, con el modelo y la herramienta de cada uno.

Esto no es papeleo. Lo que se revisa es **cómo pediste las cosas**, no solo lo que salió: un
resultado flojo con un prompt bueno y un resultado flojo con un prompt vago necesitan feedback
distinto, y sin este archivo no se distinguen.

## Cómo rellenarlo

- Un apartado `## Prompt N` por cada prompt.
- **Pega el prompt tal cual lo lanzaste**, dentro del bloque de código, aunque ocupe diez líneas
  y aunque tenga faltas. No lo reescribas para que quede bien: el que arreglaste mentalmente
  después no es el que lanzaste.
- Incluye también los que **no funcionaron**. Suelen ser los más útiles de leer.
- `Modelo` y `Herramienta` en todos. Si cambiaste de una a otra a mitad, se nota aquí.

Borra el ejemplo de abajo cuando escribas el primero.

---

## Prompt 1

**Modelo:** Claude Opus 5.5
**Herramienta:** Claude Code

```
muéstrame las reglas de proceso del CLAUDE.md
```

**Qué salió:** Me las mostró tal cual y avisó de que algunas viñetas llevan varias reglas dentro.

## Prompt 2

**Modelo:** Claude Opus 5.5
**Herramienta:** Claude Code

```
no entiendo que respuesta tengo que dar
```

**Qué salió:** Me explicó que la apuesta es una nota mía (sí / no / ni idea por regla), no una respuesta para el agente.

## Prompt 3

**Modelo:** Claude Opus 5.5
**Herramienta:** Claude Code

```
sí, crea el archivo con la sección de apuesta
1r - si
2n - ni idea
3r - no
4t - ni idea 
5t - ni idea
```

**Qué salió:** Creó `docs/auditoria/crt.md` con la apuesta, la tabla vacía y las tres líneas.

## Prompt 4

**Modelo:** Claude Opus 5.5
**Herramienta:** Claude Code

```
audita las reglas contra los últimos 15 commits sin modificar archivos
```

**Qué salió:** Funcionó a la primera: tabla en el chat con 1 se cumple y 4 no se pueden comprobar; no tocó archivos.

## Prompt 5

**Modelo:** Claude Opus 5.5
**Herramienta:** Claude Code

```
sí, vuelca la tabla en crt.md
```

**Qué salió:** Volcó la tabla en el archivo, debajo de la apuesta.

## Prompt 6

**Modelo:** Claude Opus 5.5
**Herramienta:** Claude Code

```
añade los prompts a prompts.md
```

**Qué salió:** Este archivo.

## Prompt 7

**Modelo:** Claude Opus 5.5
**Herramienta:** Claude Code

```
ayúdame a escribir las tres líneas de la parte B
```

**Qué salió:** Me dio material y un borrador por línea, avisando de que debían ser mías.

## Prompt 8

**Modelo:** Claude Opus 5.5
**Herramienta:** Claude Code

```
usa los borradores tal cual y mételos en crt.md
```

**Qué salió:** Metió los tres borradores sin cambios en `crt.md`.

## Prompt 9

**Modelo:** Claude Opus 5.5
**Herramienta:** Claude Code

```
haz el commit, el push y abre el PR
```

**Qué salió:** Commit, push de `auditoria-crt` y PR contra `s5/start` del repo del curso.
