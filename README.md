# CAR2GO – Landing Page

Landing page estática para **CAR2GO**, orientada a compra/venta/servicios de autos usados en Perú. Incluye hero con slider, secciones de servicios, planes, equipo, contacto y un **conmutador de idioma ES/EN** en la barra de navegación con paleta **amarillo/negro**.

## ✨ Características
- Hero con slider e imágenes destacadas.
- Secciones: **Servicios**, **Planes**, **Sobre nosotros**, **Equipo**, **Contacto**.
- Diseño responsive con **Bootstrap 5**.
- Accesibilidad básica (atributos `alt`, `aria-label` recomendados).


## 🧱 Estructura de carpetas
```
Landing-Page/
├─ index.html
├─ assets/
│  ├─ css/
│  │  ├─ main.css
│  │  ├─ bootstrap.css            # (revisar: si usas BS5 CDN, puedes eliminar este)
│  │  
│  ├─ js/
│  │  ├─ custom.js
│  │  ├─ bootstrap.min.js         # (revisar: v4; si usas BS5 bundle CDN, elimínalo)
│  │  ├─ jquery-1.11.0.min.js     # (revisar: obsoleto; usa jQuery 3.x sólo si es necesario)
│  │ 
│  └─ images/                      # imágenes (.jpg/.png/.webp, videos .mp4)
└─ README.md
```

> **Nota:** El proyecto incluye referencias a librerías (SliderPro, Slick, Owl). Si migras a componentes nativos de Bootstrap 5, puedes eliminar dependencias para reducir peso.

## 🚀 Requisitos y ejecución local
1. **Clonar o descomprimir** el proyecto.
2. Abre `index.html` en el navegador **o** sirve el sitio con un servidor estático:
   - Python 3:
     ```bash
     python -m http.server 8080
     # http://localhost:8080
     ```
   - Node (http-server):
     ```bash
     npm i -g http-server
     http-server -p 8080
     # http://localhost:8080
     ```

## 🧩 Accesibilidad (A11y) – Checklist rápido
- Añade `alt` **descriptivo** a todas las imágenes de contenido.
- Usa `aria-label` en botones/links icónicos.
- Mantén una jerarquía de headings correcta (un **H1** por página, luego H2/H3).
- Contraste suficiente en textos sobre imágenes (usa overlays si es necesario).

## 🔎 SEO básico
- Completa `<title>` y `<meta name="description">` (150–160 caracteres).
- Agrega Open Graph / Twitter Cards para vistas previas sociales.
- Define `<link rel="canonical" href="https://tudominio.com/">`.
- JSON-LD (`Organization`/`Website`) en `<script type="application/ld+json">`.

## 🛠️ Dependencias principales
- **Bootstrap 5 (bundle)** – componentes y utilidades responsive.
- jQuery 3.x *(solo si tus sliders/plugins lo requieren)*.
- Plugins opcionales: SliderPro, Owl Carousel, Slick, WOW.js.

> **Importante:** Evita mezclar **Bootstrap 5** con archivos locales de **Bootstrap 4** o jQuery 1.x. Dejar solo una versión evita conflictos.

## 📦 Despliegue
- **Firebase Hosting**: `firebase init` → `firebase deploy`  
- **Netlify**: arrastrar y soltar o conectar repo.  
- **GitHub Pages**: rama `gh-pages` o configuración Pages.

## 🧾 Licencia
Uso académico/educativo. Ajusta según las licencias de plantillas/recursos utilizados.

---

### Créditos y mantenimiento
Equipo CAR2GO. Para mejoras o bugs, abre un issue en el repo o contacta al responsable técnico.
