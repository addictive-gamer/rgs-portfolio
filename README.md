# 🐰 RabGamesStudio™ — Official Website README

> **Versión del sitio:** `v4.25`  
> **Última actualización:** 24 de marzo de 2026  
> **Mantenido por:** RabGamesStudio™ — Xata Jr. (Admin Web)  
> **Contacto oficial:** rabbitgames0103@gmail.com  
> **Repositorio:** [github.com/addictive-gamer/rgs-portfolio](https://github.com/addictive-gamer/rgs-portfolio)  
> **Portafolio en vivo:** [addictive-gamer.github.io/rgs-portfolio/](https://addictive-gamer.github.io/rgs-portfolio/)

![version](https://img.shields.io/badge/version-4.25-ff2d78?style=for-the-badge)
![host](https://img.shields.io/badge/Hosted_by-GitHub_Pages-black?style=for-the-badge&logo=github)
![lang](https://img.shields.io/badge/Bilingüe-ES%20%7C%20EN-b347ff?style=for-the-badge)
![worker](https://img.shields.io/badge/Backend-Cloudflare_Worker_v5.2-orange?style=for-the-badge&logo=cloudflare)
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
9. [Correcciones pendientes conocidas](#-correcciones-pendientes-conocidas)
10. [Guía para el dueño del estudio](#guía-para-el-dueño-del-estudio)
11. [Assets y recursos integrados](#assets-y-recursos-integrados)
12. [Historial de versiones](#historial-de-versiones)
13. [Cómo publicar](#cómo-publicar-en-github-pages--netlify)
14. [Créditos](#créditos-y-herramientas)

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
| Imágenes base64 | Screenshots + portadas JBS (embebidos en HTML) |
| Imágenes CDN (GameJolt) | Thumbnails y avatares por URL |
| Cloudflare Worker v5.2 | Backend del formulario |

**Peso:** ~790 KB · **Versión en código:** `const VERSION = 'v4.25'`

---

## ✨ Features Completas

### 🌐 Sistema Bilingüe (ES/EN)
- 180+ elementos traducidos con `T = { es:{...}, en:{...} }` y `applyLang(v)`
- Pop-up de idioma al cargar (`#lang-popup`) con `z-index: 99999` y `pointer-events: all`
- Toggle `🇬🇧 ENG / 🇪🇸 ESP` en el header disponible siempre

### 🕹️ CRT Effect
- CSS puro: `body::before` (scanlines) + `body::after` (viñeta) + `animation: crt-flicker`
- Al activar CRT: cursor personalizado hace fade-out — al desactivar: fade-in

### 🖱️ Cursor Personalizado — Crosshair Neón
- Crosshair rosa neón con punto central y 4 líneas, `z-index: 999999`
- Hover: escala 1.5x morado · Click: comprime a 0.65x
- Switch `✛ ON/OFF` en el header independiente del CRT
- Se oculta en touch, durante popups y con CRT activado

### 📱 Responsive / Mobile
- Breakpoints: `768px` (hamburger, grids 1col) · `480px` · `430px`
- `font-size: 16px` en inputs/textareas en ≤430px — previene autozoom iOS
- Modales con `overflow-y: auto` y `max-height` en ≤768px

### 🎞️ Slider del Hero
- 3 slides · auto-avance 4.8s · flechas + dots
- Slide 1: Talk to the Hand (GameJolt CDN)
- Slide 2: His Destiny (GameJolt CDN)
- Slide 3: imagen real de JBS_GAMES™ (base64 embebida, badge verde)

### 🎮 Catálogo de Juegos
- The Run y VaultPlanet con thumbnails reales (base64 embebidas — reemplazan SVG placeholder)
- Modal con galería de 3 imágenes, descripción bilingüe, género, estado, link GameJolt

### 🖼️ Preview de imágenes adjuntas
- Al seleccionar archivos: cuadrícula de miniaturas 72×72px con botón ✕
- Contador de archivos · se limpia al enviar con éxito

### 📁 Botón de adjuntos estilizado *(nuevo v4.25)*
- Input nativo reemplazado por botón con estética gaming (overlay invisible + botón visible)
- Borde dashed → rosa neon al hover · morado glow al focus
- Ícono de subida que sube al hover · hint de formatos aceptados
- Lista de pills bilingüe bajo el botón con nombre de cada archivo seleccionado
- Completamente accesible: input nativo superpuesto (opacity:0, z-index:2)
- Funciones: `updatePreview()` (miniaturas) + `updateFilePills()` (lista de nombres)

### ⚖️ Políticas Legales
- 5 políticas en modales: Privacidad · T&C · Accesibilidad · Envío · Reembolso

### 🚪 Exit Popup
- Intercepta todos los links `http/https` externos · bilingüe

---

## 📬 Formulario de Contacto → Cloudflare Worker

### Flujo v5.2

```
Usuario llena formulario
    ↓
FormData → POST https://xata-portfolio-bot.addictivegamer.workers.dev
    ↓
Worker v5.2:
  ├── 1. Discord (CRÍTICO — si falla aquí se devuelve error)
  │     ┌── RAB_WEBHOOK_URL configurado?
  │     │     SÍ → sendViaWebhook (embed + adjuntos, ?wait=true)
  │     │     NO → sendViaBotDM (embed + adjuntos por DM a cada ID)
  │     └── adjuntos renombrados a SPOILER_archivo.ext
  │
  ├── 2. D1 database (NON-FATAL)
  │     Si env.DB no está vinculado o falla: se loguea el error
  │     pero la respuesta sigue siendo { success: true }
  │     → el formulario nunca muestra error falso por D1
  │
  └── 3. Email HTML (non-fatal, background, no bloquea respuesta)
        Tabla de campos · blockquote de mensaje
        Sección amarilla para info sensible
        Incluye red social y plataforma
```

### ¿Por qué antes mostraba error si el mensaje llegaba?

El Worker anterior lanzaba excepción si D1 fallaba → `status: 500` → el frontend veía `success: false` → mostraba "algo salió mal". **Fix v5.2:** D1 es non-fatal. Solo `status: 500` si Discord falla.

### Campos del formulario

| ID | `name` | Tipo | **Límite** | Notas |
|---|---|---|---|---|
| `#f_name` | `name` | text | **80** | Requerido |
| `#f_email` | `email` | email | **254** | Requerido · RFC 5321 |
| `#f_social` | `social` | text | **60** | Opcional |
| `#f_platform` | `socialPlatform` | select | — | Requerido si social ≠ "" |
| `#f_type` | `reason` | select | — | Tipo de consulta |
| `#f_msg` | `message` | textarea | **1000** | Requerido |
| `#f_attach` | `attachment` | file | image/* · múltiples | Opcional · botón estilizado + preview |
| `#f_sensitive` | `sensitiveInfo` | textarea | **500** | Opcional · spoiler Discord |
| *(hidden)* | `source` | — | — | `"rab"` hardcoded en JS |

### Discord Embeds (Worker v5.2)

```
Embed:
  Título:      🎮 Nuevo mensaje — RabGamesStudio
  Color:       0xff2d78  (rosa RGS)
  Thumbnail:   favicon.png del repo GitHub
  Descripción: [nombre] se ha puesto en contacto.
  Campos:
    📧 Correo          [email]         inline
    🎯 Motivo          [motivo]        inline
    🔗 Red social      plat · @user   inline  (solo si aplica)
    💬 Mensaje         [texto max 1024]
    🔒 Info sensible   ||spoiler||     (solo si aplica)
  Footer:      RabGamesStudio · Portfolio Inbox
  Timestamp:   ISO 8601
  Adjuntos:    SPOILER_archivo.ext (blur hasta click)
```

### Configuración del Worker (Cloudflare Secrets)

| Secret | Descripción |
|---|---|
| `DISCORD_BOT_TOKEN` | Token del bot — requerido para modo DM bot |
| `RESEND_API_KEY_RAB` | API key de Resend |
| `RAB_DISCORD_IDS` | IDs de Discord separados por coma |
| `RAB_EMAIL` | Email destino (default: `rabbitgames0103@gmail.com`) |
| `RAB_WEBHOOK_URL` | *(opcional)* URL de Webhook de Discord — prioridad sobre DM bot |

> **Webhook vs Bot DM:** El Webhook envía a un canal fijo (no necesita bot activo en el servidor). El Bot DM envía mensajes privados a cada usuario en `RAB_DISCORD_IDS`. Si configuras ambos, el Webhook tiene prioridad.

---

## 🤖 Arquitectura Técnica (para IAs y Desarrolladores)

```
index.html  — único archivo autocontenido
├── <head>
│   ├── Meta SEO · OG · Twitter Card · theme-color #ff2d78
│   ├── Google Fonts CDN (Press Start 2P · Share Tech Mono · Rajdhani)
│   └── <style>  ~970 líneas
│       ├── :root, CRT, pixel-bg, cursor crosshair
│       ├── .file-input-wrap · .file-input-btn · .file-pill  ← NEW v4.25
│       ├── #f_preview · .prev-wrap · .prev-remove
│       ├── Hero slider · Games · About · Team · Allied · News
│       ├── Contact form · Sensitive field · Char counter
│       └── Responsive: 768px · 480px · 430px
├── <body>
│   ├── #mouse-blob   ← FIXED v4.25
│   ├── #cursor-dot (crosshair neón)
│   ├── #exit-popup · #lang-popup
│   ├── <header>
│   ├── <main>
│   │   ├── #home (slider, slide3 = JBS imagen real)
│   │   ├── #games-full (The Run + VP imágenes reales)
│   │   ├── #contact (botón adjuntos estilizado + preview)
│   │   └── ...resto de secciones
│   └── <script>
│       ├── let lang = 'es';   ← primera línea — fix TDZ
│       ├── const VERSION = 'v4.25'
│       ├── updateCharCounter · updatePreview · updateFilePills
│       ├── submitForm() → fetch WORKER_URL
│       └── toggleCRT · toggleCustomCursor · interceptLinks · etc.
```

---

## 🐛 Correcciones Pendientes Conocidas

### Worker — Adjuntos no llegan al email

**Severidad:** Baja — los adjuntos llegan a Discord correctamente como SPOILER_. El email solo contiene los datos de texto. Mejora futura.

---

### Página — `updateCharCounter` umbral duplicado *(cosmético)*

**Severidad:** Muy baja. `≤ 10` y `≤ 20` ambos asignan `danger`. Fix: eliminar el bloque `≤ 10`.

---

## 🗂️ Guía para el Dueño del Estudio

**Cambiar versión:** `const VERSION = 'vX.XX'` al inicio del JS.

**Usar Webhook de Discord:** Cloudflare → Settings → Variables → añadir `RAB_WEBHOOK_URL` con la URL del webhook del canal.

**Añadir juego:** entrada en `const games`, card en `#games-full`, traducciones en `T.es`/`T.en`.

**Añadir imagen real a un juego:** reemplazar `<div class="gfc-thumb-svg">` por `<div class="gfc-thumb"><img src="..."></div>`.

**Cambiar destinatarios del email:** `xata-portfolio-bot.js` → `buildSources(env)` → `rab.to[]`.

**Añadir ID de Discord:** Cloudflare Secrets → `RAB_DISCORD_IDS` (separar por coma).

---

## 📦 Assets y Recursos Integrados

| Asset | Fuente |
|---|---|
| Avatar RabGamesStudio | GameJolt CDN |
| Thumbnails TTTH / His Destiny | GameJolt CDN |
| **Thumbnail The Run** | base64 embebida ← v4.24 |
| **Thumbnail VaultPlanet** | base64 embebida ← v4.24 |
| **Hero slide 3 (JBS_GAMES™)** | base64 embebida ← v4.24 |
| Screenshots de juegos (modales) | base64 inline en JS |
| Favicon | `favicon.png` en raíz del repo |

---

## 📋 Historial de Versiones

### v4.25 — Bug fixes críticos + botón adjuntos + Worker v5.2 (24 mar 2026)

**🐛 Bug fixes**
- `#mouse-blob` faltaba en el HTML → crash en `mousemove` → div añadido
- `getElementById('exit-cancel')` retornaba null → crash → línea removida (botón ya tenía onclick inline)
- `lang` TDZ (`Cannot access 'lang' before initialization`) → `let lang = 'es'` movido a primera línea del script

**➕ Añadido**
- Botón de adjuntos estilizado: borde dashed neon, glow rosa/morado, ícono animado, lista de pills con nombres de archivos
- Funciones `updatePreview()` y `updateFilePills()` · traducciones `form_attach_btn` y `form_attach_hint`

**🔧 Worker v5.2 — xata-portfolio-bot**
- **D1 NON-FATAL:** si la base de datos falla, el Worker responde `{ success: true, dbWarning: '...' }` en vez de `status: 500` → el formulario ya no muestra error falso
- **Discord Embeds:** ya no usa texto plano — embed rico con color, thumbnail, campos inline, spoiler de info sensible, timestamp ISO
- **Webhook de Discord:** nuevo método opcional (`RAB_WEBHOOK_URL` / `XATA_WEBHOOK_URL`) — si está, se usa en vez del DM bot; soporta embeds + adjuntos
- Email HTML mejorado: tabla de campos, blockquote, sección amarilla para info sensible, incluye red social y plataforma
- Ambos métodos (webhook y DM bot) envían adjuntos como `SPOILER_archivo.ext`

---

### v4.24 — Imágenes reales JBS + preview adjuntos + Worker v5.1 (24 mar 2026)
- Thumbnails reales The Run y VaultPlanet (base64)
- Hero slide 3: imagen JBS_GAMES™
- Preview de adjuntos en el formulario
- `const VERSION` corregido

### v4.23 — Fix cursor IIFE + WORKER_URL (21 mar 2026)
### v4.22 — Crosshair neón + switch cursor (21 mar 2026)
### v4.21 — Optimización móvil completa (21 mar 2026)
### v4.20 — Fix duplicados JS + límite mensaje (21 mar 2026)
### v4.19 → v4.0 — Ver historial en el repositorio.

---

## 🚀 Cómo publicar en GitHub Pages / Netlify

1. `index.html` en la raíz del repositorio
2. **Settings → Pages → Deploy from branch → main / root**
3. URL: `https://addictive-gamer.github.io/rgs-portfolio/`

**Conectar el Worker (bot):**
1. [workers.cloudflare.com](https://workers.cloudflare.com) → pegar `xata-portfolio-bot.js`
2. **Settings → Variables and Secrets** → todos los secrets de la tabla
3. `WORKER_URL` en el HTML: `https://xata-portfolio-bot.addictivegamer.workers.dev`

**Conectar la database (xata-messages):**
1. Pegar `xata-messages.js` en un Worker separado
2. Vincular D1 database como `DB` en los bindings
3. Acceder en `https://xata-messages.addictivegamer.workers.dev/`

> ⚠️ **CRÍTICO al editar manualmente:** No borrar `</style></head><body>`. Si la página se pone negra, ese es el primer lugar donde buscar.

---

## 🛠 Créditos y Herramientas

| Elemento | Crédito |
|---|---|
| Diseño y desarrollo web | **Claude** (Anthropic) |
| Arte de juegos e identidad | RabGamesStudio™ |
| Ilustración & Sprites | Xata Jr. (Addictive Gamer) |
| Imágenes JBS_GAMES™ | JBS_GAMES™ |
| Fuentes | Google Fonts (OFL) |
| Emails | **Resend** |
| Backend | **Cloudflare Worker v5.2** |
| Hosting | **GitHub Pages** |
| Admin repo & web | **Xata Jr.** |

---

*"No seguimos tendencias — creamos las nuestras." — RabGamesStudio™ · 2026*
