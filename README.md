# Simpletron

Este proyecto consiste en el desarrollo de un simulador de la computadora **Simpletron** utilizando lenguaje C.

El programa permite cargar y ejecutar instrucciones escritas en **SML (Simpletron Machine Language)**, utilizando una memoria de 100 posiciones y diferentes registros para realizar el ciclo de búsqueda, decodificación y ejecución de instrucciones.

## Funcionalidades

El simulador cuenta con:

- Memoria de 100 posiciones.
- Captura de instrucciones SML desde el teclado.
- Uso del valor `9999` como centinela para finalizar la carga.
- Validación de los valores ingresados.
- Manejo del acumulador y registros de ejecución.
- Ejecución de las doce operaciones SML.
- Operaciones de entrada y salida.
- Operaciones de carga y almacenamiento.
- Operaciones aritméticas.
- Transferencias de control.
- Detección de errores durante la ejecución.
- Vaciado de registros y memoria.

## Compilación

Para compilar el programa utilizando GCC:

## Ejecución

Una vez compilado el programa, se ejecuta desde la terminal:

Al iniciar, el programa solicita ingresar las instrucciones del programa en lenguaje SML.

Cada instrucción se almacena en una posición de la memoria. Para finalizar la captura se debe ingresar el valor:

```text
9999
```

Después de recibir el valor centinela, Simpletron inicia la ejecución de las instrucciones almacenadas.

Durante la ejecución se realiza el ciclo de:

1. Búsqueda de la instrucción.
2. Decodificación del código de operación y operando.
3. Ejecución de la operación correspondiente.
4. Actualización del contador de instrucciones.

Al finalizar la ejecución, el programa muestra los registros y el contenido de la memoria.

## Manejo de errores

El simulador contempla la detección de errores como:

- División entre cero.
- Código de operación inválido.
- Desbordamiento del acumulador.
- Valores o estados inválidos durante la ejecución.

En caso de detectar un error fatal, el programa informa el problema y muestra el estado de los registros y la memoria.

## Pruebas

Se realizaron pruebas de ejecución para comprobar el funcionamiento del simulador y de las instrucciones SML.

La evidencia de las pruebas realizadas se encuentra en el archivo:

`Corrida Simpletron.pdf`

## Archivos del repositorio

- `Simpletron.c` - Código fuente del simulador.
- `Corrida Simpletron.pdf` - Evidencia de ejecución y pruebas.
- `README.md` - Documentación del proyecto.

## Autor

Maria Fernanda Cabrera
