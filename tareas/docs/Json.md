# JSON

1. Introducción
2. Enlaces

## 1. Introducción

```
Este bloque es parte del temario de 2º curso. Se hace pequeña introducción y poco más.
El ejemplo de uso más habitual de JSON es en el uso de APIS web. Estas APIS ofrecen su servicios en
formato JSON o XML. Desde diferentes lenguajes de programación puede lanzar peticiones a estas APIs y
procesar el resultado.
Observe un ejemplo muy sencillo de uso una API (ficticia)
https://jsonplaceholder.typicode.com/users/
https://jsonplaceholder.typicode.com/todos/
https://jsonplaceholder.typicode.com/users/
O esta otra relacionada con "Stars Wars":
https://swapi.dev/api/people/1/?format=json
https://swapi.dev/api/films/3/?format=json
Puede invocar desde CLI con el comando curl. En la primera API:
clases@lg:~$ curl https://jsonplaceholder.typicode.com/todos/
{
"userId": 1,
"id": 1,
"title": "delectus aut autem",
"completed": false
}clases@lg:~$
O sobre la segunda API donde:
hay que especificar el formato de salida (?format=json).
procesamos la salida para hacerla más legible con json_pp.
clases@lg:~$ curl -s https://swapi.dev/api/people/2/?format=json | json_pp
{
"birth_year" : "112BBY",
"created" : "2014-12-10T15:10:51.357000Z",
"edited" : "2014-12-20T21:17:50.309000Z",
"eye_color" : "yellow",
"films" : [
"https://swapi.dev/api/films/1/",
```

05_JSON.md 6/3/

```
/
"https://swapi.dev/api/films/2/",
"https://swapi.dev/api/films/3/",
"https://swapi.dev/api/films/4/",
"https://swapi.dev/api/films/5/",
"https://swapi.dev/api/films/6/"
],
"gender" : "n/a",
"hair_color" : "n/a",
"height" : "167",
"homeworld" : "https://swapi.dev/api/planets/1/",
"mass" : "75",
"name" : "C-3PO",
....
}
clases@lg:~$
```

## 2. Enlaces

```
JSON: http://www.json.org/json-es.html
Wikipedia: https://es.wikipedia.org/wiki/JSON
Tutoriales:
W3Schools JSON: https://www.w3schools.com/js/js_json_intro.asp
JSON tutorial: https://beginnersbook.com/2015/04/json-tutorial/
The Star Wars API: https://swapi.dev/
```

