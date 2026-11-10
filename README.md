# Bitacora de prompts
 
Laboratorio 06: Fundamentos de Ingenieria de Prompts.

## Evidencias del laboratorio

- [Bitácora de prompts](prompts/BITACORA.md)
- [Tarea: Mi prompt profesional](prompts/TAREA.md)
 
Herramienta de IA usada: ChatGPT
 
## Ejercicio 2: Tokens y ventana de contexto

| Texto | Caracteres | Tokens |
|-------|------------|--------|
| Los estudiantes programan en Java. |34|7|
| The students program in Java. |29|6|
| desafortunadamente |7|27|

## Ejercicio 3: Temperatura

### Resultados de las pruebas

| Temperatura | % de BiblioTec | Nombres en los 5 intentos |
|-------------|----------------|---------------------------|
| 0 | 100.0% | BiblioTec, BiblioTec, BiblioTec, BiblioTec, BiblioTec |
| 0.5 | 65.3% | BiblioTec, BiblioTec, BiblioTec, BiblioTec, LibroYa |
| 1 | 44.5% | LibroYa, BiblioTec, BiblioTec, PrestaLibro, BiblioTec |
| 1.8 | 32.2% | BiblioTec, LectoGo, LibroYa, LibroYa, BiblioTec |

### Observaciones

Al aumentar la temperatura, las probabilidades se distribuyen entre las diferentes opciones, por lo que los nombres seleccionados pueden variar más.

El simulador nunca inventa un nombre nuevo porque solamente puede elegir entre las seis opciones definidas previamente en el código Java.
 
## Ejercicio 4: Prompt vago vs estructurado

| Criterio | Prompt vago | Prompt estructurado |
|----------|-------------|---------------------|
| Menciona el objetivo del sistema |Si|Si|
| Menciona a los usuarios principales |Si|Si|
| Tiene exactamente 3 funcionalidades |No|Si|
| Esta en 3 parrafos |No|Si|
| Lo usaria en un informe real |Si|Si|

### Observaciones

El prompt vago generó una respuesta más extensa y general, incluyendo siete funcionalidades y beneficios adicionales.

En cambio, el prompt estructurado produjo una respuesta más precisa, organizada en tres párrafos y con exactamente tres funcionalidades clave, cumpliendo las instrucciones solicitadas.
 
## Ejercicio 5: Anatomia de un prompt

### Cambios observados por nivel

- Nivel 1: La IA pidió más información porque la instrucción era muy general.
- Nivel 2: La IA asumió el rol de desarrollador Java, pero todavía necesitaba conocer el tipo de programa.
- Nivel 3: Al agregar el contexto, generó un sistema para gestionar productos de una tienda.
- Nivel 4: Al especificar la clase Producto y sus atributos, el código se ajustó a los requisitos solicitados.
- Nivel 5: Al indicar el formato, explicó primero la estructura de la clase y después presentó el código Java.

### Componentes del prompt final

| Componente | Texto de mi prompt |
|---|---|
| Rol | Actúa como desarrollador Java. |
| Instrucción | Crea un programa en Java. |
| Contexto | Para gestionar los productos de una tienda, utilizando una clase Producto con los atributos codigo, nombre, precio y stock. |
| Formato | Explica primero la estructura de la clase y luego presenta el código Java. |
| Ejemplo | Usa este estilo para los métodos: getPrecio(), setPrecio(double precio). |