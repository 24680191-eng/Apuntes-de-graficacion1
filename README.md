# Apuntes-de-graficacion1
1. Introducción a la Graficación por Computadora

La graficación por computadora es una disciplina de la informática dedicada al estudio de los métodos y técnicas para generar, manipular y representar imágenes digitales mediante algoritmos matemáticos y sistemas computacionales. Esta área integra conocimientos de matemáticas, física, programación y diseño visual para producir imágenes bidimensionales (2D) y tridimensionales (3D).

A diferencia del dibujo tradicional, donde la representación gráfica depende de herramientas físicas, en la graficación por computadora la imagen se construye mediante estructuras de datos, cálculos matemáticos y procesamiento digital. Cada objeto, textura, color y efecto visual es el resultado de operaciones matemáticas realizadas por la unidad de procesamiento gráfico (GPU).

En la actualidad, la graficación por computadora es esencial en múltiples industrias como el entretenimiento digital, la ingeniería, la arquitectura, la medicina, la publicidad y la simulación científica. Programas como Blender permiten aplicar estos fundamentos teóricos de manera práctica, ofreciendo herramientas de modelado, animación, iluminación, texturizado y renderizado.

La importancia de esta disciplina radica en su capacidad para transformar datos numéricos en representaciones visuales comprensibles, facilitando tanto la comunicación visual como la simulación de fenómenos reales.

1.1 Historia y Evolución de la Graficación por Computadora

La historia de la graficación por computadora se remonta a la década de 1950, cuando las primeras computadoras comenzaron a representar imágenes simples utilizando tubos de rayos catódicos. En sus inicios, los gráficos eran vectoriales y consistían únicamente en líneas monocromáticas.

Durante los años 60 se desarrollaron sistemas interactivos pioneros como Sketchpad, considerado uno de los primeros programas de diseño asistido por computadora (CAD). Este avance permitió la manipulación directa de objetos gráficos mediante dispositivos apuntadores.

En la década de 1970 surgieron los primeros algoritmos fundamentales para el trazado de líneas y polígonos, como el algoritmo de Bresenham, que permitió dibujar líneas de manera eficiente en pantallas rasterizadas.

En los años 80 y 90, el desarrollo de hardware especializado (tarjetas gráficas) impulsó la creación de gráficos tridimensionales en tiempo real. Aparecieron técnicas como:

Renderizado por sombreado (Shading).

Modelos de iluminación como Phong y Gouraud.

Transformaciones matriciales 3D.

Sistemas CAD avanzados.

Con el avance de las GPU en los años 2000, se implementaron técnicas más complejas como:

Ray tracing.

Iluminación global.

Sombras suaves.

Reflexión y refracción realista.

Actualmente, motores de render como Cycles en Blender utilizan trazado de rayos basado en principios físicos para simular el comportamiento real de la luz, generando imágenes fotorrealistas.

La evolución ha sido constante, pasando de gráficos simples de líneas a simulaciones tridimensionales complejas con iluminación físicamente correcta.

# 1.2 Áreas de Aplicación

La graficación por computadora tiene aplicaciones en numerosos campos:

Industria del Entretenimiento

Videojuegos con gráficos 3D interactivos.

Animaciones y efectos visuales en cine.

Producción de contenido digital.

Arquitectura y Diseño

Visualización arquitectónica.

Recorridos virtuales.

Simulación de iluminación natural.

Ingeniería

Modelado de piezas mecánicas.

Simulación estructural.

Diseño industrial.

Medicina

Reconstrucción tridimensional de órganos.

Simulación de procedimientos quirúrgicos.

Visualización de estudios médicos.

Educación y Simulación

Simuladores de vuelo.

Entornos virtuales interactivos.

Representaciones científicas.

En Blender, estas aplicaciones pueden desarrollarse mediante modelado poligonal, escultura digital, simulaciones físicas y animación avanzada.

# 1.3 Aspectos Matemáticos de la Graficación

La base de la graficación por computadora es matemática. Los conceptos fundamentales incluyen:

1.3.1 Sistemas de Coordenadas

En el espacio 3D se utilizan tres ejes:

X (horizontal)

Y (profundidad)

Z (vertical)

Cada objeto en Blender posee coordenadas que determinan su posición en el espacio tridimensional.

1.3.2 Vectores

Un vector representa dirección y magnitud. En gráficos 3D se utilizan vectores para:

Dirección de la luz.

Movimiento de objetos.

Cálculo de normales.

Las normales son vectores perpendiculares a las superficies que determinan cómo incide la luz.

1.3.3 Matrices y Transformaciones

Las transformaciones geométricas se realizan mediante matrices:

Traslación.

Rotación.

Escalado.

En Blender, cuando se mueve o rota un objeto, internamente se aplican multiplicaciones matriciales.

1.3.4 Modelos de Iluminación

El comportamiento de la luz se calcula mediante ecuaciones que consideran:

Intensidad.

Dirección.

Tipo de material.

Reflexión difusa.

Reflexión especular.

El motor Cycles implementa trazado de rayos (Ray Tracing), simulando físicamente el recorrido de la luz.

# 1.4 Modelos del Color: RGB, CMY, HSV y HSL

El color digital se representa matemáticamente mediante modelos.

RGB (Red, Green, Blue)

Modelo aditivo basado en la combinación de luz roja, verde y azul.
Cada componente varía generalmente entre 0 y 255.

En Blender, los materiales y luces utilizan este modelo.

CMY / CMYK

Modelo sustractivo usado en impresión.
Se basa en la absorción de luz mediante pigmentos.

HSV (Hue, Saturation, Value)

Representa el color en términos más intuitivos:

Hue: tono.

Saturation: intensidad.

Value: brillo.

HSL (Hue, Saturation, Lightness)

Similar al HSV, pero con una representación distinta del brillo.

En Blender, el selector de color permite cambiar entre estos modelos para facilitar la creación de materiales.

1.5 Representación y Trazo de Líneas y Polígonos

Las imágenes digitales pueden representarse mediante:

Gráficos Vectoriales

Formados por líneas matemáticas.

Gráficos Rasterizados

Compuestos por píxeles organizados en una cuadrícula.

En modelado 3D, los objetos están compuestos por mallas (meshes), formadas por:

Vértices.

Aristas.

Caras.

Las caras suelen ser triángulos o cuadriláteros.
El conjunto de estas caras forma la superficie del objeto.

La correcta topología de una malla es fundamental para:

Animación adecuada.

Deformaciones correctas.

Renderizado eficiente.

1.6 Formatos de Imagen

Los formatos de imagen almacenan datos visuales de distintas maneras.

PNG

Compresión sin pérdida y soporte de transparencia.

JPEG

Compresión con pérdida, ideal para fotografía.

TIFF

Alta calidad para impresión profesional.

EXR

Formato HDR utilizado en renderizado avanzado.

En Blender, la elección del formato depende del propósito del proyecto.

1.7 Procesamiento de Mapas de Bits

Un mapa de bits es una matriz de píxeles donde cada píxel contiene información de color.

El procesamiento de mapas de bits incluye:

Ajuste de contraste.

Corrección de color.

Aplicación de filtros.

Uso como textura.

En Blender, los mapas de bits pueden utilizarse como:

Texturas de color.

Mapas normales.

Mapas de desplazamiento.

Mapas de rugosidad.

Estos mapas permiten añadir detalle sin aumentar la complejidad geométrica del modelo.

Conclusión General

La graficación por computadora es una disciplina que combina matemáticas, programación y diseño visual para generar representaciones digitales.

El uso de Blender permite aplicar estos fundamentos mediante:

Modelado 3D.

Texturizado.

Iluminación.

Animación.

Renderizado avanzado.

Comprender los aspectos históricos, matemáticos y técnicos de la graficación permite desarrollar proyectos más eficientes, optimizados y visualmente realistas.

# 1.4. Modelos del color: RBG, CMY, HSV y HSL.
# MODELOS DEL COLOR: RGB, CMY, HSV y HSL
------------------------------------------------------------

# 1. MODELO RGB (Red, Green, Blue)
------------------------------------------------------------

El modelo RGB es un modelo de color basado en la mezcla de luz. Se utiliza principalmente en dispositivos electrónicos que emiten luz, como pantallas, televisores y proyectores.

RGB significa:
R = Red (Rojo)
G = Green (Verde)
B = Blue (Azul)

Es un modelo aditivo, lo que significa que los colores se forman sumando luz.

Mezclas principales:
Rojo + Verde = Amarillo
Rojo + Azul = Magenta
Verde + Azul = Cian
Rojo + Verde + Azul (máxima intensidad) = Blanco
Ausencia de los tres colores = Negro

Cada color se representa con valores entre 0 y 255.

Ejemplos:
RGB(255, 0, 0) = Rojo
RGB(0, 255, 0) = Verde
RGB(0, 0, 255) = Azul
RGB(255, 255, 255) = Blanco
RGB(0, 0, 0) = Negro

Se utiliza en:
Pantallas digitales
Diseño web
Programación gráfica
Videojuegos

------------------------------------------------------------

# 2. MODELO CMY (Cyan, Magenta, Yellow)
------------------------------------------------------------

El modelo CMY es un modelo sustractivo utilizado principalmente en impresión.

CMY significa:
C = Cyan (Cian)
M = Magenta
Y = Yellow (Amarillo)

Es sustractivo porque trabaja con pigmentos que absorben luz.

Cian absorbe rojo.
Magenta absorbe verde.
Amarillo absorbe azul.

Mezclas principales:
Cian + Magenta = Azul
Magenta + Amarillo = Rojo
Amarillo + Cian = Verde
Cian + Magenta + Amarillo = Negro (teóricamente)

En la práctica se agrega negro (K), formando el modelo CMYK, para mejorar la calidad en impresión.

Se utiliza en:
Impresoras
Diseño editorial
Artes gráficas

------------------------------------------------------------

# 3. MODELO HSV (Hue, Saturation, Value)
------------------------------------------------------------

El modelo HSV representa los colores de forma más cercana a cómo los percibe el ojo humano.

HSV significa:
H = Hue (Matiz o tono)
S = Saturation (Saturación)
V = Value (Valor o brillo)

Componentes:

Hue (Tono):
Representa el tipo de color.
Se mide de 0° a 360° en un círculo cromático.
0° = Rojo
120° = Verde
240° = Azul

Saturation (Saturación):
Indica qué tan intenso es el color.
100% = Color puro
0% = Gris

Value (Valor o brillo):
Indica qué tan claro u oscuro es el color.
100% = Muy brillante
0% = Negro

Se utiliza en:
Edición de imágenes
Programas de diseño
Selección de colores en software

------------------------------------------------------------

# 4. MODELO HSL (Hue, Saturation, Lightness)
------------------------------------------------------------

El modelo HSL es similar al HSV, pero cambia la forma de representar la luz.

HSL significa:
H = Hue (Matiz o tono)
S = Saturation (Saturación)
L = Lightness (Luminosidad)

Componentes:

Hue (Tono):
Se mide de 0° a 360°.

Saturation (Saturación):
Indica la intensidad del color.

Lightness (Luminosidad):
Representa la cantidad de luz.
0% = Negro
50% = Color normal
100% = Blanco

Diferencia entre HSV y HSL:
En HSV, el valor 0% es negro.
En HSL, 50% es el color puro, 0% es negro y 100% es blanco.

Se utiliza en:
Diseño gráfico
CSS en páginas web
Interfaces digitales

------------------------------------------------------------

# DIFERENCIAS GENERALES
------------------------------------------------------------

RGB → Modelo aditivo (luz). Se usa en pantallas.
CMY → Modelo sustractivo (tinta). Se usa en impresión.
HSV → Modelo más intuitivo basado en tono, saturación y brillo.
HSL → Similar a HSV, pero con diferente representación de la luminosidad.


# Ahora te enseñare como poner de color las caras de un cubo

## Tutorial: Cómo iluminar un cubo y sus caras en Blender

A continuación se muestra un pequeño tutorial para iluminar un cubo en Blender.

### Paso 1: Abrir Blender

Abre el programa Blender. Al iniciar aparecerá una escena con un cubo por defecto.

<img width="960" height="565" alt="image" src="https://github.com/user-attachments/assets/a84f0f9d-5b67-4b6d-8020-c98bc8cd8a0d" />


Si no aparece, puedes agregar uno desde:

Add → Mesh → Cube

### Paso 2: Cambiar a modo de visualización

En la parte superior izquierda objet mode por edit mode

<img width="960" height="566" alt="image" src="https://github.com/user-attachments/assets/2de9f12f-3c99-4474-8d99-6a048e569bea" />

luego seleccionamos celect mode:face

<img width="960" height="562" alt="image" src="https://github.com/user-attachments/assets/7d6995c9-53fa-4d23-82cf-0e907a486f96" />

### Paso 3: Iluminar cara del cubo
Seleccionamos la cara del cubo que bayamos a iluminar 

<img width="959" height="565" alt="image" src="https://github.com/user-attachments/assets/1ea9a4ab-c593-4c3e-a880-199fc1c4dac1" />

despues en la parte derecha nos vamos a material 

<img width="958" height="565" alt="image" src="https://github.com/user-attachments/assets/f568379a-283d-4a30-acda-7d12ab97925d" />

despues seleccionamos Add material slot

<img width="960" height="563" alt="image" src="https://github.com/user-attachments/assets/7a91dd3d-39f2-4045-a122-144ad43fbb39" />

Después seleccionamos select

<img width="960" height="561" alt="image" src="https://github.com/user-attachments/assets/894e2eb3-f40f-4ad4-a6ad-b51089bbed9d" />

Selecciónelos new

<img width="960" height="562" alt="image" src="https://github.com/user-attachments/assets/7b65fa34-7fb2-4f5d-af6a-4b95b23f67d7" />



### Paso 4: Colorear las caras del cubo

Después seleccionamos el color

<img width="960" height="563" alt="image" src="https://github.com/user-attachments/assets/aab342ed-8ad0-4846-b625-75fdceb64725" />

Después es la parte superior derecha seleccionamos v y v, wport shading: material preview

<img width="960" height="565" alt="image" src="https://github.com/user-attachments/assets/65d2b1d5-f24a-492f-84cc-aa59f44bc835" />

Y haci quedaría nuestra primer cara del cubo iluminada

<img width="960" height="561" alt="image" src="https://github.com/user-attachments/assets/b3f7e4df-4e57-49f4-a01f-d15648173d29" />

Y volvemos hacer el mismo procedimiento para volver a iluminar la segunda cara y podemos seguir así repitiendo el proceso hasta poder completar todas las caras de diferentes colores de iluminación

<img width="960" height="562" alt="image" src="https://github.com/user-attachments/assets/7847721b-b9af-4534-9cf8-180f1871332d" />

## Conclusión

En esta práctica en Blender aprendí a ponerle diferentes colores a cada cara de un cubo usando materiales. También aprendí cómo hacer que cada lado se vea iluminado y cómo aplicar los materiales correctamente en el objeto.

Al principio me costó un poco entender cómo seleccionar cada cara y asignarle su color, pero practicando fui entendiendo mejor cómo funciona Blender. Esta actividad me ayudó a conocer más las herramientas básicas del programa y cómo cambiar la apariencia de un objeto 3D.

Al final logré hacer un cubo con diferentes colores en cada cara, lo que me permitió practicar y aprender algo nuevo dentro de Blender.

---

## 1.5. Representación y trazo de líneas y polígonos

La representación y el trazo de líneas y polígonos es uno de los fundamentos principales de la graficación por computadora. A partir de estos elementos básicos se construyen todas las figuras y objetos que vemos en la pantalla, tanto en gráficos 2D como en modelos 3D.

### Representación de líneas

Una línea en el entorno digital se representa mediante dos puntos en el plano cartesiano:

(x1, y1) → punto inicial  
(x2, y2) → punto final  

La computadora no dibuja la línea como en el papel, sino que en realidad enciende pequeños puntos llamados píxeles para simular la línea entre esos dos puntos. Para lograr esto, se utilizan algoritmos matemáticos que calculan qué píxeles deben activarse para que la línea se vea recta y continua.

Algunos algoritmos importantes para el trazo de líneas son:

- **Algoritmo DDA (Digital Differential Analyzer)**  
  Calcula los puntos intermedios usando incrementos pequeños y progresivos.

- **Algoritmo de Bresenham**  
  Es más eficiente porque utiliza principalmente operaciones con números enteros, lo que lo hace más rápido para las computadoras.

Estos algoritmos permiten que las líneas se dibujen correctamente en cualquier dirección.

### Representación de polígonos

Un polígono es una figura geométrica cerrada formada por tres o más líneas rectas unidas por sus extremos. Cada punto donde se unen las líneas se llama **vértice**.

Ejemplos:

- 3 vértices → Triángulo  
- 4 vértices → Cuadrado o rectángulo  
- 5 vértices → Pentágono  

En gráficos por computadora, un polígono se representa mediante una lista ordenada de vértices:

(x1, y1)  
(x2, y2)  
(x3, y3)  
...  

Al unir estos puntos en orden se forma la figura.

### Polígonos en 3D

En gráficos tridimensionales los polígonos también incluyen la coordenada Z:

(x, y, z)

En el modelado 3D, la mayoría de los objetos están formados por muchos polígonos pequeños que juntos crean superficies complejas. Normalmente se utilizan triángulos porque son más fáciles de procesar por la computadora.

Por ejemplo, un cubo en 3D está compuesto por 6 caras, y cada cara puede dividirse en dos triángulos.

### Relleno y renderizado

Después de trazar el contorno del polígono, la computadora puede rellenarlo con un color, una textura o aplicar iluminación. Este proceso es importante en videojuegos y animaciones, ya que permite que los objetos tengan apariencia realista.

El cálculo del relleno también utiliza algoritmos que determinan qué píxeles están dentro del polígono.

### Importancia

La representación y el trazo de líneas y polígonos es la base de toda la graficación digital. Desde figuras simples en 2D hasta modelos complejos en 3D, todo se construye a partir de estos elementos.

Sin líneas y polígonos no sería posible crear personajes, escenarios, objetos ni animaciones dentro de una computadora.

---

## 1.5.1 Formatos de imagen

Los formatos de imagen son estructuras digitales que permiten almacenar y visualizar imágenes en diferentes dispositivos. Cada formato tiene características específicas que lo hacen más adecuado dependiendo del uso que se le quiera dar, como calidad, tamaño del archivo o compatibilidad.

Existen dos tipos principales de imágenes digitales:

### Imágenes rasterizadas (mapa de bits)

Están formadas por píxeles. Cada píxel contiene información de color.  
Si la imagen se amplía demasiado, puede perder calidad y verse borrosa.

Formatos más comunes:

- **JPEG (.jpg)**  
  Muy utilizado para fotografías. Tiene buena calidad y tamaño reducido, pero pierde un poco de información al comprimirse.

- **PNG (.png)**  
  Permite fondo transparente y no pierde calidad al comprimirse.

- **BMP (.bmp)**  
  Formato básico sin compresión. Archivos más pesados.

- **GIF (.gif)**  
  Permite animaciones simples y usa pocos colores.

### Imágenes vectoriales

Están formadas por líneas, curvas y formas definidas mediante fórmulas matemáticas.  
No pierden calidad al cambiar de tamaño.

Formatos más comunes:

- **SVG (.svg)**  
  Muy usado en diseño web.

- **EPS (.eps)**  
  Utilizado en diseño gráfico profesional.

En graficación por computadora es importante conocer los formatos de imagen, ya que dependiendo del proyecto se debe elegir el formato adecuado para obtener mejor calidad o menor tamaño de archivo.

---

## Ejercicio práctico: Dibujo de un polígono

En esta práctica se realizó el dibujo de un polígono utilizando herramientas de modelado. El objetivo fue comprender cómo se representan las figuras mediante vértices y líneas, y cómo se forman las caras al unir estos puntos.

<img width="955" height="559" alt="image" src="https://github.com/user-attachments/assets/91b2f67b-4ba6-47d6-82b2-d6758cc71916" />

Durante el ejercicio se trabajó con:

- Creación de vértices  
- Unión de aristas  
- Formación de caras  
- Aplicación básica de materiales  

Y podemos cambiarle el radio y podemos ponerle mas lados 

<img width="955" height="562" alt="image" src="https://github.com/user-attachments/assets/5eafc921-5505-45ed-bac1-c00bc3069323" />

Esta práctica permitió entender cómo se construyen las figuras en gráficos 2D y 3D a partir de estructuras geométricas simples.

---

## Ejercicio práctico: La Flor de la Vida

En esta práctica se realizó el diseño de la figura conocida como “Flor de la Vida”, que está compuesta por múltiples círculos superpuestos de forma simétrica.

<img width="960" height="563" alt="image" src="https://github.com/user-attachments/assets/fd0ad2c2-ba1d-43c8-975c-bfeb0a8e33d1" />


El objetivo del ejercicio fue:

- Practicar el uso de figuras geométricas básicas  
- Trabajar con simetría y repetición  
- Comprender la precisión en la colocación de objetos  

 y podemos modificar para que la flor se vea con  mas vueltas Cada 60 grados para obtener 6 círculos alrededor

 <img width="960" height="564" alt="image" src="https://github.com/user-attachments/assets/6b8c63b5-244e-411e-bef9-8126b30d647b" />


Este ejercicio ayudó a mejorar el manejo de herramientas de transformación como mover, rotar y escalar objetos dentro del entorno de trabajo.

---

## 1.6. Procesamiento de mapas de bits

El procesamiento de mapas de bits consiste en la manipulación y modificación de imágenes formadas por píxeles. Un mapa de bits (bitmap) es una imagen digital compuesta por una matriz de puntos llamados píxeles, donde cada píxel contiene información de color.

Este tipo de imágenes son conocidas como imágenes rasterizadas y se utilizan principalmente en fotografías y gráficos digitales.

### ¿Qué es un píxel?

Un píxel es la unidad más pequeña de una imagen digital. Cada píxel almacena información de color, normalmente representada en el modelo RGB.

Por ejemplo:

(255, 0, 0) → Rojo  
(0, 255, 0) → Verde  
(0, 0, 255) → Azul  

La combinación de millones de píxeles permite formar una imagen completa.

---

### Resolución

La resolución indica la cantidad de píxeles que tiene una imagen.

Ejemplo:

1920 x 1080 significa que la imagen tiene 1920 píxeles de ancho y 1080 de alto.

Entre mayor resolución tenga una imagen, mayor será su nivel de detalle, pero también aumentará el tamaño del archivo.

---

### Operaciones básicas en mapas de bits

El procesamiento de mapas de bits incluye varias operaciones, entre ellas:

- Ajuste de brillo  
- Ajuste de contraste  
- Cambios de color  
- Filtros  
- Recorte  
- Escalado  
- Rotación  

Estas operaciones se realizan modificando directamente los valores de los píxeles.

---

### Filtros digitales

Los filtros permiten modificar la apariencia de una imagen aplicando operaciones matemáticas sobre los píxeles.

Algunos ejemplos son:

- Filtro de desenfoque  
- Filtro de nitidez  
- Detección de bordes  
- Escala de grises  

Estos filtros son muy utilizados en edición de imágenes, fotografía digital y visión por computadora.

---

### Ventajas de los mapas de bits

- Permiten representar imágenes con muchos detalles.
- Son ideales para fotografías.
- Son compatibles con la mayoría de los dispositivos.

### Desventajas

- Pierden calidad al ampliarse.
- Los archivos pueden ser pesados si tienen alta resolución.

---

### Importancia en la graficación por computadora

El procesamiento de mapas de bits es fundamental en áreas como:

- Edición de imágenes  
- Diseño gráfico  
- Videojuegos  
- Animación  
- Medicina (imágenes médicas)  

Permite mejorar, analizar y modificar imágenes digitales para diferentes aplicaciones.

---
## Bibliografía

Angel, E., & Shreiner, D. (2015). *Interactive computer graphics: A top-down approach with WebGL* (7th ed.). Pearson.

Foley, J. D., Van Dam, A., Feiner, S. K., & Hughes, J. F. (2014). *Computer graphics: Principles and practice* (3rd ed.). Addison-Wesley.

Hearn, D., & Baker, M. P. (2011). *Computer graphics with OpenGL* (4th ed.). Pearson Education.

Hill, F. S., & Kelley, S. M. (2014). *Computer graphics using OpenGL* (3rd ed.). Pearson.

Gonzalez, R. C., & Woods, R. E. (2018). *Digital image processing* (4th ed.). Pearson.

Burger, W., & Burge, M. J. (2016). *Principles of digital image processing: Core algorithms*. Springer.

Blender Foundation. (2023). *Blender manual*. https://docs.blender.org/manual/en/latest/****



