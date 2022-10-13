##  PySpark con Google Colab.

Este artículo lo redacte hace un tiempo debido a la complejidad de pasos previos que deben hacerse para poder
trabajar con PySpark en local.

Con estos sencillos pasos que te muestro aqui, podras instalar los paquetes y comandos necesarios para practicar
PySpark desde tu notebook de Google Colab.

Aqui te explico la instalación:

- 1º Antes de nada, necesitamos instalar una máquina virtual Java (JVM) para funcionar.
- 2º A continuación, instalaremos Apache Spark 3.2.1 con Hadoop 3.2 desde aquí --> https://spark.apache.org/downloads.html
- 3º Instalamos la libreria findspark --> ! pip install findspark
- 4º Establecemos la ruta del entorno virtual. Para ello usamos la libreria OS que permite manipular la estructura de directorios.
- 5º Localizmos Spark en el sistema. Importamos findspark y utilizamos el método findspark.init(). 
     Deberia devolver esto --> '/content/spark-3.2.1-bin-hadoop3.2'
- 6º Importamos SparkSession de pyspark.sql y creamos una SparkSession, que es el punto de entrada a Spark.

     Si todo esta correcto, al cargar Spark en memoria deberiamos obtener algo asi: 
     Version --> v3.2.1
     Masterlocal --> [*]
     AppNamepyspark --> -shell

Una vez tenemos esto podemos cargar el dataset que queramos y practicar con los comandos clásicos de PySpark en nuestro Notebook.

En este ejercicio hemos utilizado un dataset de ventas al por menor, en el que el objetivo es crear un modelo para predecir
las ventas de ciertos productos y ayudar a crear ofertas personalizadas para los clientes.

Espero que les sea de ayuda.

Un saludo.
Juanjo.
