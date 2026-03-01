# Nuevo Hogar (App de Adopción)

## Descripción de la app
**Nuevo Hogar** es una aplicación enfocada en la presentación visual de una ficha de adopción.  
La pantalla muestra una **imagen principal de la mascota**, información básica (nombre y edad), un **campo de texto** para registrar el nombre del adoptante, un **widget de puntuación** (estrellas) acompañado por una **barra de progreso**, y dos botones de acción: **Adoptar** y **Contactar**.

Este proyecto prioriza el **diseño UI** (orden, jerarquía visual, colores, tamaños, bordes redondeados y sombras) siguiendo una estructura clara y amigable para el usuario.

---

## Imagen final de la app terminada
**(Coloca aquí tu captura final)**

![App final](docs/images/final.png)

**Explicación breve:**  
La vista final mantiene el orden de elementos y aplica una paleta moderna: textos con jerarquía (nombre más destacado), widget con color personalizado y botones con colores diferenciados para acción principal y secundaria, incluyendo bordes redondeados y sombras para profundidad visual.

---

## Imagen de la plantilla blanca (base de construcción)
**(Coloca aquí tu captura de la plantilla blanca)**

![Plantilla blanca](docs/images/plantilla_blanca.png)

**Explicación breve:**  
La plantilla blanca representa la estructura inicial sin énfasis de color. Sirve como base para posicionar y alinear correctamente todos los elementos (imagen, textos, input, widget y botones) antes de aplicar estilos visuales finales.

---

## Imagen de la plantilla turquesa (maqueta de la app)
**(Coloca aquí tu captura de la plantilla turquesa)**

![Plantilla turquesa](docs/images/plantilla_turquesa.png)

**Explicación breve:**  
La plantilla turquesa funciona como maqueta visual del estilo. Se utiliza un color de acento para reforzar el enfoque tecnológico/moderno, especialmente en elementos interactivos como la barra de progreso y componentes principales.

---

## Elementos incluidos (Imagen, Texto, Input, Widget, Botones) + atributos usados y sustento

## 1) Imagen
**Elemento usado:** `ImageView` dentro de `MaterialCardView` (o CardView)

**Atributos aplicados:**
- `android:src="@drawable/fotogato"`: carga la imagen desde `res/drawable/`.
- `android:scaleType="centerCrop"`: recorta y encuadra la imagen sin deformarla.
- `app:cardCornerRadius="18dp"`: bordes redondeados para estilo moderno.
- `app:cardElevation="10dp"`: sombra para profundidad visual (efecto tarjeta).

**Sustento:**  
La imagen es el elemento principal de la ficha, por eso se coloca arriba y con formato tipo tarjeta para atraer la atención primero.

---

## 2) Texto
**Elementos usados:** `TextView` (Nombre y Edad)

**Cambios requeridos cumplidos:** se cambió **tamaño** y **color** según convenga.

**Atributos aplicados:**
- **Nombre**
  - `android:textSize="32sp"` y `android:textStyle="bold"`: máxima jerarquía visual.
  - `android:textColor="#1B1B1B"`: color fuerte para lectura clara.
- **Edad**
  - `android:textSize="22sp"`: menor jerarquía.
  - `android:textColor="#5B5B5B"`: color secundario (gris) para diferenciar del nombre.

**Sustento:**  
Se aplicó jerarquía tipográfica: lo más importante (nombre) se ve primero y más fuerte; lo secundario (edad) acompaña sin competir.

---

## 3) Input
**Elemento usado:** `EditText` (Nombre del adoptante)

**Atributos aplicados:**
- `android:hint="Nombre del adoptante"`: guía visual del campo.
- `android:inputType="textPersonName"`: adecuado para nombres.
- `android:textSize="18sp"`: tamaño legible y consistente.
- `android:backgroundTint="#009688"`: color de acento en el subrayado (estilo moderno).

**Sustento:**  
El input se coloca después de ver la mascota para que el usuario registre su dato con claridad en un solo paso, sin recargar la pantalla.

---

## 4) Widget
**Elementos usados:** `RatingBar` + `ProgressBar` horizontal

**Cambios requeridos cumplidos:** se cambió el **color del widget**.

**Atributos aplicados:**
- `RatingBar`
  - `android:numStars="5"` y `android:stepSize="1"`: puntuación estándar (1 a 5).
- `ProgressBar`
  - `style="?android:attr/progressBarStyleHorizontal"`: barra horizontal.
  - `android:progressTint="#009688"`: color turquesa (acento).
  - `android:backgroundTint="#DADADA"`: contraste con el fondo.
  - `android:progress="80"` y `android:max="100"`: representación simple del estado.

**Sustento:**  
El rating se entiende rápido con estrellas y la barra refuerza visualmente el puntaje (lectura inmediata incluso sin contar estrellas).

---

## 5) Botones
**Elemento usado:** `MaterialButton` (Adoptar / Contactar)

**Cambios requeridos cumplidos:** se cambió **color del botón** y **color del texto**.

**Atributos aplicados:**
- `android:backgroundTint="#009688"` (Adoptar): acción principal.
- `android:backgroundTint="#3B3B40"` (Contactar): acción secundaria.
- `android:textColor="@android:color/white"`: contraste alto y legibilidad.
- `app:cornerRadius="18dp"`: botones redondeados (estética moderna).
- `android:elevation="8dp"`: sombra para efecto “clickable” y profundidad.

**Sustento:**  
Se diferenció la acción principal (Adoptar) con color de acento y la secundaria (Contactar) con un tono oscuro. Esto guía al usuario a la acción más importante.

---

## Estructura de carpetas sugerida para el README (imágenes)
Guarda tus capturas en:

- `docs/images/final.png`
- `docs/images/plantilla_blanca.png`
- `docs/images/plantilla_turquesa.png`

Luego el README las mostrará automáticamente con los enlaces de arriba.

---

## Nota final
La interfaz fue desarrollada priorizando:
- orden visual (de arriba hacia abajo),
- jerarquía tipográfica,
- consistencia de color (turquesa como acento),
- componentes con bordes redondeados y sombras para un estilo moderno.
