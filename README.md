![header](https://github.com/OSWeekends/agile-project-template/raw/master/other/img/OSW-project-GitHub-template-header.jpg)

# eventpoints-backend

## Scraper

Este es un scraper   y ha sido desarrollado con la  libreria Scrapy,de Python.

#### Instalación
Requerimientos Minimos:
Para  instalar y ejecutar este projecto necesitas

Python Versión 3.6
Pip Versión 18.1

Instrucciones: 
Crear venv con el comando
 
`python3 -m venv ./venv`

necesitamos instalar las  dependencias despues con e comando 

`pip3 install -r requirements.txt`

Si usas Python 3.7, da un error que se puede solucionar ejecutando el comando

`pip3 install git+https://github.com/twisted/twisted.git@trunk`

#### Uso

[Scrapy Docs](https://doc.scrapy.org/en/latest/)

##### Lanzamiento de spiders

`scrapy crawl {spider_name} -o {json_path}`

Siendo `spider_name` el nombre de la araña y `json_path` el JSON en el que se va a
volcar el scrapeo. 
Scrapy escribe al final del fichero por lo que en sucesivas
ejecuciones habría que borrar el JSON si ya existe.

Ejemplo de uso

`scrapy crawl meetup -o output/meetup.json`

## API

El api está en el directorio `api`

Para instalar las dependencias del API nos metemos en su directorio y ejecutamos: `npm install`

Documentación de la API en swagger: http://localhost:3000/api/v1/spec

Para ejecutar el API: `npm start`
Una vez lanzado la vemos en --> http://localhost:3000/api/v1/events

`#eventpoints_new` en Slack

![footer](https://github.com/OSWeekends/agile-project-template/raw/master/other/img/OSW-project-GitHub-template-footer.jpg)
