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
