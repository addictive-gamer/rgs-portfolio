# 🐰 RabGamesStudio™ — Official Website README

> **Versión del sitio:** `v4.21`
> **Última actualización:** 21 de marzo de 2026
> **Mantenido por:** RabGamesStudio™ — Xata Jr. (Admin Web)
> **Contacto oficial:** rabbitgames0103@gmail.com
> **Repositorio:** [github.com/addictive-gamer/rgs-portfolio](https://github.com/addictive-gamer/rgs-portfolio)
> **Portafolio en vivo:** [addictive-gamer.github.io/rgs-portfolio/](https://addictive-gamer.github.io/rgs-portfolio/)

![version](https://img.shields.io/badge/version-4.21-ff2d78?style=for-the-badge)
![host](https://img.shields.io/badge/Hosted_by-GitHub_Pages-black?style=for-the-badge&logo=github)
![lang](https://img.shields.io/badge/Bilingüe-ES%20%7C%20EN-b347ff?style=for-the-badge)
![worker](https://img.shields.io/badge/Backend-Cloudflare_Worker_v4.0-orange?style=for-the-badge&logo=cloudflare)
![mobile](https://img.shields.io/badge/Mobile-Optimizado-39ff14?style=for-the-badge)
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
8. [Arquitectura técnica](#arquitectura-técnica-para-ias-y-desarrolladores)
9. [Guía para el dueño del estudio](#guía-para-el-dueño-del-estudio)
10. [Assets y recursos integrados](#assets-y-recursos-integrados)
11. [Historial de versiones](#historial-de-versiones)
12. [Cómo publicar](#cómo-publicar-en-github-pages--netlify)
13. [Créditos](#créditos-y-herramientas)

---

## 🏢 Sobre RabGamesStudio

**RabGamesStudio™** es un estudio independiente de videojuegos fundado con la misión de crear experiencias únicas, inmersivas y memorables.

| Campo | Detalle |
|---|---|
| **Nombre oficial** | RabGamesStudio™ |
| **Tipo** | Estudio indie independiente |
| **Especialidad** | Terror psicológico · Terror analógico · Narrativa indie |
| **Herramientas** | TurboWarp · Godot Engine |
| **Plataformas activas** | GameJolt · itch.io |
| **Plataformas futuras** | Steam |
| **Correo de prensa** | rabbitgames0103@gmail.com |
| **Eslogan** | "No seguimos tendencias — creamos las nuestras." |

---

## 👥 Equipo Actual

| Nombre | Rol |
|---|---|
| **Rab** | Fundador & CEO / Director |
| **Skellent** | Programador |
| **LouArtStuff** | Diseñadora Gráfica |
| **Silly** | Voice Actor (VA) |
| **Xata Jr.** (Addictive Gamer) | Ilustrador & Sprite Artist + Admin Web |
| **JBS_GAMES™** | Colaborador & Aliado externo |

---

## 🎮 Catálogo de Juegos

| Juego | Estado | URL |
|---|---|---|
| **Talk to the Hand** | En desarrollo 🔧 | https://gamejolt.com/games/Talk-to-the-hand-RGS/1006802 |
| **His Destiny** | Próximamente 🔜 | https://gamejolt.com/games/HisDestiny-RGS/1025984 |
| **The Run** *(x JBS_GAMES™)* | Lanzado ✅ | https://gamejolt.com/games/TR/1021632 |
| **VaultPlanet** *(x JBS_GAMES™)* | Lanzado ✅ | https://gamejolt.com/games/VP/1043581 |
| **Zero-State: LYXA** | Conceptualización 💭 | — |

---

## 🌐 Redes Sociales y Estudios Aliados

| Plataforma | URL |
|---|---|
| GameJolt | https://gamejolt.com/@RabGamesStudio |
| itch.io | https://rabgamesstudio.itch.io/ |
| YouTube | https://www.youtube.com/@RabbitGamesOficial |
| Discord | Próximamente |

**Estudios Aliados:** Rewite Pictures · ZAYgt · Nightmare Labs · Reptile Games · JBS_GAMES™
→ Todos en https://gamejolt.com/@[nombre]

---

## 📄 Sobre el Archivo HTML

Un **único archivo HTML autocontenido** (`index.html`). Sin servidor, sin base de datos, sin npm, sin build step.

| Tecnología | Uso |
|---|---|
| HTML5 + CSS3 + JS vanilla | Todo el sitio |
| Google Fonts CDN | Press Start 2P · Share Tech Mono · Rajdhani |
| Imágenes base64 | Screenshots de juegos embebidos en JS |
| Imágenes CDN (GameJolt) | Thumbnails y avatares por URL |
| Cloudflare Worker v4.0 | Backend del formulario |

**Peso:** ~540 KB · **Versión constante:** `const VERSION = 'v4.21'`

---

## ✨ Features Completas

### 🌐 Sistema Bilingüe (ES/EN)
- 180+ elementos traducidos con `T = { es:{...}, en:{...} }` y `applyLang(v)`
- Pop-up de idioma al cargar (`#lang-popup`) con `z-index: 99999` y `pointer-events: all`
- Toggle `🇬🇧 ENG / 🇪🇸 ESP` en el header disponible siempre

### 🕹️ CRT Effect
- CSS puro: `body::before` (scanlines) + `body::after` (viñeta) + `animation: crt-flicker`
- Al activar CRT: cursor personalizado hace fade-out — al desactivar: fade-in

### 🖱️ Cursor Personalizado
- Punto rosa 8px con `z-index: 999999`
- Se oculta completamente en dispositivos touch (`@media (hover: none)` + detección JS)
- Se oculta mientras hay cualquier popup abierto (`body.popup-open`)
- Se oculta con CRT activado

### 📱 Responsive / Mobile
- Breakpoints: `768px` (hamburger, grids 1col) · `480px` (tipografías reducidas) · `430px` (Android moderno)
- `@media (hover: none)`: cursor desactivado, `cursor: auto` restaurado
- `font-size: 16px` en todos los inputs/textareas en ≤430px — **previene autozoom en iOS**
- Modales con `overflow-y: auto` y `max-height` en ≤768px
- Botones del exit popup más grandes en ≤480px

### 🎞️ Slider del Hero
- 3 slides · auto-avance 4.8s · flechas + dots

### 🎮 Modal de Juegos
- Galería 3 imágenes · descripción bilingüe · género · estado · link GameJolt
- `overflow-y: auto` en móvil

### ⚖️ Políticas Legales
- 5 políticas en modales: Privacidad · T&C · Accesibilidad · Envío · Reembolso

### 🚪 Exit Popup
- Intercepta todos los links `http/https` externos
- Bilingüe · oculta cursor personalizado al abrirse

### 📬 Formulario con contador de caracteres
Ver sección dedicada más abajo.

---

## 📬 Formulario de Contacto → Cloudflare Worker

### Flujo

```
Usuario llena formulario
    ↓
FormData → Cloudflare Worker (POST)  [source="rab"]
    ↓
Worker envía en paralelo:
  ├── 📧 Email HTML (Resend) → 4 destinatarios
  │     adjuntos + info sensible incluidos
  └── 💬 Discord DM (bot) → IDs configurados
        mensaje texto markdown con # / ## / > / ` / || ||
        adjuntos como SPOILER_ (blur hasta click)
```

### Campos del formulario

| ID | `name` | Tipo | **Límite** | Notas |
|---|---|---|---|---|
| `#f_name` | `name` | text | **80** | Requerido |
| `#f_email` | `email` | email | **254** | Requerido · RFC 5321 |
| `#f_social` | `social` | text | **60** | Opcional |
| `#f_platform` | `socialPlatform` | select | — | Requerido si social ≠ "" |
| `#f_type` | `reason` | select | — | Tipo de consulta |
| `#f_msg` | `message` | textarea | **1000** | Requerido · overhead Discord |
| `#f_attach` | `attachment` | file | image/* · múltiples | Opcional |
| `#f_sensitive` | `sensitiveInfo` | textarea | **500** | Opcional · spoiler Discord |
| *(hidden)* | `source` | — | — | `"rab"` hardcoded en JS |

> **¿Por qué 1000 y no 2000?** El mensaje de Discord tiene un límite de 2000 chars totales. La estructura markdown del Worker (cabecera `#`, separadores `##`, blockquotes `>`, footer `-#`, bloque de info sensible) consume entre 818 y 1462 chars según los campos opcionales presentes. El Worker trunca dinámicamente al espacio real disponible; el formulario limita a 1000 como primera defensa conservadora.

### Indicador de caracteres

| Estado | Color | Condición | Animación |
|---|---|---|---|
| Normal | Gris | > 50 restantes | — |
| Advertencia | 🟡 Amarillo | ≤ 50 | `counter-pulse` |
| Peligro | 🟠 Naranja | ≤ 20 | `counter-pulse` |
| Límite | 🔴 Rosa + negrita | ≤ 0 | `counter-shake` + borde rojo |

`maxlength` en HTML (1ª defensa) + validación JS en `submitForm()` (2ª defensa). Reset automático al enviar con éxito.

### Campo de información sensible

Diseño con borde amarillo tenue, ícono 🔐 y franja superior degradada. Disclaimer de privacidad bilingüe encima del textarea.

- **Discord:** campo `🔐 ***INFORMACIÓN SENSIBLE***` + `|| contenido ||` (blur hasta click)
- **Email:** sección con fondo amarillo etiquetada "Información sensible"

### Mensajes Discord (Worker v4.0)

Formato texto puro — sin embed. Estructura real recibida en Discord:

```
# 🎮 NUEVO MENSAJE — RABGAMESSTUDIO

## ── 👤 ──────────────────────────
> 👤 ***Nombre del remitente***
> 📧 **Correo:** `correo@ejemplo.com`
> 🐦 Twitter/X: `@usuario`        ← solo si se proporcionó
> 🎯 **Motivo:** `Colaboración`    ← solo si se proporcionó
> 📎 **Adjuntos:** 2 archivos ↓   ← solo si hay adjuntos

## ── 💬 ──────────────────────────
> 💬 **Mensaje:**
> Línea 1 del mensaje
> Línea 2...

## ── 🔐 ──────────────────────────   ← solo si hay info sensible
> 🔐 ***INFORMACIÓN SENSIBLE***
> -# Maneja con discreción — solo visible al hacer click
|| contenido oculto ||

## ── 🕒 ──────────────────────────
-# 🎮 RabGamesStudio · <t:UNIX:f> · <t:UNIX:R>
```

Adjuntos (mensaje separado por cada imagen):
```
-# 📎 Adjunto 1 de 2: `foto.png` — click para revelar
[imagen con blur SPOILER_]
```

### Configuración del Worker (Cloudflare Secrets)

| Secret | Valor |
|---|---|
| `DISCORD_BOT_TOKEN` | Token del bot de Discord |
| `RESEND_API_KEY_RAB` | API key de Resend para RabGamesStudio |
| `RAB_DISCORD_ID_1` | `920017830605361232` (Addictive Gamer) |
| `RAB_DISCORD_ID_2` | vacío o `blank` |
| `RAB_DISCORD_ID_3` | vacío o `blank` |

---

## 🤖 Arquitectura Técnica para IAs y Desarrolladores

### Estructura del archivo

```
index.html
├── <head>
│   ├── Meta SEO · OG completo · Twitter Card · theme-color #ff2d78
│   ├── Google Fonts CDN
│   └── <style>  ~950 líneas
│       ├── :root — design tokens
│       ├── CRT effect
│       ├── Cursor personalizado
│       ├── @media (hover: none) — touch devices
│       ├── .char-counter · .field-counter-wrap · .field-over
│       ├── .sensitive-field · .sensitive-disclaimer
│       ├── Mobile fixes: 480px · 768px · hover:none
│       ├── Header · Hero · Slider · Secciones · Modales
│       └── Responsive: 768px · 480px · 430px
├── <body>
│   ├── .pixel-bg · #mouse-blob · #cursor-dot · #notif
│   ├── #exit-popup · #lang-popup
│   ├── <header> — nav fijo · CRT btn · lang toggle · hamburger
│   ├── <main>
│   │   ├── #home · #about-home · #support · #games-full
│   │   ├── #about-full · #team · #allied-studios · #news-full
│   │   ├── #social-embeds · #contact
│   ├── <footer>
│   ├── #legalModal · #gameModal
│   └── <script>  ~700 líneas
│       ├── const VERSION = 'v4.21'
│       ├── const IMG = {...}          ← base64 de imágenes
│       ├── const T = { es, en }       ← 180+ cadenas bilingües
│       ├── const games = { ttth, hd }
│       ├── const LEGAL = {...}        ← 5 políticas × 2 idiomas
│       └── funciones (ver tabla)
```

### Variables CSS Globales (`:root`)

```css
--bg-deep: #0a0a0f;  --bg-mid: #0f0f1a;  --bg-card: #13131f;  --bg-hover: #1a1a2e;
--border: #1e1e35;
--pink: #ff2d78;     --pink-dim: #c4215a;   --pink-glow: rgba(255,45,120,0.35);
--blue: #00d4ff;     --blue-dim: #0099bb;   --blue-glow: rgba(0,212,255,0.30);
--purple: #b347ff;   --purple-dim: #8230cc; --purple-glow: rgba(179,71,255,0.30);
--green: #39ff14;    --yellow: #ffe600;
--white: #e8e8f0;    --muted: #6a6a8a;      --muted2: #4a4a65;
--fp: 'Press Start 2P', monospace;
--fm: 'Share Tech Mono', monospace;
--fb: 'Rajdhani', sans-serif;
```

### Funciones JavaScript

| Función | Descripción |
|---|---|
| `selectLang(v)` | Cierra popup · aplica idioma · restaura cursor |
| `toggleLang()` | Alterna ES ↔ EN |
| `applyLang(v)` | Aplica `[data-i18n]` y `[data-i18n-ph]` |
| `setPopupCursor(open)` | Oculta/restaura cursor al abrir/cerrar cualquier popup |
| `updateCharCounter(el, max)` | Contador con 4 estados de color + animaciones |
| `updateSocialPlatformVisibility()` | Muestra/oculta `#f_platform_row` |
| `submitForm()` | Valida límites + envía FormData al Worker |
| `goTo(id)` · `goHome()` | Scroll suave a sección |
| `toggleCRT()` | Activa/desactiva `crt-on` |
| `slideMove(dir)` · `goSlide(n)` | Slider del hero |
| `toggleFAQ(el)` | Acordeón FAQ |
| `showNotif(msg)` | Toast 3s en `#notif` |
| `openLink(url)` | Exit popup |
| `toggleMenu()` | Nav hamburguesa |
| `openModal(id)` · `closeModal()` | Modal de juego |
| `openLegal(type)` · `closeLegal()` | Modal legal |
| `exitClose()` · `exitConfirm()` | Cerrar / confirmar exit popup |
| `interceptLinks()` | Listeners en `<a>` externos (se re-llama al cambiar idioma) |

### Responsive Breakpoints

| Breakpoint | Descripción |
|---|---|
| `768px` | Nav hamburguesa · grids 1 col · footer centrado · modales con scroll |
| `480px` | Tipografías reducidas · exit popup más grande · mobile fixes nuevos elementos |
| `430px` | Android moderno ~393px CSS · `font-size: 16px` en inputs (anti-zoom iOS) |
| `hover: none` | Cursor personalizado desactivado completamente (touch devices) |

---

## 🗂️ Guía para el Dueño del Estudio

**Cambiar versión:** solo `const VERSION = 'vX.XX'` al inicio del JS.

**Añadir juego:** entrada en `const games`, card en `#games-full`, traducciones en `T.es`/`T.en`.

**Cambiar destinatarios del email:** `worker-unified.js` → `buildSources(env)` → `rab.to[]`.

**Añadir ID de Discord:** Cloudflare Secrets → `RAB_DISCORD_ID_2` o `RAB_DISCORD_ID_3`.

**Añadir aliado:** card en `#allied-studios` + avatar en GameJolt CDN.

---

## 📦 Assets y Recursos Integrados

| Asset | Fuente |
|---|---|
| Avatar RabGamesStudio | GameJolt CDN (URL externa) |
| Thumbnails TTTH / His Destiny | GameJolt CDN (URL externa) |
| Screenshots de juegos | base64 inline en JS |
| Favicon (tab + Discord embed) | `favicon.png` en raíz del repo |
| Favicon en mensajes Discord | `https://raw.githubusercontent.com/addictive-gamer/rgs-portfolio/refs/heads/main/favicon.png` |

---

## 📋 Historial de Versiones

### v4.21 — Optimización móvil completa (21 mar 2026)

**➕ Añadido**
- `@media (hover: none)` — cursor personalizado completamente desactivado en touch: `display: none` + `cursor: auto`
- `font-size: 16px` en inputs/textareas en ≤430px — **elimina el autozoom de iOS** al tocar un campo
- `.char-counter` a `10px` en ≤480px (legible en pantallas pequeñas)
- `.sensitive-field` con padding reducido y `min-height: 80px` en ≤480px
- Botones exit popup (`font-size: 9px`) y título (`8px`) más legibles en ≤480px
- `.modal-inner` y `.legal-inner` con `overflow-y: auto` y `max-height` en ≤768px
- `.field-counter-wrap { overflow: visible }` en ≤768px — el contador no se corta

---

### v4.20 — Fix duplicados JS + límite mensaje (21 mar 2026)

**🐛 Bug fix crítico**
- `let exitTarget` declarado dos veces → `SyntaxError` que abortaba todo el script → `selectLang is not defined`
- Eliminado bloque duplicado (línea ~2544), consolidadas `exitClose()`, `exitConfirm()` e `interceptLinks()`

**✏️ Cambiado**
- Límite campo mensaje: **2000 → 1000** chars (overhead Discord)
- Worker: truncado dinámico calculando el espacio disponible real antes de truncar

---

### v4.19 — Contador de caracteres (21 mar 2026)

- Contador `restantes / máximo` en todos los campos de texto
- 4 estados: normal → 🟡 (≤50) → 🟠 (≤20) → 🔴 shake (≤0)
- `maxlength` HTML + validación JS · reset al enviar

---

### v4.18 — Campo de información sensible (21 mar 2026)

- Campo `// INFORMACIÓN SENSIBLE` con diseño amarillo + 🔐
- Discord: `||spoiler||` · Email: sección amarilla

---

### v4.17 — Worker v2.0 · Discohook · timestamps (21 mar 2026)

- Embeds Discord con favicon correcto por fuente
- Timestamps nativos `<t:UNIX:f>` · adjuntos `SPOILER_`
- Fix popup idioma: `pointer-events: all` + `z-index: 99999`

---

### v4.16 → v4.0

Ver historial completo en el repositorio.

---

## 🚀 Cómo publicar en GitHub Pages / Netlify

1. `index.html` en la raíz del repositorio
2. **Settings → Pages → Deploy from branch → main / root**
3. URL: `https://addictive-gamer.github.io/rgs-portfolio/`

**Conectar el Worker:**
1. [workers.cloudflare.com](https://workers.cloudflare.com) → nuevo Worker → pegar `worker-unified.js`
2. **Settings → Variables and Secrets** → configurar los secrets de la tabla
3. `WORKER_URL` en `index.html` ya apunta a `https://xata-portfolio-bot.addictivegamer.workers.dev/`

---

## 🛠 Créditos y Herramientas

| Elemento | Crédito |
|---|---|
| Diseño y desarrollo web | **Claude** (Anthropic) |
| Arte de juegos e identidad | RabGamesStudio™ |
| Ilustración & Sprites | Xata Jr. (Addictive Gamer) |
| Fuentes | Google Fonts (OFL) |
| Emails | **Resend** |
| Backend | **Cloudflare Worker v4.0** |
| Hosting | **GitHub Pages** |
| Admin repo & web | **Xata Jr.** |

---

> ⚠️ **CRÍTICO al editar manualmente:** No borrar `</style></head><body>`. Si la página se pone negra, ese es el primer lugar donde buscar.

*"No seguimos tendencias — creamos las nuestras." — RabGamesStudio™ · 2026*
