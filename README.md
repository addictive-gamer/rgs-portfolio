# 🐰 RabGamesStudio™ — Official Website README

> **Versión del archivo:** `rabgamesstudio_v3.html`  
> **Última actualización:** 21 de marzo de 2026  
> **Mantenido por:** RabGamesStudio™  
> **Contacto oficial:** rabbitgames0103@gmail.com  
> **Repositorio:** [github.com/addictive-gamer/rgs-portfolio](https://github.com/addictive-gamer/rgs-portfolio)  
> **Portafolio en vivo:** [addictive-gamer.github.io/rgs-portfolio/](https://addictive-gamer.github.io/rgs-portfolio/)

---

## 📑 Tabla de Contenidos

1. [Sobre RabGamesStudio](#sobre-rabgamesstudio)
2. [Sobre este archivo HTML](#sobre-este-archivo-html)
3. [Historial de versiones](#historial-de-versiones)
4. [Estructura de la web](#estructura-de-la-web)
5. [Guía para el dueño del estudio](#guía-para-el-dueño-del-estudio)
6. [Guía para usuarios / visitantes](#guía-para-usuarios--visitantes)
7. [Guía para IAs y desarrolladores](#guía-para-ias-y-desarrolladores)
8. [Assets y recursos integrados](#assets-y-recursos-integrados)
9. [Links activos en la web](#links-activos-en-la-web)
10. [Lo que falta completar](#lo-que-falta-completar)
11. [Cómo publicar en GitHub Pages / Netlify](#cómo-publicar-en-github-pages--netlify)
12. [Créditos y herramientas](#créditos-y-herramientas)

---

## 🏢 Sobre RabGamesStudio

**RabGamesStudio™** es un estudio independiente de videojuegos fundado con la misión de crear experiencias únicas, inmersivas y memorables. Se especializa principalmente en géneros de terror —psicológico, analógico y convencional— pero explora activamente otras propuestas narrativas y mecánicas.

### Identidad del estudio

| Campo | Detalle |
|---|---|
| **Nombre oficial** | RabGamesStudio™ |
| **Tipo** | Estudio indie independiente |
| **Especialidad** | Terror psicológico · Terror analógico · Narrativa indie |
| **Herramientas principales** | TurboWarp · Godot Engine |
| **Plataformas activas** | GameJolt · itch.io |
| **Plataformas futuras** | Steam |
| **Correo de prensa** | rabbitgames0103@gmail.com |

### Redes sociales

| Plataforma | URL |
|---|---|
| GameJolt | https://gamejolt.com/@RabGamesStudio |
| itch.io | https://rabgamesstudio.itch.io/ |
| YouTube | https://www.youtube.com/@RabbitGamesOficial |
| JBS_GAMES™ (colaborador) | https://gamejolt.com/@Jbs_Games |

### Colaboraciones activas

**JBS_GAMES™** (`@Jbs_Games` en GameJolt) es el principal colaborador externo del estudio. Juntos desarrollaron **The Run** y **VaultPlanet**, ambos disponibles en GameJolt.

---

## 🎮 Catálogo de juegos

### Talk to the Hand
- **Estado:** En desarrollo
- **Género:** Terror psicológico / analógico
- **Plataformas:** GameJolt, itch.io
- **Sistemas:** Windows, Linux
- **URL:** https://gamejolt.com/games/Talk-to-the-hand-RGS/1006802
- **Descripción:** La apuesta principal de RabGamesStudio. Una experiencia que desafía la percepción de la realidad del jugador mediante audio inmersivo, narrativa ramificada y lore profundo.

### His Destiny
- **Estado:** Próximamente
- **Género:** Aventura / Narrativa
- **Plataformas:** GameJolt
- **Sistemas:** Windows, Linux
- **URL:** https://gamejolt.com/games/HisDestiny-RGS/1025984
- **Descripción:** Historia de destino, sacrificio y redención. Estética minimalista monocromática con diseño visual muy distintivo.

### The Run *(colaboración)*
- **Estado:** Lanzado
- **Colaborador:** JBS_GAMES™
- **URL:** https://gamejolt.com/games/TR/1021632

### VaultPlanet *(colaboración)*
- **Estado:** Lanzado
- **Colaborador:** JBS_GAMES™
- **URL:** https://gamejolt.com/games/VP/1043581

### Zero-State: LYXA
- **Estado:** Conceptualización
- **Nota:** No se promete el mismo nivel de ambición que Talk to the Hand o His Destiny.

---

## 📄 Sobre este archivo HTML

El sitio web de RabGamesStudio está construido como un **único archivo HTML autocontenido** (`rabgamesstudio_v3.html`). No requiere servidor, base de datos, ni dependencias instaladas localmente — solo un navegador web moderno.

### Tecnologías usadas

| Tecnología | Uso |
|---|---|
| HTML5 | Estructura semántica |
| CSS3 (puro) | Estilos, animaciones, CRT effect, grid |
| JavaScript (vanilla) | Interactividad, slider, modal, FAQ |
| Google Fonts CDN | `Press Start 2P` · `Share Tech Mono` · `Rajdhani` |
| Imágenes base64 | Screenshots de His Destiny y Talk to the Hand embebidos |
| Imágenes CDN (GameJolt) | Thumbnails, avatares y banners cargados por URL |

### Requisitos para funcionar

- Navegador moderno (Chrome, Firefox, Edge, Safari 2020+)
- Conexión a internet para: Google Fonts, imágenes CDN de GameJolt
- Sin conexión: funciona parcialmente (texto, CRT, slider con placeholder, interactividad JS)

---

## 📦 Historial de versiones

| Versión | Fecha | Cambios principales |
|---|---|---|
| **v1** | 2025 | Primera versión — estructura completa, CRT, slider, secciones base |
| **v2** | 2025 | Imágenes reales integradas (base64 + CDN), links activos, logos de estudio, sección de redes sociales, modal de juegos con galería |
| **v3** | 21 mar 2026 | Popup de idioma (ES/EN) al entrar, traducción completa de 178 elementos, favicon, SVGs en lugar de emojis, sección de Equipo, políticas legales completas en modal, formulario listo para Google Sheets, link al repo y portafolio en footer |

---

## 🗂 Estructura de la web

La web es una **Single Page Application (SPA)** con scroll suave entre secciones. El orden de las secciones en la v3 es:

```
[popup de idioma]   → aparece al entrar, elige ES o EN
#home              → Hero + Slider + Preview de juegos + Blog preview
#about-home        → Resumen del estudio con avatares
#support           → Apoyanos (PayPal / Ko-fi)
#games-full        → Catálogo completo con 6 tarjetas + SVGs
#about-full        → Historia completa + Filosofía
#team              → Equipo (Rab + JBS_GAMES™ + Posición abierta)
#news-full         → Blog destacado + sidebar
#social-embeds     → Paneles de YouTube, GameJolt, itch.io, Discord
#contact           → Formulario (Google Sheets listo) + redes + FAQ
footer             → Links, plataformas, repo GitHub, portafolio, legal
[modal de juegos]  → Ficha con galería al click en TTTH o His Destiny
[modal legal]      → Políticas completas (privacidad, términos, etc.)
```

### Componentes interactivos

| Componente | Descripción |
|---|---|
| **Popup de idioma** | Aparece al cargar la página. Elige ES o EN con bandera. |
| **Toggle de idioma** | Botón en el header (🇬🇧 ENG / 🇪🇸 ESP) para cambiar en cualquier momento. |
| **Slider del hero** | Auto-avanza cada 4.8s. Flechas manuales y dots. 3 slides. |
| **Botón CRT** | Activa/desactiva efecto scanlines + aberración cromática en todo el body. |
| **Modal de juegos** | Click en Talk to the Hand o His Destiny abre ficha con galería bilingüe. |
| **Modal legal** | Click en cualquier política del footer abre el texto completo sin salir de la página. |
| **FAQ accordion** | Click en pregunta expande/colapsa la respuesta. |
| **Formulario** | Listo para conectar a Google Sheets vía Apps Script (ver guía abajo). |
| **Mouse blob** | Gradiente radial morado que sigue el cursor. |
| **Notificaciones** | Toast en esquina inferior derecha para acciones sin URL real. |
| **Menú hamburguesa** | Versión móvil del nav, desplegable. |
| **Favicon** | Logo de RabGamesStudio en la pestaña del navegador. |

---

## 🧑‍💼 Guía para el dueño del estudio

Esta sección es para **el CEO / fundador de RabGamesStudio** que mantendrá la web.

### Cómo actualizar contenido sin código

La mayoría del contenido está escrito directamente en el HTML como texto. Para actualizarlo:

1. Abre `rabgamesstudio_v2.html` con cualquier editor de texto (Notepad++, VS Code, etc.)
2. Usa `Ctrl+F` para buscar el texto que quieres cambiar
3. Edítalo directamente
4. Guarda y sube el archivo actualizado

### Dónde está cada cosa

| Quiero cambiar... | Busca en el HTML... |
|---|---|
| Entradas del blog | Busca `blog-card` — hay 3 tarjetas en home y más en `#news-full` |
| Descripción de un juego | Busca `gfc-desc` dentro del juego correspondiente |
| Correo de contacto | Busca `rabbitgames0103@gmail.com` (aparece 3 veces) |
| Links de redes sociales | Busca `href="https://gamejolt` o `href="https://rabgamesstudio` |
| Texto del About / Historia | Busca `timeline-item` — son 4 bloques |
| FAQ — preguntas y respuestas | Busca `faq-item` |
| Botones de PayPal / Ko-fi | Busca `btn-paypal` y `btn-kofi` — cambia el `href="#"` |

### Agregar un nuevo juego

1. Busca el bloque de `<!-- MÁS -->` al final de `#games-full`
2. Copia la estructura de cualquier `game-full-card` existente
3. Pega antes del bloque `<!-- MÁS -->` y rellena los datos

### Agregar una entrada de blog

1. Busca `news-mini` en la sección `#news-full`
2. Copia una de las entradas existentes
3. Cambia el emoji, título y fecha

### Activar Discord cuando esté listo

1. Busca `DISCORD` en el HTML — hay múltiples referencias
2. Reemplaza los `onclick="showNotif('DISCORD — PRÓXIMAMENTE')"` con `href="TU_LINK_DE_DISCORD" target="_blank"`
3. En la sección `#social-embeds`, quita el `style="opacity:0.6;"` del panel de Discord
4. Cambia el texto `AÚN NO DISPONIBLE` por el link real

### Activar PayPal y Ko-fi

1. Busca `btn-paypal` — cambia `href="https://paypal.com"` por tu link de donación directo
2. Busca `btn-kofi` — cambia `href="https://ko-fi.com"` por tu perfil real (ej: `https://ko-fi.com/rabgamesstudio`)

### Agregar un trailer de YouTube

En la sección `#social-embeds`, dentro del panel de YouTube, hay un `embed-placeholder`. Para poner un video real:

1. Ve al video en YouTube
2. Haz click en Compartir → Insertar → copia el `src` del iframe (formato: `https://www.youtube.com/embed/ID_DEL_VIDEO`)
3. Reemplaza el bloque `.embed-placeholder` por:
```html
<iframe class="yt-video-frame"
  src="https://www.youtube.com/embed/ID_DEL_VIDEO"
  allowfullscreen></iframe>
```

---

## 👥 Guía para usuarios / visitantes

Bienvenido al sitio oficial de **RabGamesStudio™**.

### Navegación

- El **menú superior** tiene acceso directo a todas las secciones
- En móvil, usa el **ícono de menú** (☰) en la esquina superior derecha
- El **logo** en la esquina superior izquierda te lleva al inicio

### Función CRT

El botón **CRT: OFF/ON** en la barra de navegación activa un efecto retro de monitor de tubo catódico. Es puramente visual y no afecta el contenido.

### Juegos

- Haz click en **Talk to the Hand** o **His Destiny** para ver una ficha completa con galería y links
- **The Run** y **VaultPlanet** te llevan directamente a GameJolt
- Los juegos con estado `PRÓXIMAMENTE` aún no tienen fecha de lanzamiento confirmada

### Apoyar al estudio

En la sección **Apoyanos** puedes donar mediante PayPal o Ko-fi. Cada contribución ayuda al desarrollo de los próximos juegos.

### Contacto

Usa el **formulario de contacto** para consultas generales, prensa, colaboraciones o soporte técnico. También puedes escribir directamente a `rabbitgames0103@gmail.com`.

### Reportar un bug

Selecciona **"Soporte técnico / Bug report"** en el formulario, o repórtalo directamente en la página del juego en GameJolt.

---

## 🤖 Guía para IAs y desarrolladores

Esta sección documenta la arquitectura técnica del sitio para que cualquier IA o desarrollador pueda modificarlo, extenderlo o integrarlo con precisión.

### Arquitectura general

```
rabgamesstudio_v2.html
├── <head>
│   ├── Meta tags (charset, viewport, description)
│   ├── Google Fonts (3 familias via CDN)
│   └── <style> — Todo el CSS (~650 líneas)
├── <body>
│   ├── .pixel-bg          → Fondo de cuadrícula CSS
│   ├── #mouse-blob        → Blob de cursor animado
│   ├── #notif             → Toast de notificaciones
│   ├── <header #header>   → Nav fijo
│   ├── <main>
│   │   ├── <section #home>
│   │   ├── <section #about-home>
│   │   ├── <section #support>
│   │   ├── <section #games-full>
│   │   ├── <section #about-full>
│   │   ├── <section #news-full>
│   │   ├── <section #social-embeds>
│   │   └── <section #contact>
│   ├── <footer>
│   ├── <div #gameModal>   → Modal de juego
│   └── <script>           → JS vanilla (~120 líneas)
```

### Variables CSS globales

Todas las variables de diseño están en `:root`. Modificar aquí afecta todo el sitio:

```css
--bg-deep, --bg-mid, --bg-card, --bg-hover   /* Fondos */
--border, --border-glow                       /* Bordes */
--pink, --pink-dim, --pink-glow               /* Acento principal */
--blue, --blue-dim, --blue-glow               /* Acento secundario */
--purple, --purple-dim, --purple-glow         /* Acento terciario */
--green, --yellow                             /* Estados */
--white, --muted, --muted2                    /* Texto */
--font-pixel, --font-mono, --font-body        /* Tipografías */
```

### Funciones JavaScript globales

| Función | Descripción |
|---|---|
| `selectLang(v)` | Cierra el popup y aplica el idioma elegido |
| `toggleLang()` | Alterna entre ES y EN desde el botón del header |
| `applyLang(v)` | Aplica el idioma a todos los elementos `data-i18n` y placeholders |
| `goTo(id)` | Scroll suave a sección por ID |
| `goHome()` | Alias de `goTo('home')` |
| `toggleCRT()` | Activa/desactiva clase `crt-on` en body |
| `slideMove(dir)` | Mueve slider ±1 |
| `goSlide(n)` | Va directo al slide N |
| `toggleFAQ(el)` | Toggle clase `open` en `.faq-item` |
| `showNotif(msg)` | Muestra toast en `#notif` por 3 segundos |
| `openLink(url)` | `window.open(url, '_blank')` |
| `toggleMenu()` | Despliega nav móvil |
| `openModal(id)` | Abre modal de juego con data bilingüe de `games[id]` |
| `closeModal()` | Cierra modal de juego |
| `openLegal(type)` | Abre modal legal con contenido de `LEGAL[type][lang]` |
| `closeLegal()` | Cierra modal legal |
| `submitForm()` | Envía formulario al endpoint de Google Sheets (o modo demo) |

### Objeto de datos de juegos (`games`)

```javascript
games = {
  ttth: {
    title, color, status, statusColor,
    genre, platforms, systems,
    link, linkLabel, desc,
    imgs: [banner_url, screenshot1_base64, screenshot2_base64]
  },
  hd: { ... }
}
```

Para agregar un nuevo juego al modal, agregar una entrada al objeto `games` con la misma estructura y llamar `openModal('nuevo_id')` desde el onclick de la tarjeta.

### Sistema CRT

El efecto CRT funciona exclusivamente con CSS:

```css
body.crt-on::after { /* scanlines con background repeating-linear-gradient */ }
body.crt-on { filter: contrast(1.04) brightness(0.97) saturate(1.1); }
```

No hay canvas ni WebGL — es CSS puro, liviano y funciona en todos los navegadores.

### Imágenes

| Tipo | Método | Origen |
|---|---|---|
| Thumbnails de juegos | URL directa CDN GameJolt | `m.gjcdn.net/game-thumbnail/...` |
| Avatares / logos | URL directa CDN GameJolt | `m.gjcdn.net/user-avatar/...` |
| Screenshots del modal | Base64 embebido en el HTML | Archivos `.png` locales convertidos |

Las imágenes base64 están dentro del objeto `games` en el `<script>`. Son los 4 archivos `.png` adjuntos al proyecto.

### Fuentes

```
Press Start 2P   → Títulos, pixel art, UI labels, botones
Share Tech Mono  → Código, metadata, tags, stats bars
Rajdhani         → Cuerpo de texto, descripciones, párrafos
```

Todas cargadas desde Google Fonts CDN. Si no hay conexión, el browser usa fallback `monospace` / `sans-serif`.

### Clases CSS más importantes

| Clase | Uso |
|---|---|
| `.container` | Wrapper centrado max-width 1100px |
| `.section-label` | Etiqueta rosa pequeña encima de títulos |
| `.section-title` | H2 pixel font con `<span>` rosa |
| `.btn` + modificador | Sistema de botones (primary, outline, ghost, gj, itch, yt, paypal, kofi) |
| `.tag` + modificador | Badges de estado (horror, dev, collab, soon, launched) |
| `.corner-deco` | Esquinas decorativas en tarjetas |
| `.pixel-divider` | Separador horizontal con texto central |
| `.status-bar` | Barra de estado tipo consola |
| `.game-full-card` | Grid 170px+1fr para tarjetas grandes |
| `.embed-placeholder` | Placeholder clickeable para embeds de redes |

### Responsive breakpoints

Solo hay un breakpoint en `@media (max-width: 768px)` que convierte todos los grids a `1fr` y activa el hamburger.

### Extensibilidad — Lo que se puede añadir fácilmente

- **Backend de blog:** Reemplazar tarjetas estáticas por fetch a una API (Ghost, Strapi, Contentful)
- **Formulario funcional:** Conectar el form a Formspree, Netlify Forms o EmailJS (solo cambiar el `onsubmit`)
- **Discord widget:** Usar `https://discord.com/widget?id=SERVER_ID&theme=dark` en un iframe dentro del panel de Discord
- **Steam widget:** Iframe de la página de Steam del juego cuando esté disponible
- **i18n / traducciones:** El stub de `changeLang()` está listo para conectar con un objeto de strings por idioma
- **Analytics:** Agregar Google Analytics o Plausible antes del cierre de `</head>`
- **Merch / tienda:** Sección nueva `#merch` con integración a Shopify Buy Button o Gumroad

---

## 🖼 Assets y recursos integrados

### Imágenes base64 (embebidas en el HTML)

| Variable | Archivo original | Usado en |
|---|---|---|
| `TTTH` | `Talk_To_The_Hand.png` | Modal de Talk to the Hand (slide 3) |
| `TTTH0` | `Talk_To_The_Hand0.png` | Modal de Talk to the Hand (slide 2) |
| `HD` | `His_Destiny.png` | Modal de His Destiny (slide 3) |
| `HD0` | `His_Destiny0.png` | Modal de His Destiny (slide 2) |

### Imágenes por URL CDN (requieren internet)

| Recurso | URL |
|---|---|
| Logo RabGamesStudio | `https://m.gjcdn.net/user-avatar/200/11291402-crop0_7_695_702-sxnh9aum-v4.webp` |
| Logo JBS_GAMES™ | `https://m.gjcdn.net/user-avatar/200/8296794-crop372_138_811_577-ggcsk7b6-v4.webp` |
| Banner Talk to the Hand | `https://m.gjcdn.net/game-thumbnail/500/1006802-crop0_0_1149_646-k8fexezw-v4.webp` |
| Banner His Destiny | `https://m.gjcdn.net/game-thumbnail/500/1025984-crop0_104_1103_725-twvfcufw-v4.webp` |

> ⚠️ **Nota:** Las URLs de GameJolt CDN pueden cambiar o expirar. Si las imágenes dejan de cargar, actualiza las URLs desde los perfiles de GameJolt o sube las imágenes a tu propio hosting.

---

## 🔗 Links activos en la web

| Destino | URL | Secciones donde aparece |
|---|---|---|
| GameJolt RabGamesStudio | https://gamejolt.com/@RabGamesStudio | Header, About, News, Contact, Footer, Embeds |
| itch.io | https://rabgamesstudio.itch.io/ | Hero, About, Contact, Footer, Embeds |
| YouTube | https://www.youtube.com/@RabbitGamesOficial | News sidebar, Contact, Footer, Embeds |
| GameJolt JBS_GAMES™ | https://gamejolt.com/@Jbs_Games | News sidebar, Contact, Footer, Embeds |
| Talk to the Hand (GJ) | https://gamejolt.com/games/Talk-to-the-hand-RGS/1006802 | Modal + tarjeta |
| His Destiny (GJ) | https://gamejolt.com/games/HisDestiny-RGS/1025984 | Modal + tarjeta |
| The Run (GJ) | https://gamejolt.com/games/TR/1021632 | Tarjeta |
| VaultPlanet (GJ) | https://gamejolt.com/games/VP/1043581 | Tarjeta |
| Email prensa | mailto:rabbitgames0103@gmail.com | Contact, Footer |
| PayPal | https://paypal.com *(placeholder)* | Support |
| Ko-fi | https://ko-fi.com *(placeholder)* | Support |

---

## ⏳ Lo que falta completar

Estas son las partes marcadas como `PRÓXIMAMENTE` o con placeholders en la v3 actual:

| Pendiente | Dónde en el HTML | Acción necesaria |
|---|---|---|
| Link real de PayPal | `btn-paypal` en `#support` | Cambiar `href` al link de donación directo |
| Link real de Ko-fi | `btn-kofi` en `#support` | Cambiar `href` a tu perfil de Ko-fi |
| Servidor de Discord | Panel Discord en `#social-embeds` | Agregar link de invitación + quitar `opacity:.6` |
| Trailers de YouTube | Panel YouTube en `#social-embeds` | Reemplazar placeholder por `<iframe>` con video ID |
| URL de Google Sheets | `const SHEET_URL = 'YOUR_APPS_SCRIPT_URL_HERE'` | Seguir la guía de Apps Script abajo |
| Entradas reales de blog | `#news-full` | Reemplazar textos placeholder con posts reales |
| Sección de Merch | No implementada | Crear cuando el merch esté listo |
| Página de Zero-State: LYXA | Tarjeta en `#games-full` | Agregar link cuando exista la página en GameJolt |
| Foto real de Rab | Tarjeta equipo en `#team` | Reemplazar avatar CDN por imagen personalizada |

### 📊 Cómo conectar el formulario a Google Sheets

1. Crea una Google Sheet nueva en [sheets.google.com](https://sheets.google.com)
2. Ve a **Extensiones → Apps Script** y pega este código:

```javascript
function doPost(e) {
  var sheet = SpreadsheetApp.getActiveSpreadsheet().getActiveSheet();
  var data = JSON.parse(e.postData.contents);
  sheet.appendRow([data.date, data.name, data.email, data.type, data.message, data.lang]);
  return ContentService.createTextOutput('OK');
}
```

3. Guarda con `Ctrl+S`
4. Click en **Implementar → Nueva implementación**
5. Tipo: **Aplicación web** — Acceso: **Cualquier persona**
6. Copia la URL generada
7. En el HTML busca `YOUR_APPS_SCRIPT_URL_HERE` y reemplázala con esa URL

Cada envío del formulario agrega una fila con: **fecha · nombre · email · tipo · mensaje · idioma**.

---

## 🚀 Cómo publicar en GitHub Pages / Netlify

### GitHub Pages

1. Crea un repositorio en GitHub (puede ser privado o público)
2. Renombra el archivo a `index.html`
3. Súbelo al repo
4. Ve a **Settings → Pages → Source → main branch / root**
5. Tu web estará en `https://TU_USUARIO.github.io/NOMBRE_DEL_REPO/`

Para un dominio personalizado: agrega un archivo `CNAME` con tu dominio y configura los DNS.

### Netlify (recomendado — más fácil)

1. Ve a https://netlify.com y crea una cuenta gratuita
2. Arrastra y suelta el archivo `index.html` en el dashboard
3. Netlify lo publica instantáneamente con una URL aleatoria
4. En **Site Settings → Domain Management** puedes conectar tu dominio propio

### Estructura de archivos recomendada para el repo

```
/
├── index.html          ← el archivo principal (renombrado)
├── README.md           ← este archivo
└── assets/             ← (opcional) si decides sacar las imágenes del base64
    ├── images/
    │   ├── ttth_banner.png
    │   ├── hd_banner.png
    │   └── ...
    └── fonts/          ← (opcional) si quieres fuentes locales offline
```

---

## 🛠 Créditos y herramientas

| Elemento | Crédito |
|---|---|
| Diseño y desarrollo web | Claude (Anthropic) — Generado para RabGamesStudio™ |
| Arte de juegos | RabGamesStudio™ |
| Arte de colaboraciones | RabGamesStudio™ × JBS_GAMES™ |
| Fuente "Press Start 2P" | CodeMan38 — Google Fonts (OFL) |
| Fuente "Share Tech Mono" | Carrois Apostrophe — Google Fonts (OFL) |
| Fuente "Rajdhani" | Indian Type Foundry — Google Fonts (OFL) |
| Imágenes CDN | GameJolt CDN (m.gjcdn.net) |
| Iconos | SVGs inline personalizados (sin dependencias externas) |
| Hosting sugerido | GitHub Pages / Netlify |
| Repositorio | [github.com/addictive-gamer/rgs-portfolio](https://github.com/addictive-gamer/rgs-portfolio) |
| Portafolio en vivo | [addictive-gamer.github.io/rgs-portfolio/](https://addictive-gamer.github.io/rgs-portfolio/) |

---

## 📝 Notas finales

- La v3 pesa aproximadamente **491 KB** gracias a las imágenes base64 embebidas.
- Las URLs de GameJolt CDN son estables pero no están bajo control del estudio. Si el CDN cambia, actualiza las URLs desde los perfiles de GameJolt.
- El sistema de idiomas cubre **178 elementos** — absolutamente todo el texto de la web cambia al alternar entre ES y EN.
- Las políticas legales (privacidad, términos, reembolso, etc.) están integradas como modales — no requieren páginas separadas.
- El CRT effect es una característica de identidad de RabGamesStudio. No eliminar.

---

*README generado para RabGamesStudio™ · 21 de marzo de 2026 · Todos los derechos reservados.*  
*"No seguimos tendencias — creamos las nuestras."*
