# Landing Page - Escuela de Danzas Populares Mexicanas


Landing page moderna para una escuela de danzas folklóricas y populares mexicanas, con carrusel de imágenes, menú hamburguesa responsivo y página de plan de Trabajo interactivo dividido por grupos de edad.

## Características

- 🇲🇽 **Enfoque en danzas mexicanas** - Contenido especializado en folklore nacional
- ✨ **Página principal** con carrusel automático de imágenes de danzas tradicionales
- 🍔 **Menú hamburguesa** responsivo con navegación (Inicio, Acerca de, Mi pequeño mundo)
- 📅 **Mi Pequeño Mundo**: Plan de Trabajo de 10 meses (40 semanas) dividido en 2 columnas por grupos de edad
- 👩‍🏫 **Sección "Acerca de"**: Perfil completo de la maestra con formación y trayectoria
- 📱 **Diseño responsivo** que se adapta a todos los dispositivos
- 🎨 **Diseño moderno** - Gradientes purple/blue elegantes y animaciones suaves
- 🔼 **Botón Scroll to Top** - Flecha para regresar al inicio de la página fácilmente
- 🌊 **Smooth Scroll** - Navegación fluida entre secciones de la página

## Estructura del Proyecto

InfLibDanz/
{{ ... }}
│   └── images/          # Carpeta para imágenes del carrusel
├── src/
│   ├── components/
│   │   ├── Header.astro   # Header con menú hamburguesa
│   │   ├── Footer.astro   # Footer del sitio
│   │   └── Carousel.astro # Carrusel de imágenes
│   ├── layouts/
│   │   └── Layout.astro   # Layout base
│   └── pages/
│       ├── index.astro              # Página principal
│       └── mi-pequeno-mundo.astro   # Plan de Trabajo
└── package.json
```

## Instalación y Uso

### 1. Instalar dependencias

```bash
npm install
```

### 2. Iniciar el servidor de desarrollo

```bash
npm run dev
```

### 3. Construir para producción

```bash
npm run build
```

### 4. Vista previa de producción

```bash
npm run preview
```

## Personalización

### Cambiar las imágenes del carrusel

1. Agrega tus imágenes en la carpeta `public/images/`
2. Nombra las imágenes como: `slide1.jpg`, `slide2.jpg`, etc.
3. Edita `src/pages/index.astro` y actualiza el array `carouselImages`:

```javascript
const carouselImages = [
  '/images/slide1.jpg',
  '/images/slide2.jpg',
  '/images/slide3.jpg',
  '/images/slide4.jpg'
];
```

### Modificar el contenido de la página principal

Edita `src/pages/index.astro` para cambiar:

- Título y descripción
- Características de la escuela
- Disciplinas ofrecidas
- Sección de llamado a la acción

### Personalizar el plan de Trabajo

En `src/pages/mi-pequeno-mundo.astro`, modifica el array `planDeTrabajo` para:

- Agregar o quitar meses
- Modificar semanas
- Cambiar objetivos y actividades

### Cambiar colores y estilos

Los colores principales están en los gradientes:

- Gradiente principal: `#667eea` → `#764ba2`

Puedes modificarlos en los archivos `.astro` en la sección `<style>`.

## Navegación

- **Inicio**: Página principal con información de la escuela
- **Mi pequeño mundo**: Plan de Trabajo detallado por meses y semanas

## Tecnologías

- [Astro](https://astro.build) - Framework web moderno
- HTML/CSS/JavaScript
- Google Fonts (Poppins)
