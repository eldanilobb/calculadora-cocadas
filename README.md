# 🧁 El Sabor de las Matemáticas: Cocadas Mágicas

Aplicación web educativa interactiva desarrollada especialmente para niñas y niños de 8 años en evaluación y apoyo de **Educación Diferencial** y aprendizaje de matemáticas iniciales.

A través del enfoque **CPA (Concreto - Pictórico - Abstracto)**, los estudiantes transitan desde la manipulación física de dulces hasta la comprensión del valor posicional en el sistema decimal:
* **Cocada de Coco (Grande, tono avena/dorado)** = **DECENA (D)** = Vale 10 unidades.
* **Cocada con Chispas (Pequeña, chispitas de colores)** = **UNIDAD (U)** = Vale 1 unidad.

---

## 🌟 Características Pedagógicas y de Accesibilidad

1. **Diseño Visual Infantil Amigable**:
   - Fondo cuadriculado pastel estilo cuaderno escolar.
   - Tipografía redondeada y legible (`Fredoka` y `Quicksand`).
   - Botones táctiles extragrandes con retroalimentación háptica/visual (`active:scale-95`).
   - Colores suaves y cálidos: menta, vainilla, lila, caramelo (decenas) y rosa pastel (unidades).

2. **Refuerzo Positivo Incondicional**:
   - Cero mensajes frustrantes o alertas rojas punitivas.
   - En caso de acierto: fiesta de confeti, arpegio de campanas y acumulación de estrellas.
   - En caso de error: acompañamiento cálido (*"¡Estuviste muy cerca! Vamos a contarlas juntas"*) y botón de pista guiada paso a paso.

3. **Soporte Auditivo Lúdico**:
   - Sonidos dulces sintetizados con `Web Audio API` (sin archivos pesados ni dependencias externas).
   - Interruptor rápido para silenciar sonido si existe sensibilidad auditiva.

---

## 🗂️ Módulos de la Aplicación

### 1. 🧮 Mi Calculadora de Mesa (Paso Concreto a Simbólico)
- Diseñada para cuando la niña tiene cocadas físicas en su mesa.
- Contadores táctiles de Decenas y Unidades con botones gigantes `[+]` y `[-]`.
- Bandejas dinámicas que muestran las cocadas contadas.
- **Tabla de Valor Posicional Vertical** (`D` en naranja / `U` en rosa).
- Desglose matemático: *"2 cocadas de coco son 20 + 3 cocadas con chispas son 3 = ¡Tienes 23 en total!"*.
- Tarjeta gigante del total con el número y su lectura en palabras (*"Veintitrés cocadas"*).

### 2. 🎯 Mini Reto de Cocadas (Paso Pictórico)
- Ejercicios dulces aleatorios con resultado máximo de 30 para evitar fatiga cognitiva.
- Tres modalidades:
  * 🔍 **Contar**: contar las cocadas organizadas en la bandeja.
  * ➕ **Sumas**: juntar bandejas de la mañana y de la tarde.
  * ➖ **Restas**: cocadas que nos comemos (con tachita visual suave).
- Teclado numérico táctil en pantalla optimizado para tablets.
- Pistas paso a paso que agrupan de 10 en 10 y luego de 1 en 1.

### 3. 📦 Caja Mágica de Cocadas (Zona Libre Manipulativa)
- Tapete interactivo donde la niña puede experimentar libremente sin calificaciones.
- Dispensadores superiores para agregar `+ Cocada de Coco (+10)` y `+ Cocada con Chispas (+1)`.
- Cada dulce se puede tocar en el tapete para devolverlo o comérselo.
- **🪄 ¡Canje Mágico!**: cuando acumula 10 o más chispitas, se activa un botón para transformarlas en 1 cocada de coco, interiorizando el canje posicional.

---

## 🖼️ Manejo de Imágenes y Fallback

En la parte superior del script en [index.html](file:///index.html) se encuentran las constantes:
```javascript
const IMG_DECENA = 'img/cocada-coco.png';
const IMG_UNIDAD = 'img/cocada-chispas.png';
```
- Si las imágenes locales existen, se cargan con estilo responsivo y sombras suaves.
- Si las rutas están vacías o las imágenes fallan al cargar, el sistema activa automáticamente un **fallback visual elegante** en CSS/emojis para garantizar que la interfaz jamás se rompa.

---

## 🚀 Despliegue en GitHub Pages

1. Sube este repositorio a tu cuenta de GitHub:
   ```bash
   git add .
   git commit -m "feat: Calculadora de Cocadas para educacion diferencial"
   git push origin main
   ```
2. En tu repositorio en GitHub, ve a **Settings** > **Pages**.
3. En **Source**, selecciona `Deploy from a branch` y elige la rama `main` (carpeta `/root`).
4. Haz clic en **Save**. ¡En pocos segundos tu sitio estará activo en `https://<usuario>.github.io/<repositorio>/`!
