# Tarea: Mi Prompt profesional

## Funcionalidad elegida
Cálculo de promedio final de notas de un estudiante en consola usando Java, validando que las notas estén entre 0 y 20.
## Version 1: prompt basico

```text
Crea un programa en Java que calcule el promedio de notas.
```

* **Qué cambié:** Es el punto de partida inicial.
* **Por qué:** Para probar qué genera la IA sin darle detalles.
* **Qué mejoró:** Aún nada, la respuesta fue muy genérica y sin validaciones.

markdown
## Version 2

```text
Actúa como desarrollador Java. Crea un programa de consola para calcular el promedio final de 3 notas de un estudiante, validando que cada nota esté entre 0 y 20.
```

* **Qué cambié:** Agregué un rol de desarrollador Java, el contexto (programa de consola para 3 notas) y una instrucción clara con rango de validación.
* **Por qué:** En la versión 1 la IA asumió datos aleatorios y no controlaba notas inválidas.
* **Qué mejoró:** El código ya pide los datos por teclado, valida el rango de 0 a 20 y calcula el promedio exacto.

## Version 3: prompt final

```text
Actúa como dev Java. Para una app escolar de consola, crea la clase CalculadoraNotas que promedie 3 notas (0 a 20). Sin librerías externas. Explica breve y luego da el código. Salida ejemplo: "Promedio: 15.5 - Aprobado".
```

* **Qué cambié:** Añadí una restricción (no usar librerías externas), un ejemplo exacto de salida en consola y el formato de entrega (explicación + código).
* **Por qué:** Para evitar código innecesario, asegurar que compile directo y controlar cómo se imprime el mensaje final.
* **Qué mejoró:** La respuesta salió ordenada, limpia, sin dependencias raras y con el mensaje exacto que necesitaba.

## Componentes del prompt final

| Componente | Texto de mi prompt |
| :--- | :--- |
| Rol | Actúa como dev Java. |
| Contexto | Para una app escolar de consola, |
| Instrucción | crea la clase CalculadoraNotas que promedie 3 notas (0 a 20). Sin librerías externas. |
| Formato | Explica breve y luego da el código. |
| Ejemplos | Salida ejemplo: "Promedio: 15.5 - Aprobado". |

## Evaluacion del resultado

| Criterio | Cumple (Sí / No) |
| :--- | :--- |
| ¿Usa Java sin librerías externas? | Sí |
| ¿Calcula el promedio validando notas de 0 a 20? | Sí |
| ¿Explica brevemente antes de mostrar el código? | Sí |
| ¿Imprime la salida con el formato del ejemplo? | Sí |

## Errores que evite

* **Ser demasiado general:** En lugar de pedir solo "un programa de notas", especifiqué el nombre de la clase, la cantidad de notas y el rango exacto de 0 a 20.
* **No indicar el formato:** Definí desde el inicio que quería primero una explicación breve y luego el código, además de dar un ejemplo exacto de la salida en consola.