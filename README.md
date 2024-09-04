Proyecto de Procesamiento de Texto

Este proyecto incluye varios scripts y comandos para procesar archivos de texto utilizando herramientas como AWK, C, y ANTLR. A continuación se detallan los comandos y pasos para ejecutar cada una de las partes del proyecto.
Requisitos Previos

Asegúrate de tener las siguientes herramientas instaladas:

    AWK
    GCC (Compilador de C)
    Java
    ANTLR (Descargable desde ANTLR website)

Instrucciones
1. Procesamiento de texto con AWK

Para ejecutar el script AWK, utiliza el siguiente comando:

    awk -f token.awk archivo.txt

Este comando ejecuta un script AWK (token.awk) sobre un archivo de texto (archivo.txt).

2. Ejecución de un archivo binario

Si tienes un archivo binario compilado (a.out), puedes ejecutarlo con el archivo de texto como entrada:

    ./a.out archivo.txt

3. Contar palabras en C

Primero, compila el archivo de C utilizando GCC:

    gcc contar_palabra.c -o contar_palabra

Luego, ejecuta el programa para contar la palabra "arroz" en el archivo de texto:

    ./contar_palabra archivo.txt arroz

5. Procesamiento de expresiones con ANTLR

Para procesar expresiones utilizando ANTLR, sigue los siguientes pasos:

Genera el lexer y parser desde el archivo Trig.g4:

    java -jar antlr-4.13.2-complete.jar -no-listener -visitor Trig.g4

Compila los archivos .java generados:

    javac -cp .:antlr-4.13.2-complete.jar *.java

Finalmente, ejecuta el analizador con un archivo de entrada (expr.in):

    java -cp .:antlr-4.13.2-complete.jar Test expr.in
