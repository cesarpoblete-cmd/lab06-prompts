# Bitacora de prompts
Laboratorio 06: Fundamentos de Ingenieria de Prompts.
Herramienta de IA usada: (Gemini)
## Ejercicio 2: Tokens y ventana de contexto
| Texto | Caracteres | Tokens | 
|-------|------------|--------| 
| Los estudiantes programan en Java. |7 |34 | 
| The students program in Java. |6 |29 | 
| desafortunadamente |4 |18 |

En el paso 4 en el chat tenia una ventana de contexto motivo por el cual podia darme una respuesta en cambio en el paso 5 al ser un chat nuevo no contaba con ninguna informacion(ventana de contexto).

## Ejercicio 3: Temperatura
| Temperatura | % de BiblioTec | Nombres en los 5 intentos | 
|-------------|----------------|---------------------------| 
| 0 | 100| BiblioTec, BiblioTec, BiblioTec, BiblioTec, BiblioTec| 
| 0.5 | 84| BiblioTec, BiblioTec, BiblioTec, LibroYa, BiblioTec| 
| 1 | 55| BiblioTec, LibroYa, BiblioTec, PrestaLibro, LectoGo| 
| 1.8 | 32| BiblioTec, LibroYa, PrestaLibro, LectoGo, PaginaLibre|

Al subir la temperatura, los nombres elegidos cambian más y salen opciones menos probables.

## Ejercicio 4: Prompt vago vs estructurado
| Criterio | Prompt vago | Prompt estructurado | 
|----------|-------------|---------------------|
| Menciona el objetivo del sistema | no| si| 
| Menciona a los usuarios principales | no| si| 
| Tiene exactamente 3 funcionalidades | no| si| 
| Esta en 3 parrafos | no| si| 
| Lo usaria en un informe real | no| si|

## Ejercicio 5: Anatomia de un prompt

| Componente | Texto de mi prompt | 
|------------|--------------------|
| Rol | Actua como desarrollador Java.| 
| Instruccion | Usando una clase Producto con los atributos codigo, nombre, precio y stock.| 
| Contexto | Crea un programa en Java para gestionar los productos de  una tienda.| 
| Ejemplo | Usa este estilo para los metodos: getPrecio(), setPrecio(double precio).| 
| Formato | Explica primero la estructura de la clase y luego presenta el codigo Java|

Nivel 1: La IA generó un programa muy básico y genérico.

Nivel 2: Mejoró la estructura del código aplicando buenas prácticas.

Nivel 3: Se definio la clase `Producto` únicamente con los cuatro atributos (`codigo`, `nombre`, `precio` y `stock`).

Nivel 4: Se enfocó en el inventario de una tienda, creando clases y variables relacionadas con ventas o productos.

Nivel 5: Estandarizó los métodos *getters* y *setters* para que coincidieran con el estilo del ejemplo dado.

Nivel 6: Cambió el orden de la respuesta, mostrando primero una explicación de la clase antes de entregar el bloque de código.