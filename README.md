# Laboratorio 4 - Grupo 1 - Frontend

### Instalar NPM
Ir a este enlace y seguir las instrucciones de acuerdo al Sistema Operativo:

https://nodejs.org/en/download/

Para validar que la ejecución fue exitosa se debe ejecutar el siguiente comando:

`npm -v`

### Instalar Newman

Ejecutar en un terminal el siguiente comando:

`npm install -g newman`

### Contenido del Repositorio

Los archivo que se encuentran en este repositorio son:

**LabFinalGrupo01.postman_collection.json** : Colección de Postman con 2 request.
- **DxC_ObtieneUF**: Obtiene la UF del dia y la guarda como variable global.
- **DxC**: Ejecuta la prueba del microservicio utilizando la UF obtenida en el request anterior.

**DataLabFinalGrupo01.csv** : Datos para las pruebas de Postman en formato CSV.
Para cada fila del CSV se ejecutan los request anteriores.


### Ejecutar Servidor Http

Desde la raiz de este repositorio ejecutar:

`newman run LabFinalGrupo01.postman_collection.json -d DataLabFinalGrupo01.csv`

Para que funcionen las pruebas debe estar levantado el microservicio en el puerto 8089.