## Elementos FabLab

Para el lanzamiento de **Trendvision** (*Soporte modular inteligente para plantas*) preparamos dos elementos físicos que nos permiten dar a conocer la solución y dirigir a las personas a nuestro prototipo en línea: una hoja de stickers y un llavero impreso en 3D. Los necesitamos para el **12 de noviembre**.

### Elemento 1 · Hoja de stickers con código QR

**Para qué sirve en la campaña:** Los stickers se entregan a las personas que visitan nuestro stand y se pegan en cuadernos, botellas, laptops o macetas. Cada sticker lleva el logo, el nombre, el eslogan y un código QR que abre el prototipo en https://trendvision27.netlify.app/. Así la campaña sigue visible después del evento y facilita el acceso a la solución.

**Contenido del diseño (cada sticker):**
- Logo de Trendvision (hoja verde con detalle naranja y su planta), en la parte superior.
- Nombre: **Trendvision**.
- Eslogan: *Soporte modular inteligente para plantas*.
- Código QR de 22 × 22 mm que enlaza a https://trendvision27.netlify.app/, con margen blanco alrededor para que se lea bien.

| Característica | Detalle |
|---|---|
| Medidas de cada sticker | 50 × 50 mm (5 × 5 cm) |
| Medidas de la hoja | Tamaño carta: 215,9 × 279,4 mm |
| Distribución | 4 columnas × 5 filas = 20 stickers por hoja, con 3 mm de separación entre ellos |
| Material | Papel adhesivo blanco, mate |
| Espesor | Aprox. 0,1 mm |
| Cantidad | 2 hojas (40 stickers en total) |
| Servicio | Impresión 2D a color en papel adhesivo y recorte posterior de cada sticker |
| Archivo | hoja-stickers.pdf |
| Tiempo estimado | 15 min de impresión y 30 min de recorte (aprox. 45 min en total) |

### Elemento 2 · Llavero impreso en 3D

**Para qué sirve en la campaña:** El llavero es el obsequio principal del lanzamiento. Lleva en relieve el ícono de la hoja y el nombre Trendvision, de modo que las personas se lleven un objeto útil que también les recuerde la solución. Además, muestra las posibilidades de fabricación digital que usamos en el proyecto.

| Característica | Detalle |
|---|---|
| Medidas | 72 × 30 × 4,2 mm (largo × ancho × alto) |
| Composición del espesor | Base de 3 mm y relieve de 1,2 mm |
| Perforación para la argolla | Orificio de 5 mm de diámetro, a 6 mm del borde izquierdo |
| Material | PLA |
| Color | Verde claro y verde oscuro |
| Cantidad | 10 llaveros (5 en verde claro y 5 en verde oscuro) |
| Servicio | Impresión 3D |
| Archivo | llavero-3d.stl |
| Parámetros de impresión | Altura de capa de 0,2 mm, relleno del 20 % y sin soportes |
| Tiempo estimado | Aprox. 40 min por pieza; unas 7 horas para las 10 piezas |

### Pasos para modelar el llavero en Tinkercad y exportarlo en STL

1. Ingresamos a Tinkercad y creamos un diseño nuevo. Configuramos la cuadrícula en milímetros.
2. Arrastramos una **Caja** al plano de trabajo y fijamos sus medidas en 72 mm (largo), 30 mm (ancho) y 3 mm (alto). Esta es la base.
3. Redondeamos las esquinas. Para ello, aumentamos el radio de la caja o combinamos cilindros en los extremos.
4. Colocamos un **Cilindro** de 5 mm de diámetro cerca del extremo izquierdo, lo convertimos en **Agujero** y lo alineamos con el centro de la base para formar la perforación de la argolla.
5. Importamos el ícono de la hoja del logo en formato SVG, o lo modelamos con formas básicas. Lo escalamos para que quepa en la mitad izquierda de la base y fijamos su altura en 1,2 mm.
6. Añadimos la forma **Texto** con la palabra «Trendvision», con fuente en negrita y altura de 1,2 mm. La ubicamos a la derecha del ícono, centrada verticalmente.
7. Apoyamos el ícono y el texto sobre la base con la herramienta **Alinear**, de modo que queden sobre la cara superior. El alto total debe ser de 4,2 mm.
8. Seleccionamos todas las piezas y las unimos con **Agrupar**. Comprobamos las dimensiones finales: 72 × 30 × 4,2 mm.
9. Verificamos que el modelo quede apoyado sobre el plano, con la base hacia abajo y el relieve hacia arriba.
10. Hacemos clic en **Exportar**, elegimos el formato **.STL** y guardamos el archivo como `llavero-3d.stl`. Lo entregamos al FabLab junto con el color elegido.

![Elementos FabLab](../assets/fablab/foto-final.jpg)
# 10 · Campaña de lanzamiento

![Logo](../assets/campana/logo.png)

## 1. Propósito de la campaña

Trendvision es el panel de monitoreo que recibe las lecturas de sensores de temperatura, humedad ambiente y humedad del suelo de cada bloque de cultivo. Las muestra en tiempo real y envía alertas cuando un valor sale del rango óptimo para la flor. Con esta campaña queremos que el equipo comercial y los clientes de la empresa floricultora conozcan la solución y entiendan qué ganan con ella: dejar de registrar a mano las condiciones de los invernaderos y detectar a tiempo plagas, hongos o estrés hídrico para proteger la flor de calidad de exportación.

## 2. A quién le hablamos

- **Vendedores:** necesitan un mensaje sencillo y confiable para explicar que la flor viene de cultivos monitoreados de forma continua. Así pueden respaldar la calidad ante sus compradores.
- **Clientes:** buscan flor de corte (rosas, claveles y crisantemos) con calidad constante, tanto en el mercado nacional como en exportación. Les transmitimos que cada bloque de cultivo se cuida con datos oportunos.

## 3. Tono de comunicación

Nuestro tono es **cercano y confiable**. Usamos frases cortas y un lenguaje de campo, sin tecnicismos innecesarios. Hablamos de cuidado, de anticiparse y de calidad, y evitamos las promesas exageradas.

## 4. Nombre de la solución

La solución se llama **Trendvision**. Combina *trend* (tendencia, el comportamiento de las variables del cultivo en el tiempo) y *vision* (ver, tener a la vista el estado de cada bloque).

| Criterio | Evaluación | Cumple |
|---|---|---|
| Corto | Tiene once letras y dos sílabas fuertes. Se escribe, se dice y cabe en un sticker o en un ícono de aplicación sin esfuerzo. | Sí |
| Recordable | Une dos palabras conocidas y se pronuncia igual en español e inglés. Su sonido es fluido y fácil de repetir en una conversación comercial. | Sí |
| Asociado al beneficio | «Vision» remite a ver el cultivo en tiempo real, y «trend» a seguir su tendencia para anticipar anomalías. Esto resume el beneficio principal: detectar a tiempo. | Sí |

**Nombre elegido: Trendvision.**

## 5. Eslóganes

1. Detecta a tiempo, cosecha calidad.
2. Cada flor en su punto.
3. **Tu cultivo siempre a la vista.** ← *Elegido*

Elegimos el tercero porque expresa el beneficio central en pocas palabras, tiene un tono cercano y refuerza el significado del nombre. Con 29 caracteres, además, cabe bien en el logo y en los stickers.

## 6. Identidad visual

### Paleta de colores

El verde es el color principal porque remite a la naturaleza, al cultivo y a la confianza.

| Uso | Color | HEX |
|---|---|---|
| Principal (textos y contornos) | Verde bosque | `#1B5E20` |
| Secundario (símbolo y acentos) | Verde hoja | `#66BB6A` |
| Fondo | Blanco hoja | `#F7FAF5` |

### Tipografía

Usamos **Poppins**, una tipografía gratuita de Google Fonts. Sus formas redondeadas y su buena legibilidad refuerzan el tono cercano y confiable. Empleamos Poppins Bold para el nombre y Poppins Regular para el eslogan y los textos de apoyo.

### Qué representa el logo

El logo muestra un ojo que contiene una hoja como pupila. Representa la vigilancia constante del cultivo y el cuidado de la flor.

![Logo](../assets/campana/logo.png)

## 7. Stickers de lanzamiento

Para el lanzamiento entregaremos a los asistentes, vendedores y clientes una hoja de **12 stickers de 5 × 5 cm**. Cada sticker lleva el logo, el nombre **Trendvision**, el eslogan «Tu cultivo siempre a la vista» y un **código QR** que lleva al prototipo: [https://trendvision27.netlify.app/](https://trendvision27.netlify.app/).

- **Formato:** 12 stickers distribuidos en 3 columnas por 4 filas, con separación suficiente para recortarlos fácilmente.
- **Colores:** fondo blanco hoja (`#F7FAF5`), textos en verde bosque (`#1B5E20`) y acentos en verde hoja (`#66BB6A`).
- **Uso:** los asistentes pueden pegarlos en sus cuadernos, equipos o herramientas de trabajo. Al escanear el QR con el celular acceden directamente al prototipo.

![Hoja de stickers](../assets/campana/hoja-stickers.png)

## 8. Mensajes clave

- **Para vendedores:** «Respalde cada pedido con cultivos monitoreados de forma continua».
- **Para clientes:** «La flor que recibe se cuidó con datos, bloque por bloque».
- **Para ambos:** «Tu cultivo siempre a la vista».
