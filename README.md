# Sitio Web de Patricia Castro - Psicóloga

## Descripción del Proyecto
Este proyecto consiste en el desarrollo de un sitio web profesional para Patricia Castro, una psicóloga clínica especializada en terapia individual, mindfulness y bienestar emocional. El sitio tiene como objetivo proporcionar información sobre los servicios ofrecidos, compartir recursos útiles a través de un blog y facilitar el contacto con los pacientes.

## Estructura del Proyecto
El proyecto está organizado en las siguientes secciones principales:

### 1. **Inicio (`index.html`)**
   - Presentación general de Patricia Castro y sus servicios.
   - Carrusel de imágenes destacadas.
   - Beneficios de los servicios ofrecidos.
   - Enlace a las secciones de servicios y contacto.

### 2. **Sobre Mí (`pages/sobre-mi.html`)**
   - Biografía de Patricia Castro.
   - Formación académica y credenciales.
   - Enfoque terapéutico basado en técnicas como la terapia cognitivo-conductual y mindfulness.

### 3. **Servicios (`pages/servicios.html`)**
   - Descripción de los servicios ofrecidos:
     - Terapia individual.
     - Talleres temáticos.
     - Sesiones online.
   - Preguntas frecuentes sobre los servicios.

### 4. **Blog (`pages/blog.html`)**
   - Artículos sobre psicología, bienestar emocional y desarrollo personal.
   - Categorías para filtrar contenido.
   - Sección de suscripción al boletín.

### 5. **Contacto (`pages/contacto.html`)**
   - Formulario de contacto para agendar citas o solicitar información.
   - Información de contacto (email, teléfono, dirección).
   - Mapa de ubicación de la consulta.

## Estructura SCSS
El proyecto utiliza una arquitectura SCSS modular siguiendo la metodología 7-1 y BEM para nomenclatura de clases:

### Directorio SCSS
```
scss/
├── styles.scss                # Archivo principal que importa todos los componentes
├── abstracts/                 # Variables, mixins, placeholders y utilidades
│   ├── _mixins.scss           # Mixins reutilizables (hover-lift, flex-center, button-styles)
│   ├── _placeholders.scss     # Placeholders para extender estilos
│   ├── _responsive.scss       # Breakpoints y mixins para responsive design
│   └── _variables.scss        # Variables globales de colores, espaciados, etc.
├── base/
│   └── _base.scss             # Estilos base y reset
├── components/                # Componentes reutilizables
│   ├── _buttons.scss          # Estilos de botones y CTA
│   ├── _cards.scss            # Tarjetas de servicios y blog
│   ├── _carousel.scss         # Carrusel hero con optimización de selectores
│   ├── _forms.scss            # Formularios y campos de entrada
│   └── animations.scss        # Animaciones personalizadas
├── layout/                    # Elementos estructurales del sitio
│   ├── _footer.scss           # Footer del sitio
│   ├── _header.scss           # Header con navbar
│   └── _page-banner.scss      # Banner de cabecera de páginas internas
└── pages/                     # Estilos específicos de cada página
    ├── _about.scss            # Página Sobre Mí
    ├── _blog.scss             # Página de Blog
    ├── _contact.scss          # Página de Contacto
    ├── _home.scss             # Página de Inicio
    └── _services.scss         # Página de Servicios
```

## Características SCSS implementadas
- **Metodología BEM**: Block, Element, Modifier para nomenclatura de clases
- **Nesting óptimo**: Limitado a máx. 3-4 niveles con selectores avanzados
- **Selectores avanzados**: Uso de selectores de hijo directo (`>`), hermano adyacente (`+`) y hermano general (`~`)
- **Mixins reutilizables**: 
  - `hover-lift`: Efectos de elevación en hover
  - `flex-center`: Centrado con flexbox
  - `button-filled` y `button-outline`: Estilos de botones
- **Variables semánticas**: Sistema de colores, sombras, espaciados y transiciones
- **Placeholders**: Compartir estilos entre elementos con `@extend`

## Tecnologías Utilizadas
- **HTML5**: Estructura del contenido con elementos semánticos.
- **SCSS/Sass**: Preprocesador CSS con arquitectura modular y avanzada.
- **CSS3**: Estilos personalizados con enfoque en diseño responsivo y mobile-first.
- **Bootstrap 5**: Framework para componentes UI responsivos.
- **FontAwesome**: Biblioteca de iconos vectoriales.
- **JavaScript**: Funcionalidades interactivas básicas.

## Configuración del Proyecto
1. Clona este repositorio:
   ```bash
   git clone https://github.com/lautarobermudez/DesarrolloWebCoder
   ```
2. Instala las dependencias (si es necesario):
   ```bash
   npm install
   ```
3. Compila los archivos SCSS a CSS:
   ```bash
   sass --watch scss/styles.scss:css/styles-new.css
   ```
4. Abre el archivo `index.html` en tu navegador para visualizar el sitio.

## Autor
**Lautaro Bermudez**  

---

Este proyecto fue desarrollado como parte de un curso de desarrollo web en CoderHouse.
