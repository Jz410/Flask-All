# Flask-All
Plantillas de una web desarrollada con Flask, que incluye la funcionalidad completa desde el inicio de sesión hasta el registro de usuarios, con el hash de contraseñas implementado.

## Carpetas que estarán disponibles al iniciar el proyecto:
- config:
  -
- models:
  -
- routers:
  -
- static:
  - Aquí se encontrarán los archivos multimedia, así como los archivos de CSS, JavaScript y otras dependencias. Además, se detallarán las carpetas utilizadas, tales como:
    - Imagenes
    - Sonidos
    - Videos
    - Js
    - Css
     
- templates:
  - Se incluyen todos los archivos HTML, así como el archivo layout.html, donde se encuentra la configuración de los enlaces a los estilos <strong> (styles.css) </strong> y el código de <strong>(app.js)</strong>. Solo es necesario modificar filename='TuRuta/Imagen.png' según corresponda.
      - Esta línea de código se utilizará para exportar archivos, imágenes u otros tipos de archivos
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
