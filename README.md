# spark
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
    
Nota: la descarga es larga, es un contenedor de varios GB. Incluye Hadoop Core, Spark, PySpark, Jupyter. Lanza una instancia de Jupyter Lab. 
