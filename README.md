# Cajero API
Este es el backend del ejercicio del Cajero. Esta construido sobre la base de __FastAPI__, un framework bastante sencillo para esta labor. 
Este proyecto está diseñado para correr específicamente en Heroku. Para ello, es importante que usted ajuste en el archivo `main.py` el arreglo de `origins` válidos para __CORS__. En particular, debe agregar el nombre de la app en `Heroku` asociada al front-end del cajero, en este ejemplo está al app de `Heroku` del autor del presente repositorio. 

## Requerimientos
Recuerde que para la ejecución de esta API, debe crear un entorno virtual e instalar los requerimientos necesarias.

En Linux:
```
python -m venv env
source env/bin/activate
pip install -r requirements.txt
```

En Windows:
```
python -m venv env
env\Scripts\activate
pip install -r requirements.txt
```

## Ejecución
Una vez haya hecho esto, ya está disponible el servicio de API para ejecutarse. Para ello, debe ejecutar la siguiente instrucción:
```
uvicorn main:api --reload
```