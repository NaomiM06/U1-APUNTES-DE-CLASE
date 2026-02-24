# Unidad I. Introducción a la graficación por computadora
--------------------
# 1.1 Historia y evolución de la graficación por computadora

La graficación por computadora es el área de la informática encargada de generar, manipular y representar imágenes mediante el uso de algoritmos y hardware especializado. Su desarrollo ha estado ligado al avance de la computación y la electrónica.

Los primeros antecedentes se remontan a la década de 1950, cuando los sistemas informáticos comenzaron a utilizar pantallas para mostrar información gráfica básica. Un hito fundamental fue el sistema Sketchpad, desarrollado en 1963 por Ivan Sutherland, considerado el padre de la computación gráfica. Este sistema permitió dibujar directamente en la pantalla mediante un lápiz óptico, introduciendo conceptos como la interacción gráfica y la representación de objetos.

Durante las décadas de 1970 y 1980, la graficación evolucionó con la aparición de gráficos rasterizados y los primeros sistemas de diseño asistido por computadora (CAD). En este periodo se desarrollaron algoritmos fundamentales para el trazo de líneas, eliminación de superficies ocultas y modelado tridimensional.

En los años 90, con el aumento de la potencia de procesamiento y el desarrollo de tarjetas gráficas (GPU), la graficación en 3D se volvió más realista y accesible, impulsando industrias como los videojuegos y la animación digital.

Actualmente, la graficación por computadora incluye técnicas avanzadas como renderizado en tiempo real, simulación física, realidad virtual y gráficos generados mediante inteligencia artificial, consolidándose como un campo multidisciplinario clave en la tecnología moderna.

-----------
# 1.2 Áreas de aplicación

La graficación por computadora tiene un amplio campo de aplicación en diversas disciplinas:

Diseño asistido por computadora (CAD): utilizado en ingeniería y arquitectura para crear planos y modelos tridimensionales.

Animación y entretenimiento: cine, videojuegos y efectos visuales.

Visualización científica: representación de datos complejos en áreas como medicina, meteorología y física.

Simulación: entrenamiento en aviación, medicina y procesos industriales.

Interfaces gráficas de usuario (GUI): diseño de sistemas interactivos.

Realidad virtual y aumentada: entornos inmersivos para educación y entretenimiento.

Publicidad y diseño digital: creación de contenido visual y multimedia.

Estas aplicaciones demuestran que la graficación no solo es una herramienta estética, sino también un medio para analizar, comprender y comunicar información.

------------------------------
# 1.3 Aspectos matemáticos de la graficación

La base de la graficación por computadora se encuentra en las matemáticas, principalmente en:

Geometría analítica

Permite representar objetos mediante coordenadas en el plano (2D) o en el espacio (3D). Los puntos se describen con pares o ternas (x, y, z).

Álgebra lineal

Es fundamental para realizar transformaciones geométricas como:

Traslación

Rotación

Escalamiento

Proyección

Estas operaciones se realizan mediante matrices y vectores, lo que permite manipular objetos de forma eficiente.

Cálculo

Se utiliza para modelar curvas y superficies, así como para cálculos de iluminación y sombreado.

Interpolación

Permite generar valores intermedios entre puntos, esencial en animaciones y suavizado de gráficos.

Gracias a estos fundamentos, es posible construir escenas complejas con precisión y realismo.

----------------------------------
# 1.4 Modelos del color: RGB, CMY, HSV y HSL

Los modelos de color son sistemas matemáticos que describen cómo representar colores digitalmente.

RGB (Red, Green, Blue)

Es un modelo aditivo basado en la mezcla de luz. Se utiliza en pantallas y dispositivos electrónicos.
Cada color se obtiene combinando intensidades de rojo, verde y azul.

CMY (Cyan, Magenta, Yellow)

Modelo sustractivo utilizado en impresión. Los colores se generan absorbiendo ciertas longitudes de onda de la luz.

HSV (Hue, Saturation, Value)

Representa el color en términos más cercanos a la percepción humana:

Matiz (Hue): tipo de color

Saturación: intensidad

Valor: brillo

HSL (Hue, Saturation, Lightness)

Similar a HSV, pero la luminosidad se calcula de forma distinta, permitiendo un control más intuitivo en diseño digital.

Tutorial básico: iluminación de un cubo en Blender

(Software desarrollado por la organización Blender Foundation)

Abrir Blender y eliminar el objeto inicial si es necesario.

Añadir un cubo: menú Add → Mesh → Cube.

Insertar una fuente de luz: Add → Light → Point o Sun.

Posicionar la luz para que ilumine una cara del cubo.

Ajustar la intensidad en el panel de propiedades de la luz.

Asignar un material al cubo:

Seleccionar el cubo

Ir a Material Properties

Cambiar el color base

Activar la vista renderizada para observar sombras y reflejos.

Con estos pasos se puede comprender cómo la posición de la luz, la intensidad y el material influyen en la percepción de volumen.

----------------------------------
# 1.5 Representación y trazo de líneas y polígonos

La representación de primitivas gráficas es la base de cualquier sistema de graficación.


# Líneas

Las líneas se generan a partir de dos puntos en el plano.
Existen algoritmos específicos para dibujarlas de manera eficiente, como:

- Algoritmo de DDA (Digital Differential Analyzer)

- Algoritmo de Bresenham

Estos métodos determinan qué píxeles deben activarse para aproximar la línea con precisión.

# Polígonos

Un polígono es una figura formada por un conjunto de vértices conectados.
Son fundamentales porque la mayoría de los objetos 3D se construyen mediante mallas poligonales.

Procesos importantes:

- Relleno de polígonos

- Determinación de superficies visibles

- Suavizado de bordes

- La correcta representación de polígonos permite construir modelos complejos y realistas en gráficos tridimensionales.
-----
# 1.5.1
# FLOR DE VIDA
<img width="1782" height="679" alt="image" src="https://github.com/user-attachments/assets/b206e6a4-0dcf-4462-ae3c-8dda3b9ce93f" />

# POLÍGONO
<img width="1713" height="788" alt="image" src="https://github.com/user-attachments/assets/c6bcc5d3-b213-4b87-b4fa-660b60bcbb22" />

----------
# 1.6 Procesamiento de mapas de bits

El procesamiento de mapas de bits se refiere al conjunto de técnicas utilizadas para manipular imágenes digitales formadas por píxeles. Un mapa de bits (bitmap) es una representación matricial donde cada posición almacena información de color o intensidad.

Este tipo de imágenes es fundamental en la graficación por computadora, ya que la mayoría de los dispositivos de visualización, como monitores y pantallas, trabajan con gráficos rasterizados.

# Concepto de mapa de bits

Un mapa de bits es una estructura de datos compuesta por una cuadrícula de píxeles organizados en filas y columnas. Cada píxel contiene información de color, generalmente codificada en formatos como RGB o escala de grises.

Las características principales de una imagen bitmap son:

- Resolución: cantidad de píxeles que forman la imagen.

- Profundidad de color: número de bits usados para representar el color.

- Tamaño de archivo: depende de la resolución y la profundidad de color.

# Operaciones básicas sobre mapas de bits
1. Adquisición de imágenes

Consiste en obtener imágenes mediante escáneres, cámaras digitales o capturas de pantalla.

2. Mejora de imágenes

Busca optimizar la calidad visual mediante técnicas como:

- Ajuste de brillo y contraste

- Corrección de color

- Filtrado de ruido

3. Transformaciones geométricas

Permiten modificar la forma o tamaño de la imagen:

- Escalado

- Rotación

- Traslación

- Recorte

Estas transformaciones se realizan mediante interpolación para mantener la calidad.

4. Filtrado digital

Se utilizan filtros para modificar características específicas de la imagen:

- Filtros suavizantes: reducen ruido

- Filtros de realce: resaltan bordes

- Filtros de detección de bordes

5. Compresión de imágenes

Reduce el tamaño del archivo para facilitar almacenamiento y transmisión.
Puede ser:

- Con pérdida (ejemplo: JPEG)

- Sin pérdida (ejemplo: PNG)

Aplicaciones del procesamiento de mapas de bits

El procesamiento de imágenes rasterizadas se utiliza en:

- Edición y diseño gráfico

- Fotografía digital

- Medicina (imágenes médicas)

- Reconocimiento de patrones

- Sistemas de visión artificial

- Multimedia y videojuegos

# Ventajas y desventajas

Ventajas:

- Representación precisa de detalles y colores

- Compatibilidad con la mayoría de dispositivos

- Adecuado para imágenes complejas

Desventajas:

- Archivos grandes en alta resolución

- Pérdida de calidad al escalar

- Dependencia de la resolución
-----------------------
# Bibliografía
1. Foley, J. D., van Dam, A., Feiner, S. K., & Hughes, J. F. (2014). Computer graphics: Principles and practice (3rd ed.). Addison-Wesley.

2. Hearn, D., & Baker, M. P. (2011). Computer graphics with OpenGL (4th ed.). Pearson.
   
3. Gonzalez, R. C., & Woods, R. E. (2018). Digital image processing (4th ed.). Pearson.

4. Angel, E., & Shreiner, D. (2015). Interactive computer graphics: A top-down approach with WebGL (7th ed.). Addison-Wesley.

5. Blender Foundation. (2024). Blender documentation. https://docs.blender.org
