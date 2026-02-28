# Nuevo Hogar — App de Adopción 🐾

## Descripción
**Nuevo Hogar** es una app de adopción que muestra la ficha de una mascota (imagen, nombre y edad),
permite ingresar el **nombre del adoptante**, asignar una **puntuación (1–5)** y visualizarla con una
**barra de progreso**. Incluye dos acciones principales: **Adoptar** y **Contactar**.

---

## Capturas

### App terminada (pantalla final)
- Se reemplazó la imagen por una mascota distinta.
- Se ajustaron tamaños y colores de texto para jerarquía visual.
- El rating se controla con estrellas y se refleja en una barra de progreso.
- Botones con color de fondo y color de texto personalizados.

![App final](docs/images/final_screen.png)

### Plantilla blanca (base de construcción)
- Placeholder de imagen.
- Estilos neutros antes de aplicar la paleta final.

![Plantilla blanca](docs/images/template_white_screen.png)

### Plantilla turquesa (maqueta)
- Variante de maqueta con acento turquesa para el estilo de la app.

![Plantilla turquesa](docs/images/template_turquoise_screen.png)

---

## Elementos requeridos y atributos usados

### 1) Imagen
- `Image.asset`
- `BoxDecoration` con `borderRadius` y `boxShadow`
- `fit: BoxFit.cover`

### 2) Textos
- `TextStyle(fontSize, fontWeight, color)`
- Nombre con tamaño mayor (jerarquía)
- Edad con color gris (secundario)

### 3) Input
- `TextField` con `controller`
- `InputDecoration` con subrayado (Underline)
- Borde enfocado en turquesa

### 4) Widget (rating + barra)
- Estrellas con `Icons.star / star_border`
- `LinearProgressIndicator(value: rating/5)`

### 5) Botones
- `ElevatedButton`
- `backgroundColor` y `foregroundColor`
- `borderRadius` para estilo moderno

---

## Cómo ejecutar (VS Code)
```bash
flutter pub get
flutter run
