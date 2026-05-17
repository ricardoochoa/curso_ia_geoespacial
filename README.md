# Inteligencia Artificial Generativa para Análisis Geoespacial y Urbano
## Introducción 
Aquí puedes encontrar las instrucciones y ejercicios resueltos del curso "Inteligencia Artificial Generativa para Análisis Geoespacial y Urbano"

## Ejercicio 1

### Paso 1: Preparación
A. Abre [https://colab.google.com](colab.google.com) en el navegador de tu preferencia y accede con tu cuenta de Gmail.
B. Da clic en “Nuevo cuaderno”

### Paso 2: Datos
C. Descarga los datos de la siguiente liga: [https://bit.ly/48Syq15](https://bit.ly/48Syq15)
D. Da clic en el ícono de la carpeta en la barra de la izquierda para desplegar el cajón de archivos. Arrastra y suelta tus datos en el cajón.

### Paso 3: Prompt
E. Da clic en el ícono azul en la parte inferior de la pantalla y escribe el siguiente prompt. 
>“Lee el archivo tijuana_mun_osm.geojson usando la librería GeoPandas y crea un mapa usando la variable estaciones_bus como color de relleno.”
Presiona ENTER o (INTRO). Lee la respuesta de Gemini y haz clic en “Aceptar y Ejecutar” (Accept & Run). 

### Paso 4: Iteración
F. ¿El resultado es el esperado? ¿Te gustaría modificar algo o algo falló en el proceso? Da continuidad a la conversación con Gemini. Por ejemplo, puedes pedir a Gemini que modifique la rampa de color:

> “Modifica la rampa de color a un gradiente que vaya del blanco al rojo.”

También puedes agregar un mapa base con la siguiente instrucción. 

> “Modifica el código para agregar un mapa base con estilo de CartoDB.Positron usando la librería contextily.”

Intenta lo siguiente: 

> “Tengo un archivo geojson que contiene una variable numérica llamada "estaciones_bus" que indica la distancia en metros a la estación de bus más cercana. Escribe un código para leer el archivo geojson e imprimir un mapa con las siguientes características: 
> 1. El mapa debe tener un mapa base en escala de grises, un título "Distancia a estaciones de bus (m)", 
> 2. El mapa debe mostrar la variable  "estaciones_bus" como color de relleno usando un gradiente de blanco a rojo.
> 3. El mapa debe tener una leyenda (simbología) de color en la esquina inferior izquierda. 
> Además de imprimir en pantalla, el código debe guardar la imagen en formato PNG a 300 dpi. 
> Utiliza las librerías geopandas, matplotlib y contextily verificando que estén instaladas.“

### Paso 5: Análisis
G. Aprovecha tu prompt y tu código para analizar y documentar tu análisis.  Aquí hay un ejemplo de análisis que combina mapa, gráficas y análisis numérico. 

## Ejercicio 2
## Paso 1: Preparación
A. Abre colab.google.com o si ya estás ahí, haz clic en “Nuevo cuaderno”

## Paso 2: Datos
B. [https://bit.ly/48Syq15](Descarga) y arrastra los datos igual que en el Ejercicio 1. 

## Paso 3: Prompt
C. Da clic en el ícono azul en la parte inferior de la pantalla y escribe el siguiente prompt. 
> Actúa como una científica de datos espaciales experta en Python. Voy a trabajar en Google Colab con un archivo llamado tijuana_mun_osm.geojson. Este archivo contiene una retícula hexagonal del área metropolitana de Tijuana con las siguientes columnas:
> estaciones_bus: Distancia en metros a la estación de bus más cercana 
> escuelas: Distancia en metros a la escuela más cercana 
> hospitales: Distancia en metros al hospital más cercano 
> oficinas_gobierno: Distancia en metros a la oficina de gobierno más cercana 
> clinicas: Distancia en metros a la clínica más cercana 
> empleo: Número de unidades económicas 
> uso_residencial: Zonas con uso de suelo residencial 
> uso_industrial: Zonas con uso de suelo industrial 
> Tu primera tarea: Escribe el código en Python usando la librería geopandas para cargar este archivo y mostrar las primeras 5 filas para verificar que se haya leído correctamente. Asegúrate de incluir cualquier comando de instalación (!pip install...) si consideras que es necesario en Colab.

## Paso 4: Iteración
D. Crear índice con un prompt simple: 

> Imprime un mapa que despliegue un índice de proximidad usando las variables hospitales, escuelas y estaciones_bus. El índice debe mostrar, al estilo de mapa de calor, aquellas zonas que están alejadas de escuelas, del transporte público y de oportunidades de empleo.

