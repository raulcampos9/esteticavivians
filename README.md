# Estética Vivians

Sitio web profesional para Estética Vivians, desarrollado como proyecto integrador del curso de JavaScript. El objetivo es que el sitio sea funcional en producción una vez finalizado el curso.

---

## Demo

[Ver sitio en vivo](https://raulcampos9.github.io/esteticavivians)

---

## Descripción

Estética Vivians es un centro de estética ubicado en Buenos Aires, Argentina. El sitio web cubre dos áreas principales:

- **Estética:** presentación de tratamientos faciales, corporales y depilación, con descripción, precio, duración y botón para agendar turno vía WhatsApp.
- **Tienda:** catálogo de productos de belleza dividido en cremas, perfumes y maquillaje, con descripción, precio y botón de consulta vía WhatsApp.

---

## Tecnologías utilizadas

| Tecnología | Uso |
|------------|-----|
| HTML5 | Estructura y semántica de todas las páginas |
| CSS3 | Estilos, Flexbox, Grid, animaciones, responsive |
| JavaScript | Pendiente — se incorpora en etapas siguientes del curso |
| Google Fonts | Fuente Playfair Display para el cuerpo del texto |
| Font Awesome 6 | Íconos en botones y datos de contacto |
| Git + GitHub | Control de versiones y despliegue |
| GitHub Pages | Hosting del sitio estático |

**Fuente propia:** BrunoAceSC (archivo .ttf incluido en `/font/`)

---

## Estructura del proyecto

```
esteticavivians/
│
├── index.html                      — página principal
│
├── css/
│   └── estilo.css                  — hoja de estilos unificada para todo el sitio
│
├── js/
│   └── main.js                     — pendiente, se implementa con JS del curso
│
├── font/
│   └── BrunoAceSC-Regular.ttf      — fuente personalizada para títulos
│
├── imagenes/
│   ├── bienvenida/                 — imagen hero de la página principal
│   ├── tratamientos/               — imágenes de faciales, corporales y depilación
│   ├── tienda/                     — imágenes de categorías de productos
│   └── favicon/                    — íconos del sitio
│
├── videos/                         — pendiente, para mostrar tratamientos
│
├── html/
│   ├── nosotros.html               — pendiente
│   ├── contacto.html               — página de contacto con formulario y mapa
│   ├── turnos.html                 — pendiente
│   │
│   ├── tratamientos/
│   │   ├── faciales.html           — lista de tratamientos faciales
│   │   ├── corporales.html         — pendiente
│   │   └── depilacion.html         — pendiente
│   │
│   └── tienda/
│       ├── index.html              — página principal de la tienda
│       ├── cremas.html             — galería de cremas
│       ├── perfumes.html           — pendiente
│       └── maquillaje.html         — pendiente
│
└── git-scripts/
    ├── git-nuevo-proyecto.bat      — automatiza la creación de un nuevo repo
    ├── git-subir-cambios.bat       — automatiza commits y push
    ├── git-borrar-archivo.bat      — elimina archivos del repositorio
    ├── git-crear-gitignore.bat     — genera el archivo .gitignore
    └── git-panel.bat               — panel de control de Git
```

---

## Decisiones técnicas

**Un solo archivo CSS**
Todo el sitio usa `estilo.css`. Centralizar los estilos facilita el mantenimiento: cambiar un color o fuente en un solo lugar actualiza todo el sitio.

**Sin JavaScript por ahora**
El curso introduce JS progresivamente. La primera entrega es HTML y CSS puro. El menú hamburguesa en mobile y la dinámica de productos se agregarán en etapas siguientes.

**Menú desplegable con CSS puro**
Los submenús de Tratamientos y Tienda se activan con `:hover` en CSS, sin necesidad de JS.

**Productos hardcodeados en HTML**
En la etapa actual los productos se escriben directamente en el HTML. Cuando se llegue a la sección de arrays en el curso, se reemplazará por generación dinámica con JavaScript.

**Turnos online vía WhatsApp**
Por ahora el botón de agendar turno abre WhatsApp con un mensaje predefinido. En versiones futuras se implementará un sistema de calendario.

**Responsive design**
El sitio está optimizado para tres tamaños de pantalla:
- Desktop: mayor a 768px
- Tablet: hasta 768px
- Mobile: hasta 480px

---

## Paleta de colores y tipografía

| Elemento | Valor |
|----------|-------|
| Color primario | `#2c3e50` azul oscuro |
| Color acento | `#c9a96e` dorado |
| Color fondo | `#faf9f7` crema suave |
| Fuente títulos | BrunoAceSC (fuente propia) |
| Fuente cuerpo | Playfair Display (Google Fonts) |

---

## Cómo correr el proyecto localmente

1. Clonar el repositorio:
```bash
git clone https://github.com/raulcampos9/esteticavivians.git
```

2. Abrir `index.html` en el navegador. No requiere servidor local ni dependencias.

---

## Roadmap

### Etapa 1 — HTML y CSS (actual)
- [x] Página principal con hero, tratamientos y tienda
- [x] CSS unificado con variables, Flexbox, Grid y responsive
- [x] Navegación con submenús desplegables en CSS puro
- [x] Página de contacto con formulario y mapa
- [x] Página de tratamientos faciales
- [x] Galería de cremas
- [x] Scripts de automatización para Git
- [ ] Nosotros
- [ ] Turnos online
- [ ] Corporales y depilación
- [ ] Perfumes y maquillaje

### Etapa 2 — JavaScript (próxima)
- [ ] Menú hamburguesa funcional en mobile
- [ ] Productos cargados dinámicamente desde arrays
- [ ] Validación del formulario de contacto
- [ ] Filtros de productos por categoría

### Etapa 3 — Producción (futuro)
- [ ] Backend con Node.js
- [ ] Base de datos para productos y tratamientos
- [ ] Panel de administración para cargar contenido
- [ ] Sistema de turnos con calendario
- [ ] Vouchers de regalo
- [ ] Integración con MercadoPago
- [ ] Videos de tratamientos

---

## Changelog

### v0.2.1 — 2025
- Actualización de fuentes
- Imágenes agregadas al proyecto

### v0.2.0 — 2025
- Nueva página principal con hero de imagen completa
- CSS completamente unificado en un solo archivo
- Menú de navegación con submenús desplegables
- Sección de tratamientos en el index
- Franja con frase motivacional
- Reestructura de carpetas del proyecto
- Página de tratamientos faciales con layout de 3 columnas

### v0.1.0 — 2025
- Estructura base del proyecto
- Header y navegación
- Página de tienda con categorías
- Galería de productos (cremas) con imagen, descripción y precio
- Botón de consulta vía WhatsApp
- Página de contacto con formulario, mapa y redes sociales
- Scripts de automatización para Git (.bat)
- Diseño responsive para tablet y mobile

---

## Autor

Desarrollado por **Raul Campos** como proyecto integrador del curso de JavaScript.

---

## Estado del proyecto

🚧 En desarrollo — Etapa 1 de 3
