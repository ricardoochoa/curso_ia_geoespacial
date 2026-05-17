# Inteligencia Artificial Generativa para Análisis Geoespacial y Urbano
## Introducción 
Aquí puedes encontrar las instrucciones y ejercicios resueltos del curso "Inteligencia Artificial Generativa para Análisis Geoespacial y Urbano"

## Ejercicio 1. 

### Paso 1: Preparación
A. Abre colab.google.com en el navegador de tu preferencia y accede con tu cuenta de Gmail.
B. Da clic en “Nuevo cuaderno”

### Paso 2: Datos
C. Da clic en el ícono de la carpeta en la barra de la izquierda para desplegar el cajón de archivos. 
D. Arrastra y suelta tus datos en el cajón.

### Paso 3: Prompt
E. Da clic en el ícono azul en la parte inferior de la pantalla y escribe el siguiente prompt. Presiona ENTER o (INTRO). Lee la respuesta de Gemini y haz clic en “Aceptar y Ejecutar” (Accept & Run). 
>“Lee el archivo tijuana_mun_osm.geojson usando la librería GeoPandas y crea un mapa usando la variable estaciones_bus como color de relleno.”

### Paso 4: Iteración
F. ¿El resultado es el esperado? ¿Te gustaría modificar algo o algo falló en el proceso? Da continuidad a la conversación con Gemini. 

> “Modifica la rampa de color a un gradiente que vaya del blanco al rojo.”

> “Modifica el código para agregar un mapa base con estilo de CartoDB.Positron usando la librería contextily.”

Intenta lo siguiente: 

> “Tengo un archivo geojson que contiene una variable numérica llamada "estaciones_bus" que indica la distancia en metros a la estación de bus más cercana. Escribe un código para leer el archivo geojson e imprimir un mapa con las siguientes características: 
1. El mapa debe tener un mapa base en escala de grises, un título "Distancia a estaciones de bus (m)", 
2. El mapa debe mostrar la variable  "estaciones_bus" como color de relleno usando un gradiente de blanco a rojo.
3. El mapa debe tener una leyenda (simbología) de color en la esquina inferior izquierda. 
Además de imprimir en pantalla, el código debe guardar la imagen en formato PNG a 300 dpi. 
Utiliza las librerías geopandas, matplotlib y contextily verificando que estén instaladas.“

### Paso 5: Análisis
G. Aprovecha tu prompt y tu código para analizar y documentar tu análisis.  Aquí hay un ejemplo de análisis que combina mapa, gráficas y análisis numérico. 
