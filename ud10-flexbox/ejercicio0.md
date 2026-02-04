# Aclaraciones del Ejercicio 0

https://codepen.io/fgomrom726/pen/azZEpqX

Explicación didáctica por bloques

1. Modelo de caja

width y height no incluyen padding ni border.

Tamaño real de .caja:

150px (ancho)

padding (20px)

borde (4px)

Esto permite introducir la idea de box-sizing más adelante.

2. display

Al usar display: inline-block:

Se colocan en línea

Respetan ancho y alto

Admiten márgenes y padding

Comparación rápida en clase:

inline: no respeta ancho/alto

block: ocupa toda la línea

inline-block: comportamiento intermedio

3. margin y padding

margin: separa elementos entre sí

padding: separa el contenido del borde

Se visualiza claramente gracias al fondo y al borde

4. Posicionamiento (position)

.contenedor → position: relative

.especial → position: absolute

La caja especial:

Sale del flujo normal

Se posiciona respecto al contenedor, no al body

Este punto es clave para entender layouts más adelante.

5. Selectores y herencia

body define tipografía y color base

Esos estilos se heredan automáticamente

.especial sobrescribe el color heredado

nav a demuestra selector descendente

:hover introduce pseudoclases


Preguntas conceptuales (comprensión)

1. ¿Qué partes componen el modelo de caja (box model) de un elemento en CSS?
A. margin, border, padding y content
B. width, height, color y font
C. padding, background y display
D. content, position y float

Respuesta correcta: A

2. ¿Qué propiedad define cómo se calcula el tamaño total de un elemento según el modelo de caja?
A. display
B. box-sizing
C. position
D. overflow

Respuesta correcta: B

3. ¿Cuál es la diferencia principal entre margin y padding?
A. margin afecta al interior del elemento y padding al exterior
B. padding afecta al interior del elemento y margin al exterior
C. Ambos hacen exactamente lo mismo
D. Solo padding acepta valores negativos

Respuesta correcta: B

Preguntas sobre display

4. ¿Qué comportamiento tiene por defecto un elemento con display: block?
A. Se ajusta al contenido y no permite margen vertical
B. Ocupa solo el ancho necesario
C. Ocupa todo el ancho disponible y comienza en una nueva línea
D. Se comporta como un elemento en línea

Respuesta correcta: C

5. ¿Qué ventaja tiene display: inline-block frente a inline?
A. Permite definir width y height
B. Ocupa toda la línea
C. No admite margen ni padding
D. Se comporta como un bloque completo

Respuesta correcta: A

Selectores y herencia

6. ¿Qué selector tiene mayor especificidad?
A. .caja
B. div
C. #principal
D. *

Respuesta correcta: C

7. ¿Qué propiedad se hereda automáticamente por los elementos hijos?
A. margin
B. padding
C. color
D. width

Respuesta correcta: C

Posicionamiento básico (conceptual)

8. ¿Cuál es la diferencia entre position: relative y position: absolute?
A. Relative saca el elemento del flujo y absolute no
B. Absolute se posiciona respecto al viewport siempre
C. Relative mantiene su espacio y absolute no
D. Ambas hacen exactamente lo mismo

Respuesta correcta: C

9. ¿Qué elemento se usa como referencia para un elemento con position: absolute?
A. Siempre el body
B. El elemento anterior en el HTML
C. El contenedor padre posicionado
D. El navegador

Respuesta correcta: C

Preguntas de razonamiento práctico

10. Si un elemento tiene width: 200px y padding: 20px, ¿cuál será su ancho real con box-sizing: content-box?
A. 200px
B. 220px
C. 240px
D. Depende del navegador

Respuesta correcta: C

11. ¿Por qué estos conocimientos son necesarios antes de usar Flexbox o Grid?
A. Porque Flexbox reemplaza todas las propiedades anteriores
B. Porque Flexbox y Grid no usan el modelo de caja
C. Porque el comportamiento de los elementos depende de display, box model y herencia
D. Porque son obligatorios por la especificación CSS

Respuesta correcta: C