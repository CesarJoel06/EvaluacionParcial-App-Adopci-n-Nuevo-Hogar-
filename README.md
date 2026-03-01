# Nuevo Hogar (App de Adopción)

## Descripción de la app
**Nuevo Hogar** es una aplicación enfocada en la presentación visual de una ficha de adopción.  
La pantalla muestra una **imagen principal de la mascota**, información básica (nombre y edad), un **campo de texto** para registrar el nombre del adoptante, un **widget de puntuación** (estrellas) acompañado por una **barra de progreso**, y dos botones de acción: **Adoptar** y **Contactar**.

Este proyecto prioriza el **diseño UI** (orden, jerarquía visual, colores, tamaños, bordes redondeados y sombras) siguiendo una estructura clara y amigable para el usuario.

---

## Imagen final de la app terminada
**(Coloca aquí tu captura final)**
<img width="595" height="661" alt="Captura de pantalla 2026-03-01 a las 14 42 17" src="https://github.com/user-attachments/assets/bc142b44-d3b0-4f15-894d-351d7386779a" />



**Explicación breve:**  
La vista final mantiene el orden de elementos y aplica una paleta moderna: textos con jerarquía (nombre más destacado), widget con color personalizado y botones con colores diferenciados para acción principal y secundaria, incluyendo bordes redondeados y sombras para profundidad visual.

---

## Imagen de la plantilla blanca (base de construcción)
**(Coloca aquí tu captura de la plantilla blanca)**

<img width="1285" height="792" alt="Captura de pantalla 2026-03-01 a las 14 09 22" src="https://github.com/user-attachments/assets/3d0e0966-67d8-4c15-945b-1262039df49e" />

 
La plantilla blanca representa la estructura inicial sin énfasis de color. Sirve como base para posicionar y alinear correctamente todos los elementos (imagen, textos, input, widget y botones) antes de aplicar estilos visuales finales.

---

## Imagen de la plantilla turquesa (maqueta de la app)
**(Coloca aquí tu captura de la plantilla turquesa)**

<img width="341" height="598" alt="Captura de pantalla 2026-03-01 a las 14 03 28" src="https://github.com/user-attachments/assets/be331243-bf3a-40c8-af6b-ce545618d946" />


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

<img width="787" height="676" alt="Captura de pantalla 2026-03-01 a las 14 41 06" src="https://github.com/user-attachments/assets/e35a906c-811f-4a9d-bb55-0f926f290184" />

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

<img width="790" height="633" alt="Captura de pantalla 2026-03-01 a las 14 40 38" src="https://github.com/user-attachments/assets/1d245bd8-51f8-414b-9a5e-44979bf69a97" />
---

## 3) Input
**Elemento usado:** `EditText` (Nombre del adoptante)

**Atributos aplicados:**
- `android:hint="Nombre del adoptante"`: guía visual del campo.
- `android:inputType="textPersonName"`: adecuado para nombres.
- `android:textSize="18sp"`: tamaño legible y consistente.
- `android:backgroundTint="#009688"`: color de acento en el subrayado (estilo moderno).



<img width="787" height="648" alt="Captura de pantalla 2026-03-01 a las 14 40 16" src="https://github.com/user-attachments/assets/33ef25ea-7e4c-44d4-a982-f7e887f2b056" />

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


--<img width="779" height="657" alt="Captura de pantalla 2026-03-01 a las 14 39 58" src="https://github.com/user-attachments/assets/f52ab89a-e50e-4bc7-adc7-6ff50af2a22f" />
-

## 5) Botones
**Elemento usado:** `MaterialButton` (Adoptar / Contactar)

**Cambios requeridos cumplidos:** se cambió **color del botón** y **color del texto**.

**Atributos aplicados:**
- `android:backgroundTint="#009688"` (Adoptar): acción principal.
- `android:backgroundTint="#3B3B40"` (Contactar): acción secundaria.
- `android:textColor="@android:color/white"`: contraste alto y legibilidad.
- `app:cornerRadius="18dp"`: botones redondeados (estética moderna).
- `android:elevation="8dp"`: sombra para efecto “clickable” y profundidad.

<img width="782" height="663" alt="Captura de pantalla 2026-03-01 a las 14 41 26" src="https://github.com/user-attachments/assets/d03ca7d2-b93b-40ae-8510-0f1296349af6" />

---
