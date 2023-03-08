# GitHub Pages y mkdocs

1. GitHub Pages
2. mkdocs
3. Enlaces
4. Anexo: instalación de mkdocs

```
Se supone realizadas las prácticas de uso de GitHub y Markdown.
```

## 1. GitHub Pages

```
GitHub nos da la posibilidad de publicar páginas HTML en el repositorio, por ejemplo la documentación del
código o del proyecto, etc.
Para ello
Crear repo test-demo-pages
Activar Pages en rama main usando la carpeta docs.
Clonar repositorio en local.
Crear directorio docs y añadir y editar fichero index.html con estilos.css.
Subir los cambios a GitHub y probar la URL que nos indica Pages que será similar a
http://<usuario>.github.io/<repositorio>
```

## 2. mkdocs

```
Pasos a dar:
Instalar mkdocs (requiere python3, pip, uso de venv).
Usando como guía Getting Started with MkDocs
Crear proyecto dentro de directorio clonado con mkdocs new misdocs
Lanzar mkdocs serve para ver cambios en vivo antes de subirlos a GitHub.
Añadir al menos dos ficheros en formato Markdown.
Modificar el fichero de configuración para que indexe los tres ficheros.
Probar a modificar el tema por defecto
Una vez terminado hacer mkdocs gh-deploy, esperar unos momentos y ver la página en GitHub
Pages. mkdocs activa Pages y crea una rama de nombre gh-pages donde sube el sitio web
generado.
```

## 3. Enlaces

```
GitHub Pages: https://docs.github.com/es/pages
Mkdocs: https://www.mkdocs.org/
```

## 4. Anexo: instalación de mkdocs

```
Debe tener instalado:
python
```

03 _pages_mkdocs.md 24 / 2 / 2023

```
/
python-venv
Creamos un entorno virtual en el repositorio:
$ python3 -m venv mivenv
Añadimos el entorno virtual al fichero .gitignore:
$ echo "mivenv" >> .gitignore
$ echo ".gitignore" >> .gitignore
Activamos el entorno virtual
$ source mivenv/bin/activate
(mivenv) $
Instalamos mkdocs con pip:
(mivenv) $ pip install mkdocs
...
(mivenv) $
Y ya podemos usar mkdocs:
(mivenv) $ mkdocs new misdocs
Al terminar:
(mivenv) $ deactivate
$
```

This is a offline tool, your data stays locally and is not send to any server!