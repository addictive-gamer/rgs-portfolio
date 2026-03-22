# 🐰 RabGamesStudio™ — Official Website README

> **Versión del sitio:** `v4.19`
> **Última actualización:** 21 de marzo de 2026
> **Mantenido por:** RabGamesStudio™ — Xata Jr. (Admin Web)
> **Contacto oficial:** rabbitgames0103@gmail.com
> **Repositorio:** [github.com/addictive-gamer/rgs-portfolio](https://github.com/addictive-gamer/rgs-portfolio)
> **Portafolio en vivo:** [addictive-gamer.github.io/rgs-portfolio/](https://addictive-gamer.github.io/rgs-portfolio/)

![version](https://img.shields.io/badge/version-4.19-ff2d78?style=for-the-badge)
![host](https://img.shields.io/badge/Hosted_by-GitHub_Pages-black?style=for-the-badge&logo=github)
![lang](https://img.shields.io/badge/Bilingüe-ES%20%7C%20EN-b347ff?style=for-the-badge)
![worker](https://img.shields.io/badge/Backend-Cloudflare_Worker_v3.0-orange?style=for-the-badge&logo=cloudflare)
![crt](https://img.shields.io/badge/Feature-CRT_Mode-00d4ff?style=for-the-badge)

---

## 📑 Tabla de Contenidos

1. [Sobre RabGamesStudio](#sobre-rabgamesstudio)
2. [Equipo actual](#equipo-actual)
3. [Catálogo de juegos](#catálogo-de-juegos)
4. [Redes sociales y estudios aliados](#redes-sociales-y-estudios-aliados)
5. [Sobre el archivo HTML](#sobre-el-archivo-html)
6. [Features completas](#features-completas)
7. [Formulario de Contacto → Cloudflare Worker](#formulario-de-contacto--cloudflare-worker)
8. [Arquitectura técnica para IAs y desarrolladores](#arquitectura-técnica-para-ias-y-desarrolladores)
9. [Guía para el dueño del estudio](#guía-para-el-dueño-del-estudio)
10. [Assets y recursos integrados](#assets-y-recursos-integrados)
11. [Historial de versiones](#historial-de-versiones)
12. [Cómo publicar en GitHub Pages / Netlify](#cómo-publicar-en-github-pages--netlify)
13. [Créditos y herramientas](#créditos-y-herramientas)

---

## 🏢 Sobre RabGamesStudio

**RabGamesStudio™** es un estudio independiente de videojuegos fundado con la misión de crear experiencias únicas, inmersivas y memorables. Se especializa en terror —psicológico, analógico y convencional— pero explora activamente otras propuestas narrativas y mecánicas.

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
| **Eslogan** | "No seguimos tendencias — creamos las nuestras." |

---

## 👥 Equipo Actual

| Nombre | Rol | Notas |
|---|---|---|
| **Rab** | Fundador & CEO / Director | Visión creativa, narrativa, desarrollo. 15 años. |
| **Skellent** | Programador | Desarrollo técnico de los proyectos |
| **LouArtStuff** | Diseñadora Gráfica | Identidad visual y arte del estudio |
| **Silly** | Voice Actor (VA) | Actor de doblaje para personajes |
| **Xata Jr.** (a.k.a. Addictive Gamer) | Ilustrador & Sprite Artist + Admin Web | Administrador del repositorio y sitio web |
| **JBS_GAMES™** | Colaborador & Aliado externo | Desarrollo de The Run y VaultPlanet |

---

## 🎮 Catálogo de Juegos

### Talk to the Hand
- **Estado:** En desarrollo 🔧 · **Género:** Terror psicológico / analógico
- **Plataformas:** GameJolt · itch.io · Windows · Linux
- **URL:** https://gamejolt.com/games/Talk-to-the-hand-RGS/1006802

### His Destiny
- **Estado:** Próximamente 🔜 · **Género:** Aventura / Narrativa
- **Plataformas:** GameJolt · Windows · Linux
- **URL:** https://gamejolt.com/games/HisDestiny-RGS/1025984

### The Run *(colaboración con JBS_GAMES™)*
- **Estado:** Lanzado ✅ — https://gamejolt.com/games/TR/1021632

### VaultPlanet *(colaboración con JBS_GAMES™)*
- **Estado:** Lanzado ✅ — https://gamejolt.com/games/VP/1043581

### Zero-State: LYXA
- **Estado:** Conceptualización 💭

---

## 🌐 Redes Sociales y Estudios Aliados

| Plataforma | URL |
|---|---|
| GameJolt | https://gamejolt.com/@RabGamesStudio |
| itch.io | https://rabgamesstudio.itch.io/ |
| YouTube | https://www.youtube.com/@RabbitGamesOficial |
| Discord | Próximamente |

### Estudios Aliados (`#allied-studios`)

| Estudio | GameJolt |
|---|---|
| **Rewite Pictures** | https://gamejolt.com/@RewitePictures |
| **ZAYgt** | https://gamejolt.com/@ZAYgt |
| **Nightmare Labs** | https://gamejolt.com/@NightmareLabs |
| **Reptile Games** | https://gamejolt.com/@ReptileGames |
| **JBS_GAMES™** | https://gamejolt.com/@Jbs_Games |

---

## 📄 Sobre el Archivo HTML

El sitio es un **único archivo HTML autocontenido** (`index.html`). Sin servidor, sin base de datos, sin dependencias instaladas.

| Tecnología | Uso |
|---|---|
| HTML5 + CSS3 + JS vanilla | Todo el sitio — sin frameworks ni bundlers |
| Google Fonts CDN | Press Start 2P · Share Tech Mono · Rajdhani |
| Imágenes base64 | Screenshots de juegos embebidos directamente en JS |
| Imágenes CDN (GameJolt) | Thumbnails, avatares y banners por URL |
| Cloudflare Worker v3.0 | Backend del formulario (email + Discord DM) |

**Peso:** ~540 KB (incluye imágenes base64, sistema bilingüe completo, CRT)

---

## ✨ Features Completas

### 🌐 Sistema Bilingüe (ES/EN)
- **178+ elementos** traducidos — absolutamente todo el texto cambia al alternar idioma
- Pop-up de idioma al cargar (`#lang-popup`) con fix de `pointer-events` y `z-index: 99999`
- Toggle en el header (`🇬🇧 ENG` / `🇪🇸 ESP`) disponible siempre
- Implementado con `T = { es: {...}, en: {...} }` y función `applyLang(v)`

### 🕹️ CRT Effect
- Botón **CRT: OFF / ON** en el header activa/desactiva el modo retro
- CSS puro: `body::before` (scanlines) + `body::after` (viñeta) + `animation: crt-flicker`
- Al activar: cursor personalizado fade-out (0.4s) · Al desactivar: fade-in

### 🖱️ Cursor Personalizado
- Punto rosa 8px con `z-index: 999999` — por encima de todos los overlays
- Hover: escala 1.6x en morado · Click: comprime · Fade suave con CRT

### 🎞️ Slider del Hero
- 3 slides con auto-avance cada 4.8 segundos
- Flechas manuales + dots de navegación · Contenido bilingüe

### 🎮 Modal de Juegos
- Galería de 3 imágenes · descripción bilingüe · género · estado · link GameJolt

### ⚖️ Políticas Legales
- 5 políticas en modales: Privacidad · T&C · Accesibilidad · Envío · Reembolso

### 🚪 Exit Popup
- Intercepta todos los links `http/https` externos
- Modal con URL destino antes de salir · Bilingüe

### 🔔 Toast de Notificaciones
- Toast en esquina inferior derecha · se autocierra en 3 segundos

### 📬 Formulario con contador de caracteres
- Ver sección dedicada más abajo

---

## 📬 Formulario de Contacto → Cloudflare Worker

### Flujo de envío

```
Usuario llena formulario
       ↓
FormData enviado a Cloudflare Worker (POST)
  con campo source="rab"  ← fd.append explícito en JS
       ↓
Worker identifica fuente → config RabGamesStudio
       ↓
Worker envía en paralelo:
  ├── 📧 Email HTML vía Resend → 4 destinatarios
  │     · Adjuntos como body.attachments
  │     · Info sensible en sección amarilla
  └── 💬 Discord DM (bot) → IDs configurados
        · Intento 1: embed Discohook
        · Fallback: markdown enriquecido si DM de bot
        · Adjuntos: embeds SPOILER_ con imagen inline
        · Info sensible: ||spoiler|| al click
```

### Campos del formulario

| ID | `name` | Tipo | Límite | Notas |
|---|---|---|---|---|
| `#f_name` | `name` | text | **80** | Requerido |
| `#f_email` | `email` | email | **254** | Requerido · RFC 5321 |
| `#f_social` | `social` | text | **60** | Opcional — nick/usuario |
| `#f_platform` | `socialPlatform` | select | — | Requerido si `social ≠ ""` |
| `#f_type` | `reason` | select | — | Tipo de consulta |
| `#f_msg` | `message` | textarea | **2000** | Requerido · límite Discord |
| `#f_attach` | `attachment` | file | image/* | Opcional · múltiples |
| `#f_sensitive` | `sensitiveInfo` | textarea | **500** | Opcional · spoiler Discord |
| *(hidden)* | `source` | — | — | `"rab"` hardcoded |

### Indicador de caracteres restantes

Todos los campos de texto tienen un contador `restantes / máximo` a la derecha debajo del input:

| Nivel | Color | Condición | Animación |
|---|---|---|---|
| Normal | Gris muted | > 50 restantes | — |
| Advertencia | 🟡 Amarillo (`--yellow`) | ≤ 50 | `counter-pulse` |
| Peligro | 🟠 Naranja (`#ff9500`) | ≤ 20 | `counter-pulse` |
| Límite | 🔴 Rosa (`--pink`) + negrita | ≤ 0 | `counter-shake` + borde rojo en input |

El `maxlength` en HTML bloquea el teclado. La validación JS en `submitForm()` bloquea el fetch si algún campo supera el límite (segunda línea de defensa). Ambos se resetean al enviar con éxito.

### Campo de información sensible

Visible siempre (no se oculta). Diseño con borde y fondo amarillo tenue, ícono 🔐 y franja superior degradada. Disclaimer de privacidad bilingüe encima del textarea.

- **Discord (embed):** campo `🔐 Información sensible` con valor `||contenido||` — blur hasta click
- **Discord (markdown fallback):** bloque `> 🔐 **INFORMACIÓN SENSIBLE:**` + `|| contenido ||`
- **Email:** sección con fondo amarillo tenue etiquetada "Información sensible"

### Embeds de Discord (estilo Discohook)

```
content: 🎮 Nuevo mensaje en RabGamesStudio

[EMBED]
 author: 🖼 RabGamesStudio · Formulario de contacto
 title:  👤 Nombre del remitente
 color:  #e91e8c (rosa RGS)
 fields:
   📧 Correo          [inline]
   🌐 Red social      [inline]  ← solo si se proporcionó
   ␣ spacer           [inline]
   🎯 Motivo          [full]
   💬 Mensaje         [full]
   🔐 Info sensible   [full]  ← ||spoiler|| si se proporcionó
   📎 Adjuntos        [full]  ← solo si los hay
 footer: RabGamesStudio · favicon
 timestamp: <t:UNIX:f>  ← localizado al timezone del receptor
```

Adjuntos (por cada imagen):
```
[EMBED]
 author: 📎 Adjunto N/TOTAL — nombre.ext · favicon
 description: > Haz click para revelar (spoiler activo)
 image: attachment://SPOILER_adjunto_N_nombre.ext   ← inline + blur
 footer: RabGamesStudio · <t:UNIX:R>
```

### Configuración del Worker (Cloudflare Secrets)

| Secret | Valor |
|---|---|
| `DISCORD_BOT_TOKEN` | Token del bot de Discord |
| `RESEND_API_KEY_RAB` | API key de Resend para RabGamesStudio |
| `RAB_DISCORD_ID_1` | `920017830605361232` (Addictive Gamer) |
| `RAB_DISCORD_ID_2` | vacío o `blank` |
| `RAB_DISCORD_ID_3` | vacío o `blank` |

> Los secrets vacíos o con valor `blank` son filtrados automáticamente por el Worker — no causan errores.

---

## 🤖 Arquitectura Técnica para IAs y Desarrolladores

### Estructura del archivo

```
index.html
├── <head>
│   ├── Meta tags SEO · OG completo · Twitter Card · theme-color #ff2d78
│   ├── Google Fonts CDN
│   └── <style>  ~900 líneas
│       ├── :root — design tokens
│       ├── CRT effect
│       ├── Cursor personalizado
│       ├── .char-counter · .field-counter-wrap · .field-over
│       ├── .sensitive-field · .sensitive-disclaimer
│       ├── Header · Hero · Slider · Secciones · Modales
│       └── Responsive 768px / 480px / 430px
├── <body>
│   ├── .pixel-bg · #mouse-blob · #cursor-dot · #notif
│   ├── <header> — nav fijo · CRT btn · lang toggle · hamburger
│   ├── <main>
│   │   ├── #home · #about-home · #support · #games-full
│   │   ├── #about-full · #team · #allied-studios · #news-full
│   │   ├── #social-embeds · #contact
│   ├── <footer>
│   ├── #gameModal · #legalModal · #exit-popup · #lang-popup
│   └── <script>  ~650 líneas
│       ├── const VERSION = 'v4.19'
│       ├── const IMG = {...}          ← base64 de imágenes
│       ├── const T = { es, en }       ← 180+ cadenas bilingües
│       ├── const games = { ttth, hd } ← datos + base64
│       ├── const LEGAL = {...}        ← 5 políticas × 2 idiomas
│       ├── updateCharCounter(el,max)  ← contador de caracteres
│       ├── submitForm()               ← valida + envía al Worker
│       └── ...resto de funciones
```

### Variables CSS Globales

```css
:root {
  --bg-deep: #0a0a0f;  --bg-mid: #0f0f1a;
  --bg-card: #13131f;  --bg-hover: #1a1a2e;
  --border: #1e1e35;
  --pink: #ff2d78;     --pink-dim: #c4215a;   --pink-glow: rgba(255,45,120,0.35);
  --blue: #00d4ff;     --blue-dim: #0099bb;   --blue-glow: rgba(0,212,255,0.30);
  --purple: #b347ff;   --purple-dim: #8230cc; --purple-glow: rgba(179,71,255,0.30);
  --green: #39ff14;    --yellow: #ffe600;
  --white: #e8e8f0;    --muted: #6a6a8a;      --muted2: #4a4a65;
  --fp: 'Press Start 2P', monospace;
  --fm: 'Share Tech Mono', monospace;
  --fb: 'Rajdhani', sans-serif;
}
```

### Funciones JavaScript

| Función | Descripción |
|---|---|
| `selectLang(v)` | Cierra popup · aplica idioma · muestra cursor |
| `toggleLang()` | Alterna ES ↔ EN |
| `applyLang(v)` | Aplica traducciones a `[data-i18n]` y `[data-i18n-ph]` |
| `updateCharCounter(el, max)` | Contador de chars con estados visual y animaciones |
| `updateSocialPlatformVisibility()` | Muestra/oculta `#f_platform_row` |
| `submitForm()` | Valida límites de chars + envía FormData al Worker |
| `goTo(id)` · `goHome()` | Scroll suave a sección |
| `toggleCRT()` | Activa/desactiva `crt-on` en body |
| `slideMove(dir)` · `goSlide(n)` | Control del slider |
| `toggleFAQ(el)` | Toggle `.open` en `.faq-item` |
| `showNotif(msg)` | Toast 3 segundos en `#notif` |
| `openLink(url)` | Exit popup |
| `toggleMenu()` | Nav hamburguesa móvil |
| `openModal(id)` · `closeModal()` | Modal de juego |
| `openLegal(type)` · `closeLegal()` | Modal legal |
| `interceptLinks()` | Listeners en links externos (se re-llama al cambiar idioma) |

### Responsive Breakpoints

| Breakpoint | Cambios principales |
|---|---|
| `768px` | Nav hamburguesa · grids 1 columna · botones apilados · footer centrado |
| `480px` | Team grid 1col · status bar apilada · tipografías reducidas |
| `430px` | Optimizado para Android moderno ~393px CSS |

---

## 🗂️ Guía para el Dueño del Estudio

**Cambiar versión:** solo `const VERSION = 'vX.XX'` — el footer se actualiza automáticamente.

**Añadir juego:** entrada en `const games`, card en `#games-full`, traducciones en `T.es` / `T.en`.

**Cambiar destinatarios del email:** en `worker-unified.js` → `buildSources(env)` → `rab.to[]`.

**Añadir ID de Discord:** en Cloudflare Secrets → `RAB_DISCORD_ID_2` o `RAB_DISCORD_ID_3`.

---

## 📦 Assets y Recursos Integrados

| Asset | Fuente |
|---|---|
| Avatar RabGamesStudio | GameJolt CDN (URL externa) |
| Thumbnails TTTH / His Destiny | GameJolt CDN (URL externa) |
| Screenshots de juegos | base64 inline en JS |
| Favicon | `favicon.png` en raíz del repo |
| Favicon en embeds Discord | `https://raw.githubusercontent.com/addictive-gamer/rgs-portfolio/refs/heads/main/favicon.png` |

---

## 📋 Historial de Versiones

### v4.19 — Contador de caracteres (21 mar 2026)

**➕ Añadido**
- Contador `restantes / máximo` en todos los campos de texto del formulario
- 4 estados: normal → 🟡 amarillo (≤50) → 🟠 naranja (≤20) → 🔴 rojo+shake (≤0)
- `maxlength` en HTML + validación JS secundaria en `submitForm()`
- Función reutilizable `updateCharCounter(el, max)`
- Reset automático al enviar exitosamente
- Límites: nombre 80 · correo 254 · nick 60 · mensaje 2000 · sensible 500

---

### v4.18 — Campo de información sensible (21 mar 2026)

**➕ Añadido**
- Campo `// INFORMACIÓN SENSIBLE` opcional con diseño amarillo + ícono 🔐
- Disclaimer de privacidad bilingüe
- Discord: `||spoiler||` en embed y markdown · Email: sección amarilla tenue

---

### v4.17 — Worker v2.0 · Discohook · thumbnails (21 mar 2026)

- Embeds estilo Discohook con `author`, `title`, `footer` + favicon correcto por fuente
- Fix popup idioma: `pointer-events: all` + `z-index: 99999`
- Timestamps nativos `<t:UNIX:f>` · adjuntos `SPOILER_` · base64 chunked

---

### v4.16 — Fix popup idioma + adjuntos Discord (21 mar 2026)

- Fix pointer-events popup idioma
- Adjuntos Discord: embed inline con `attachment://SPOILER_...`

---

### v4.15 → v4.0

Ver historial completo en el repositorio.

---

## 🚀 Cómo publicar en GitHub Pages / Netlify

### GitHub Pages (método actual)

1. Repositorio con `index.html` en la raíz
2. **Settings → Pages → Deploy from branch → main / root**
3. URL: `https://addictive-gamer.github.io/rgs-portfolio/`

### Conectar el Cloudflare Worker

1. [workers.cloudflare.com](https://workers.cloudflare.com) → nuevo Worker
2. Pegar `worker-unified.js`
3. **Settings → Variables and Secrets** → todos los secrets de la tabla
4. `WORKER_URL` en `index.html` ya apunta a `https://xata-portfolio-bot.addictivegamer.workers.dev/`

---

## 🛠 Créditos y Herramientas

| Elemento | Crédito |
|---|---|
| Diseño y desarrollo web | **Claude** (Anthropic) |
| Arte de juegos e identidad | RabGamesStudio™ |
| Ilustración & Sprites | Xata Jr. (Addictive Gamer) |
| Fuentes | Google Fonts (OFL) |
| Emails | **Resend** |
| Backend | **Cloudflare Worker v3.0** |
| Hosting | **GitHub Pages** |
| Admin repo & web | **Xata Jr.** |

---

> ⚠️ **CRÍTICO al editar manualmente:** No borrar `</style></head><body>`. Si la página se pone negra, ese es el primer lugar donde buscar.

*"No seguimos tendencias — creamos las nuestras." — RabGamesStudio™ · 2026*
