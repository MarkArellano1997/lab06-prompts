# Tarea: Mi prompt profesional

## Funcionalidad elegida

La funcionalidad elegida es la **gestión de productos para la aplicación TiendaTec**, desarrollada en Java Swing.

El sistema permitirá administrar los productos de una tienda mediante una interfaz gráfica. Cada producto tendrá los siguientes atributos:

- Código: identificador único del producto.
- Nombre: descripción del producto.
- Precio: valor de venta.
- Stock: cantidad disponible.

Las operaciones principales serán registrar, listar, buscar, actualizar y eliminar productos.

**Tecnologías:** Java, Java Swing y ArrayList para almacenar temporalmente los productos en memoria.

## Version 1: prompt básico

**Prompt utilizado:**

```text
Crea un programa en Java para gestionar productos de una tienda.
```

**¿Qué cambié?**

Esta primera versión contiene una instrucción muy general. Solamente indiqué que necesitaba un programa para gestionar productos.

**¿Por qué lo cambié?**

Porque el prompt no especificaba qué información debía tener cada producto ni qué operaciones debía realizar el sistema.

**¿Qué mejoró en la respuesta?**

Obtuve una propuesta inicial, pero la respuesta podía ser demasiado general y no necesariamente cumplir con las características que necesitaba para mi aplicación.

## Version 2: prompt mejorado

**Prompt utilizado:**

```text
Actúa como desarrollador Java. Crea un programa para gestionar
los productos de una tienda utilizando programación orientada
a objetos.

Cada producto debe tener los atributos codigo, nombre, precio
y stock.

El sistema debe permitir registrar, listar, buscar y actualizar
productos. Utiliza una clase Producto con atributos privados,
constructor y métodos getters y setters.

Explica el funcionamiento del programa y presenta el código Java.
```

**¿Qué cambié?**

Agregué un rol para la inteligencia artificial, definí los atributos de la clase Producto y especifiqué las operaciones principales del sistema.

**¿Por qué lo cambié?**

Para proporcionar mayor contexto y evitar que la inteligencia artificial genere un programa que no corresponda con las necesidades de mi aplicación.

**¿Qué mejoró en la respuesta?**

La respuesta fue más específica y organizada. Se incorporaron conceptos de programación orientada a objetos, encapsulamiento, constructores y métodos de acceso.

## Version 3: prompt final

**Prompt utilizado:**

```text
ROL:
Actúa como desarrollador de software especializado en Java,
programación orientada a objetos y desarrollo de interfaces
gráficas con Java Swing.

INSTRUCCIÓN:
Desarrolla una funcionalidad de gestión de productos para
la aplicación TiendaTec. El sistema debe permitir registrar,
listar, buscar, actualizar y eliminar productos.

CONTEXTO:
TiendaTec es una aplicación de escritorio para administrar
los productos de una tienda. Está desarrollada en Java Swing.
Cada producto contiene los atributos codigo, nombre, precio
y stock.

Utiliza una clase Producto con atributos privados, constructor,
getters y setters. Utiliza ArrayList para almacenar los productos
temporalmente en memoria.

EJEMPLOS:
Ejemplo de registro:
Código: P001
Nombre: Laptop Lenovo
Precio: 2500.00
Stock: 10

Resultado esperado:
Producto registrado correctamente.

Ejemplo de búsqueda:
Código: P001

Resultado esperado:
Se muestran el código, nombre, precio y stock del producto.

Si se intenta registrar nuevamente el código P001,
el sistema debe informar que el código ya existe.

RESTRICCIONES:
- No utilices librerías externas.
- Utiliza únicamente las herramientas estándar de Java y Java Swing.
- No utilices bases de datos.
- Valida que el precio y el stock no sean negativos.
- Mantén el código organizado y aplica encapsulamiento.

FORMATO DE RESPUESTA:
Presenta el resultado organizado en las siguientes secciones:
1. Descripción de la funcionalidad.
2. Estructura de las clases.
3. Código Java completo de cada archivo.
4. Explicación del funcionamiento.
5. Ejemplo de ejecución.

El código debe ser coherente, compilable y fácil de comprender.
```

**¿Qué cambié?**

Incorporé los cinco componentes de un prompt profesional: rol, instrucción, contexto, ejemplos y formato. También agregué restricciones técnicas y validaciones para controlar el comportamiento del programa.

**¿Por qué lo cambié?**

Porque necesitaba que la inteligencia artificial comprendiera el propósito de TiendaTec, las tecnologías que debía utilizar y las condiciones que debía respetar al generar el código.

**¿Qué mejoró en la respuesta?**

La respuesta esperada es más precisa, estructurada y relacionada con los requerimientos de la aplicación. Además, los ejemplos permiten comprender el comportamiento esperado y las restricciones ayudan a evitar soluciones que utilicen tecnologías innecesarias.

## Componentes del prompt final

| Componente | Identificación dentro del prompt | Función |
|---|---|---|
| Rol | Actúa como desarrollador de software especializado en Java. | Define el perfil que debe asumir la IA. |
| Instrucción | Desarrolla una funcionalidad de gestión de productos. | Establece lo que debe realizar. |
| Contexto | TiendaTec es una aplicación de escritorio desarrollada en Java Swing. | Explica el proyecto y sus características. |
| Ejemplos | Registro, búsqueda y validación del código P001. | Muestra el comportamiento esperado. |
| Formato | Descripción, estructura, código, explicación y ejecución. | Organiza la presentación de la respuesta. |

## Evaluación del resultado

Se establecieron los siguientes criterios para comprobar si la respuesta generada cumple con los requerimientos del prompt profesional.

| Criterio de evaluación | Sí / No |
|---|---|
| ¿La respuesta utiliza Java y Java Swing? | Sí |
| ¿Implementa los atributos codigo, nombre, precio y stock? | Sí |
| ¿Aplica encapsulamiento mediante atributos privados? | Sí |
| ¿Permite registrar, listar, buscar y actualizar productos? | Sí |
| ¿Incluye la operación de eliminar productos? | Sí |
| ¿Valida códigos duplicados, precios y stock? | Sí |
| ¿Presenta el código organizado y explicado? | Sí |
| ¿Respeta las restricciones establecidas? | Sí |

## Errores que evité

**1. Ser demasiado general**

En la primera versión solamente solicité crear un programa para gestionar productos. Esto podía producir una respuesta poco específica.

¿Cómo lo evité?

En las siguientes versiones definí los atributos, las operaciones, el lenguaje de programación y las características que debía tener la aplicación.

**2. No indicar el formato de respuesta**

Un prompt sin formato puede generar respuestas desordenadas o presentar el código sin explicar su estructura.

¿Cómo lo evité?

En la versión final establecí cinco apartados para organizar la respuesta: descripción, estructura de clases, código, explicación y ejemplo de ejecución.

## Conclusiones

Durante el desarrollo de esta actividad comprendí que un prompt profesional no consiste solamente en realizar una pregunta a la inteligencia artificial, sino en proporcionar instrucciones claras, contexto y ejemplos que permitan obtener resultados más precisos.

Mediante las tres versiones pude observar cómo la incorporación progresiva de los componentes del prompt mejora la calidad y organización de las respuestas.

Finalmente, aprendí que la ingeniería de prompts es una herramienta útil para el desarrollo de software, ya que permite aprovechar la inteligencia artificial como apoyo en la programación y resolución de problemas.