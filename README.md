# Aidan Antares — Pianista & Compositor

Web oficial de **Aidan Antares**, pianista y compositor.

## 🌐 Sitio en vivo

**https://isasimon.gitlab.io/aidanantares/**

Publicada automáticamente en GitLab Pages desde `main`.

## 📋 Contenido actual

- **Biografía** — Descripción (en construcción)
- **Vídeos** — 1 video de YouTube + 2 placeholders (en construcción)
- **Premios** — Sección de reconocimientos (en construcción)
- **Iconos** — Instagram, TikTok, Spotify, YouTube, Email
- **Botón "Escúchame"** — Enlace directo a Spotify
- **Foto de portada** — Placeholder para foto de Aidan tocando el piano

## 🛠️ Actualizar la web

### 1. Clonar el repositorio
```bash
git clone https://gitlab.com/isasimon/aidanantares.git
cd aidanantares
```

### 2. Hacer cambios
Edita los archivos en `public/index.html`:

- **Biografía:** Reemplaza el texto "En construcción" en la sección `<!-- BIOGRAFÍA -->`
- **Videos:** Cambia `VIDEO_ID_2` y `VIDEO_ID_3` por IDs reales de YouTube
- **Email:** Reemplaza `ejemplo@correo.com` en la sección `<!-- ICONOS -->`
- **Redes:** Actualiza los enlaces de Instagram, TikTok, Spotify, YouTube
- **Foto:** Guarda la foto en `fotografias/portada.png` y descomenta la línea `<img>` en la sección `<!-- HERO -->`

### 3. Publicar cambios
```bash
git add .
git commit -m "Descripción del cambio"
git push
```

**Nota:** Las credenciales se guardan localmente. La primera vez que hagas `push`, git te pide usuario/contraseña una sola vez.

## 🎨 Diseño

- **Dark mode elegante** — Tonos blancos, negros y grises
- **Tipografía moderna** — Playfair Display (títulos) + Space Grotesk (cuerpo)
- **Responsive** — Optimizado para mobile, tablet y desktop
- **Iconos animados** — Efectos hover suaves
- **Fondo de universo** — Gradiente oscuro sofisticado

## 📁 Estructura

```
aidanantares/
├── public/
│   └── index.html        ← Página principal
├── fotografias/
│   └── portada.png       ← Foto (pendiente)
├── .gitlab-ci.yml        ← Configuración de CI/CD
├── cspell.json          ← Configuración de ortografía
└── README.md            ← Este archivo
```

## 🚀 Tecnología

- **HTML5** — Estructura semántica
- **CSS3** — Estilos modernos y responsive
- **JavaScript** — Mínimo, solo para funcionalidad básica
- **Google Fonts** — Tipografía elegante
- **GitLab Pages** — Hosting automático

## ✨ Características futuras

- [ ] Agregar foto del piano
- [ ] Completar biografía
- [ ] Agregar 2 vídeos más
- [ ] Actualizar links de redes sociales
- [ ] Agregar más premios
- [ ] Posible sección de galería

---

**Última actualización:** 2026-08-16
