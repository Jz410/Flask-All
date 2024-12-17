# Flask-All
templates de una web con flask con todo hecho desde login hasta registro y hashar contraseñas

## Carpetas Que Estaran Al Iniciar El Proyecto Son:
- config:
  -
- models:
  -
- routers:
  -
- static:
  - Aqui estaran los archivos multimedia y archivos de Css, Js u otra dependecias y Vas las carpetas usadas como:
    - Imagenes
    - Sonidos
    - Videos
    - Js
    - Css
     
- templates:
  - Estan todos los Html y el layout.html donde esta la configuracion de link de estilos estilos.css o codigo app.js solo cambiar filename='TuRuta/Imagen.png'
      - Esta Linea de codigo se usara para exportar archivos e imagnes u otro tipo de archivo
    ```bash
        {{ url_for('static', filename='rutaDeCarpeta/tuArchivo.Tipo')}}
     ```
      ### Ejemplos de uso:
    
      - Para importar el css 
    ```bash
        <link rel="stylesheet" href="{{ url_for('static', filename='Css/Style.css')}}">
     ```
      - Para importar Imagenes 
    ```bash
        <img src="{{ url_for('static', filename='Imagenes/Imagen.png')}}" alt="Imagen Png">
     ```
- .gitingnore:
  - Esta configurado para que no se suba archivos basuras de tu pc o del desarrollo al repositorio, mas si estas usando un entorno virtual.
- requeriments.txt:
  - Este archivo se llamara al iniciar el proyecto si no tienes las dependecias descargadas o estas en un entorno virtual nuevo.
     ```bash
        pip install requeriments.txt
     ```
    se te descargaran todas las dependecias con la version espesificada en el requeriement.txt modificar la version si quieres usar una espesificamente.
     
- Main.py:
  - Archivo Principal donde se ejecutara para poder iniciar la web en Modo desarrollo o Modo Produccion
