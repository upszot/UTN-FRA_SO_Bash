# Guía Basica de Bash Scripting en Linux

## Introducción
Bash (Bourne Again SHell) es el intérprete de comandos predeterminado en muchas distribuciones de Linux. Permite a los usuarios automatizar tareas, manipular archivos y crear scripts para simplificar procesos complejos.


### Ejecución de Comandos
- Puedes ejecutar comandos directamente desde la línea de comandos.
  - Ejemplo: Para listar archivos en un directorio, usa `ls`.
- o Agrupar un conjunto de comandos en un archivo y luego ejecutar el mismo.
  - Ejemplo: [Como crear y ejecutar un script](./Primeros_Pasos/primeros_pasos.md)

### **Ejemplos de Bash Script Básicos**
- [ ] Variables
  - Declarar y asignar valores a variables
  - Usar variables en scripts Bash
- [ ] **Parámetros**
  - Recibir parámetros desde la línea de comandos:
    - Obtener parámetros individuales: `$1`, `$2`, etc.
    - Pedir datos al usuario con `read`
- [ ] **Manejo de parámetros y variables de entorno:**
  - `$0`: nombre del script
  - `$#`: número total de parámetros pasados al script
  - `$n`: acceso a parámetros específicos (con `n` de 1 a 9)
  - `$$`: PID del proceso actual
  - `$*`: todos los parámetros como una cadena
  - `$@`: todos los parámetros como lista
  - `$?`: código de salida del último comando
  - `$!`: PID del último proceso ejecutado en segundo plano
  - `$_`: último argumento del último comando ejecutado

  > Aca puede ver un [Ejemplo de Variables y parametros](./variables_parametros/variables_parametros.sh)

- [ ] **Bucles**
  - Bucle `for`:
    - [Iteración sobre listas: ](./Bucle_for/1_for_lista.sh) `for valor in 1 2 3`
    - [Iteración con comandos:](./Bucle_for/2_for_cmd_lista.sh) `for linea in $(cat archivo)`
  - Bucle `while`:
    - [Repetición basada en condiciones simples](./Bucle_while/1_while_simple.sh)
    - [Repetición basada en comandos:](./Bucle_while/2_while_cmd_lista.sh) `while read linea; do ... done < archivo`    
- [ ] **Condicionales**
  - [condiciones simples y Condicional anidado:](./Condicionales/if_simple.sh) `if`,  `if-elif-else`
  - [Condicionales múltiples:](./Condicionales/if_multiple.sh) `if [[ condición1 && condición2 ]]; then`
  - [para múltiples opciones:](./Condicionales/case_example.sh) `case`
- [ ] **Menús y Argumentos**
  - [creación de menús interactivos:](./menu/select_menu.sh) `select`
  - [manejo de argumentos de línea de comandos:](./menu/getopts.sh) `getopts` y `OPTARG`


### **Ejemplos de Bash Script Avanzados**
- [ ] [**Variables avanzadas**](./bash_avanzado/vectores_matrices.sh)
  - Vectores (Arrays) para listas
  - Matrices para estructuras más complejas
- [ ] [**Funciones**](./bash_avanzado/funciones.sh)
  - Definir y usar funciones
  - Pasar parámetros a funciones
- [ ] [**Entrada/Salida**](./bash_avanzado/entradas_salidas.sh)
  - Redireccionamiento de entrada y salida (`>`, `>>`, `<`, `|`)
  - Tubos (`|`): conexión de comandos
  - Control de errores y códigos de salida
- [ ] **Operadores**
  - Operadores aritméticos (+, -, *, /, %, etc.)
  - Operadores lógicos (`&&`, `||`)
  - Comparaciones numéricas y de cadenas
  

## Extras
- [Manual de bash-scripting](https://github.com/upszot/UTN-FRA_SO_onBording/tree/master/Extras)

