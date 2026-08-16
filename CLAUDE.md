# Aidan Antares — Guía de Desarrollo Web

## 📋 Información del Proyecto

- **Tipo:** Sitio web estático (HTML, CSS, JavaScript)
- **Propósito:** Portfolio de pianista & compositor
- **Stack:** HTML5, CSS3, JavaScript vanilla (sin frameworks)
- **Hosting:** GitHub Pages
- **URL:** https://isabelsimonalonso.github.io/aidan/

## 🎨 Características Principales

- ✓ Favicon de piano
- ✓ Sistema bilingüe (ES/EN)
- ✓ Responsive design (mobile-first)
- ✓ Traducciones dinámicas
- ✓ Videos embebidos de YouTube
- ✓ Links a redes sociales
- ✓ Tema oscuro elegante

## 📐 Arquitectura

### Estructura
```
index.html          → Único archivo HTML (monolítico)
.claude/           → Configuración del proyecto
  skills/          → Skills personalizadas para desarrollo
.vscode/           → Configuración VS Code
fotografias/       → Imágenes del sitio
```

### HTML
- Estructura semántica: header, main, footer
- Una sección principal por tema
- Atributos `data-i18n` para traducción

### CSS
- Variables CSS para colores y espaciado
- Mobile-first responsive
- Animaciones suaves con transitions
- Grid/flexbox para layouts

### JavaScript
- Traducción dinámica con localStorage
- Event listeners para botones de idioma
- Sin dependencias externas

## 🌐 Sistema de Traducción

### Cómo funciona
1. Elementos con `data-i18n="key"` se traducen automáticamente
2. Objeto `translations` en el script contiene pares clave-valor
3. localStorage guarda idioma seleccionado
4. Por defecto: español

### Agregar traducción nueva
```javascript
translations.es["new.key"] = "Texto en español";
translations.en["new.key"] = "Text in English";
```

```html
<element data-i18n="new.key">Texto en español</element>
```

## 🚀 Flujo de Desarrollo

### Para cambios pequeños
```bash
1. Editar index.html
2. ! /quality-check     (verifica código)
3. ! /web-test          (prueba en navegador)
4. git commit & push
```

### Para nuevas secciones
```bash
1. ! /web-generator    (genera componente HTML/CSS)
2. ! /design-review    (mejora visual)
3. Integrar en index.html
4. Agregar traducciones
5. ! /web-test         (prueba)
6. ! /pre-deploy       (checklist)
7. git push
```

### Antes de deployar
```bash
! /pre-deploy
```

## 📱 Responsive Design

### Breakpoints
- **Desktop:** > 768px (encabezado con banderas, header normal)
- **Mobile:** ≤ 768px (banderas en footer)

### Prueba responsiva
- Abre DevTools (F12)
- Toggle device toolbar (Ctrl+Shift+M)
- Prueba todas las características en móvil

## 🎯 Convenciones

### HTML
- IDs en camelCase: `heroFrame`, `year`
- Classes en kebab-case: `section-title`, `social-link`
- Estructura semántica: `<section>`, `<header>`, `<footer>`
- Atributos traducibles: `data-i18n="sección.clave"`

### CSS
- Variables en `--kebab-case`: `--dark`, `--accent`
- Selectores simples y específicos
- Mobile-first, luego media queries
- Comentarios para secciones grandes

### JavaScript
- Usa `const` (no var)
- Nombres descriptivos: `setLanguage()`, `translations`
- Sin console.log en producción
- Event delegation donde aplica

## 🔧 Herramientas Disponibles

### Locales
```bash
npm run format      # Prettier formatea código
npm run lint        # ESLint verifica JavaScript
npm run lint:css    # Stylelint verifica CSS
```

### Skills
- `! /web-generator` - Genera componentes
- `! /design-review` - Revisa diseño
- `! /web-test` - Prueba en navegador
- `! /quality-check` - Control de calidad
- `! /web-audit` - Audita SEO/a11y
- `! /pre-deploy` - Checklist final
- `! /code-review` - Revisa cambios

## 📝 Agregar Nueva Sección

### Pasos
1. Generar con `! /web-generator`
2. Copiar HTML al index.html en lugar correcto
3. Agregar traducciones al objeto `translations`
4. Verificar styling y responsive con `! /design-review`
5. Probar con `! /web-test`
6. Hacer commit describiendo el cambio

### Orden de secciones (actual)
1. Hero
2. Biografía
3. Premios
4. Últimas actuaciones
5. Social links
6. Footer

## 🎵 Personalizaciones Frecuentes

### Cambiar colores
Edita variables CSS en `:root`:
```css
--dark: #0f0f0f;
--accent: #d4d4d4;
```

### Agregar redes sociales
Copia un `.social-link` y actualiza href, aria-label y SVG.

### Cambiar videos/imágenes
- Videos: actualiza src en iframe
- Imágenes: coloca en `fotografias/` y actualiza src

### Agregar nueva traducción
1. Agrega clave a ambas versiones en `translations`
2. Agrega `data-i18n` al elemento HTML

## 🚨 Errores Comunes

| Error | Solución |
|-------|----------|
| Traducción no funciona | Verifica `data-i18n` exacto en HTML y JS |
| Imagen no carga | Verifica ruta: `./fotografias/archivo.png` |
| Estilos rotos | Abre DevTools, busca errores de CSS |
| Botón no funciona | Verifica clase `.lang-btn` y `data-lang` |

## 📊 Performance

- ✓ Sin frameworks externos
- ✓ CSS inline (una carga)
- ✓ Imágenes optimizadas
- ✓ Fuentes Google Fonts (preconect)
- ✓ JavaScript vanilla
- ✓ Lighthouse score ~95+

## 🔐 Seguridad

- ✓ Sin dependencias npm de terceros
- ✓ Sin eval() o innerHTML inseguro
- ✓ CSP compatible
- ✓ Links con `rel="noopener"`
- ✓ Atributos alt en imágenes

## 📚 Referencias Útiles

- [MDN HTML Semántico](https://developer.mozilla.org/es/docs/Glossary/Semantics)
- [CSS Grid & Flexbox](https://developer.mozilla.org/es/docs/Web/CSS)
- [JavaScript vanilla](https://developer.mozilla.org/es/docs/Web/JavaScript)
- [GitHub Pages](https://pages.github.com/)

## 🤝 Contacto & Mantenimiento

- **Propietario:** Isabel Simon (isabel.simon@zataca.com)
- **Última actualización:** 2026-08-16
- **Próximas mejoras:** [Agregar según necesidad]
