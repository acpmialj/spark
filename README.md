# Spark
Clonar este repositorio, y hacer "cd spark". En ese directorio estarán almacenados los cuadernos Jupyter. 

Lanzar un contenedor con:

```sh
docker run --rm -it \
    --name spark \
    -p 4040:4040 \
    -p 50070:50070 \
    -p 8088:8088 \
    -p 8888:8888 \
    -v "$PWD":/workspace \
    jdvelasq/spark:3.1.3 
```
    
Nota: la descarga puede ser bastante larga, es una imagen de varios GB. Incluye Hadoop Core, Spark, PySpark, Jupyter. 

La creación del contenedor termina lanzando una instancia de Jupyter Lab. Abrir el el navegador del anfitrión el URL que empieza por http://127.0.0.1:8888

Hecho esto, desde Jupyter Lab podremos ver y ejecutar los cuadernos. Seguir las instrucciones que se dan en ellos. 


