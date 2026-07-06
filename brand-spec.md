# 🎨 Kioshi Shimabuku — Brand Spec

> Identidad visual del diseñador, educador y creador de cultura.
> Documento fuente para la landing page demo-kioshi-landing.

---

## 1. Brand Attributes

### Voz
- **Directa, sin relleno.** Al grano. Como él dice: "La mente está hecha para crear ideas, no para retenerlas."
- **Precisa y ejecutable.** Las ideas valen si se ejecutan. El "cómo" importa tanto como el "qué".
- **Peruana sin vueltas.** Español directo, a veces seco, sin falsa energía.
- **Conectivista.** Cruza disciplinas: moda × tecnología, diseño × IA, artesanía × digital.

### Tono
| Canal | Tono |
|-------|------|
| Landing / Bio | Profesional, minimalista, seguro de sí mismo |
| Proyectos | Técnico pero accesible — muestra el proceso |
| Redes sociales | Directo, cultural, sin pulir en exceso |
| Docencia | Pedagógico, estructurado, generoso con el conocimiento |
| Cotidiano | Seco, práctico, peruano sin filtro |

### Valores
1. **Impacto cultural peruano** — no folclore turístico, sino diseño contemporáneo con raíz nikkei-tusan
2. **Ejecución sobre teoría** — lo que se puede hacer, enseñar y compartir
3. **Fusión análogo-digital** — el puente entre lo físico (pines, libretas, tela) y lo digital (IA, fabricación 3D, diseño generativo)
4. **Propósito como norte** — ayudar a otros a encontrar el suyo mientras construye el propio
5. **Autenticidad sin postureo** — nada de "productivity porn", nada de filtros preestablecidos, nada de falso táctico

---

## 2. Paleta de Color (OKLCH)

### Sistema cromático

```
Negro base  ──  techwear, minimalismo funcional
Rojo Perú   ──  presencia, impacto, cultura
Gris frío   ──  neutro técnico, estructura
Dorado      ──  detalle premium, ediciones especiales
Crema       ──  contrapunto cálido, textura editorial
Blanco      ──  soporte, espacio negativo
```

### Colores

| Token | OKLCH | HEX | Uso |
|-------|-------|-----|-----|
| `--ks-black` | `oklch(0% 0 0)` | `#000000` | Fondo principal, base visual |
| `--ks-black-soft` | `oklch(12% 0.003 280)` | `#1A1A1E` | Fondo de tarjetas, secciones secundarias |
| `--ks-black-mid` | `oklch(22% 0.005 275)` | `#303036` | Bordes, líneas divisorias, superficie hover |
| `--ks-red` | `oklch(50% 0.21 29)` | `#CC0000` | Color héroe — acento principal, botones CTA |
| `--ks-red-emphasis` | `oklch(42% 0.18 29)` | `#990000` | Hover del rojo, estados activos |
| `--ks-gray-700` | `oklch(35% 0.008 280)` | `#525258` | Texto terciario, metadatos |
| `--ks-gray-500` | `oklch(52% 0.01 280)` | `#808088` | Texto muted, descripciones |
| `--ks-gray-300` | `oklch(72% 0.01 278)` | `#B0B0B8` | Texto secundario sobre fondos oscuros |
| `--ks-gray-100` | `oklch(88% 0.005 278)` | `#DBDBE0` | Texto body sobre fondos oscuros |
| `--ks-gold` | `oklch(65% 0.14 78)` | `#C8A84C` | Acento premium — badges, detalles de edición limitada |
| `--ks-gold-soft` | `oklch(75% 0.09 82)` | `#DCC78A` | Gold hover, brillo sutil |
| `--ks-cream` | `oklch(95% 0.007 90)` | `#F2EDE6` | Fondo alternativo claro, textura editorial |
| `--ks-white` | `oklch(100% 0 0)` | `#FFFFFF` | Fondo claro, texto sobre fondos oscuros |
| `--ks-white-off` | `oklch(98% 0.002 280)` | `#F8F8FA` | Fondo claro secundario |

### Combinaciones clave

| Contexto | Fondo | Texto | Acento |
|----------|-------|-------|--------|
| Modo oscuro (default) | `#000000` | `#DBDBE0` | `#CC0000` |
| Modo claro | `#F2EDE6` | `#1A1A1E` | `#CC0000` |
| Tarjeta oscura | `#1A1A1E` | `#B0B0B8` | `#C8A84C` |
| Hero / landing section | `#000000` | `#FFFFFF` | `#CC0000` |
| Detalle premium | `#1A1A1E` | `#C8A84C` | `#DCC78A` |

---

## 3. Tipografía

### Sistema tipográfico

| Rol | Fuente | Peso | Uso |
|-----|--------|------|-----|
| **Display / Títulos** | `"DM Serif Display"` | 700 (Bold) | H1–H3, hero headings, marquee |
| **Display alterno** | `"DM Serif Display"` | 400 (Regular) | H4, subtítulos grandes, pull quotes |
| **Body / Sans** | `"Inter"` | 300–700 | Cuerpo de texto, UI, nav, body copy |
| **Monospace (funcional)** | `"JetBrains Mono"` | 400–700 | Código, specs técnicas, métricas, datos |
| **Fallback** | `serif` / `system-ui` / `monospace` | — | Stack de respaldo progresivo |

### Stack font-family (Tailwind v4)

```css
/* Display serif */
'DM Serif Display', serif

/* Body sans */
'Inter', system-ui, -apple-system, sans-serif

/* Mono funcional */
'JetBrains Mono', 'SF Mono', 'Fira Code', monospace
```

### Escala tipográfica

| Nivel | Tamaño | Line-height | Font | Peso |
|-------|--------|-------------|------|------|
| `h1` | `clamp(2.5rem, 5vw, 4.5rem)` | `1.1` | Display | 700 |
| `h2` | `clamp(2rem, 3.5vw, 3rem)` | `1.2` | Display | 700 |
| `h3` | `clamp(1.5rem, 2.5vw, 2.25rem)` | `1.25` | Display | 400 |
| `h4` | `clamp(1.25rem, 2vw, 1.75rem)` | `1.3` | Display | 400 |
| `body-large` | `1.125rem` | `1.6` | Inter | 400 |
| `body` | `1rem` | `1.6` | Inter | 400 |
| `body-small` | `0.875rem` | `1.5` | Inter | 400 |
| `caption` | `0.75rem` | `1.4` | Inter | 500 |
| `mono` | `0.875rem` | `1.5` | JetBrains Mono | 400 |
| `mono-small` | `0.75rem` | `1.4` | JetBrains Mono | 500 |

### Tracking (letter-spacing)

| Contexto | Letter-spacing |
|----------|----------------|
| Display H1–H2 | `-0.02em` |
| Display H3–H4 | `-0.01em` |
| Body (Inter) | `0` |
| Mono | `0` |
| Nav / UI labels | `0.05em` (uppercase) |
| Caption / metadatos | `0.03em` |

---

## 4. Design Tokens — @theme para Tailwind v4

```css
@theme {
  /* ─── Colores ─── */
  --color-ks-black: #000000;
  --color-ks-black-soft: #1A1A1E;
  --color-ks-black-mid: #303036;
  --color-ks-red: #CC0000;
  --color-ks-red-emphasis: #990000;
  --color-ks-gray-700: #525258;
  --color-ks-gray-500: #808088;
  --color-ks-gray-300: #B0B0B8;
  --color-ks-gray-100: #DBDBE0;
  --color-ks-gold: #C8A84C;
  --color-ks-gold-soft: #DCC78A;
  --color-ks-cream: #F2EDE6;
  --color-ks-white: #FFFFFF;
  --color-ks-white-off: #F8F8FA;

  /* ─── Tipografía ─── */
  --font-display: 'DM Serif Display', serif;
  --font-body: 'Inter', system-ui, -apple-system, sans-serif;
  --font-mono: 'JetBrains Mono', 'SF Mono', 'Fira Code', monospace;

  /* ─── Escala tipográfica ─── */
  --text-h1: clamp(2.5rem, 5vw, 4.5rem);
  --text-h1--line-height: 1.1;
  --text-h1--font-weight: 700;
  --text-h1--letter-spacing: -0.02em;
  --text-h1--font-family: var(--font-display);

  --text-h2: clamp(2rem, 3.5vw, 3rem);
  --text-h2--line-height: 1.2;
  --text-h2--font-weight: 700;
  --text-h2--letter-spacing: -0.02em;
  --text-h2--font-family: var(--font-display);

  --text-h3: clamp(1.5rem, 2.5vw, 2.25rem);
  --text-h3--line-height: 1.25;
  --text-h3--font-weight: 400;
  --text-h3--letter-spacing: -0.01em;
  --text-h3--font-family: var(--font-display);

  --text-h4: clamp(1.25rem, 2vw, 1.75rem);
  --text-h4--line-height: 1.3;
  --text-h4--font-weight: 400;
  --text-h4--letter-spacing: -0.01em;
  --text-h4--font-family: var(--font-display);

  --text-body: 1rem;
  --text-body--line-height: 1.6;
  --text-body--font-weight: 400;
  --text-body--font-family: var(--font-body);

  --text-body-large: 1.125rem;
  --text-body-large--line-height: 1.6;
  --text-body-large--font-weight: 400;
  --text-body-large--font-family: var(--font-body);

  --text-body-small: 0.875rem;
  --text-body-small--line-height: 1.5;
  --text-body-small--font-family: var(--font-body);

  --text-caption: 0.75rem;
  --text-caption--line-height: 1.4;
  --text-caption--font-weight: 500;
  --text-caption--letter-spacing: 0.03em;
  --text-caption--font-family: var(--font-body);

  --text-mono: 0.875rem;
  --text-mono--line-height: 1.5;
  --text-mono--font-family: var(--font-mono);

  --text-mono-small: 0.75rem;
  --text-mono-small--line-height: 1.4;
  --text-mono-small--font-weight: 500;
  --text-mono-small--font-family: var(--font-mono);

  /* ─── Espaciado ─── */
  --spacing-unit: 8px;
  --spacing-gap: 24px;
  --spacing-section: clamp(4rem, 8vw, 8rem);

  /* ─── Layout ─── */
  --radius-none: 0px;
  --radius-sm: 4px;
  --radius-md: 8px;
  --radius-full: 9999px;
  --container-max: 1280px;
  --container-narrow: 960px;

  /* ─── Bordes ─── */
  --border-ks-black-mid: 1px solid var(--color-ks-black-mid);
  --border-ks-gray-500: 1px solid var(--color-ks-gray-500);
  --border-ks-gold: 1px solid var(--color-ks-gold);

  /* ─── Animación ─── */
  --duration-fast: 150ms;
  --duration-normal: 300ms;
  --duration-slow: 500ms;
  --easing-default: cubic-bezier(0.4, 0, 0.2, 1);
  --easing-emphasis: cubic-bezier(0.16, 1, 0.3, 1);
}
```

---

## 5. CSS Variables para aplicar

```css
:root {
  /* Colores */
  --ks-black: #000000;
  --ks-black-soft: #1A1A1E;
  --ks-black-mid: #303036;
  --ks-red: #CC0000;
  --ks-red-emphasis: #990000;
  --ks-gray-700: #525258;
  --ks-gray-500: #808088;
  --ks-gray-300: #B0B0B8;
  --ks-gray-100: #DBDBE0;
  --ks-gold: #C8A84C;
  --ks-gold-soft: #DCC78A;
  --ks-cream: #F2EDE6;
  --ks-white: #FFFFFF;
  --ks-white-off: #F8F8FA;

  /* Tipografía */
  --ks-font-display: 'DM Serif Display', serif;
  --ks-font-body: 'Inter', system-ui, -apple-system, sans-serif;
  --ks-font-mono: 'JetBrains Mono', 'SF Mono', 'Fira Code', monospace;

  /* Escala */
  --ks-h1: clamp(2.5rem, 5vw, 4.5rem);
  --ks-h2: clamp(2rem, 3.5vw, 3rem);
  --ks-h3: clamp(1.5rem, 2.5vw, 2.25rem);
  --ks-h4: clamp(1.25rem, 2vw, 1.75rem);
  --ks-body: 1rem;
  --ks-body-large: 1.125rem;
  --ks-body-small: 0.875rem;
  --ks-caption: 0.75rem;
  --ks-mono: 0.875rem;
  --ks-mono-small: 0.75rem;

  /* Espaciado */
  --ks-unit: 8px;
  --ks-gap: 24px;
  --ks-section: clamp(4rem, 8vw, 8rem);
}

/* Modo oscuro (default) */
:root {
  --ks-bg: var(--ks-black);
  --ks-bg-card: var(--ks-black-soft);
  --ks-bg-surface: var(--ks-black-soft);
  --ks-text: var(--ks-gray-100);
  --ks-text-secondary: var(--ks-gray-300);
  --ks-text-muted: var(--ks-gray-500);
  --ks-border: var(--ks-black-mid);
  --ks-accent: var(--ks-red);
  --ks-accent-hover: var(--ks-red-emphasis);
  --ks-premium: var(--ks-gold);
}

/* Modo claro */
.light {
  --ks-bg: var(--ks-cream);
  --ks-bg-card: var(--ks-white);
  --ks-bg-surface: var(--ks-white-off);
  --ks-text: var(--ks-black-soft);
  --ks-text-secondary: var(--ks-gray-700);
  --ks-text-muted: var(--ks-gray-500);
  --ks-border: var(--ks-gray-300);
  --ks-accent: var(--ks-red);
  --ks-accent-hover: var(--ks-red-emphasis);
  --ks-premium: var(--ks-gold);
}
```

---

## 6. Layout & Espaciado

### Grid
- **Sistema:** 12 columnas responsivas (4 móvil, 8 tablet, 12 desktop)
- **Gap:** 24px (`--ks-gap`)
- **Max width:** 1280px (`--container-max`)
- **Narrow width:** 960px (`--container-narrow`)
- **Margen lateral:** `clamp(1rem, 4vw, 3rem)`

### Component layout patterns

| Patrón | Descripción |
|--------|-------------|
| **Hero full-bleed** | Fondo negro total, título display serif, línea roja decorativa |
| **Bento grid** | Secciones asimétricas con tarjetas de fondo `black-soft` |
| **Marquee** | Texto display scrolling, típicamente listando proyectos |
| **Proyecto card** | Imagen + título + tags + breve descripción, sin bordes |
| **Timeline** | Línea vertical con dots rojos, texto mono para fechas |

---

## 7. Animación

| Token | Valor | Uso |
|-------|-------|-----|
| `--duration-fast` | `150ms` | Hover en links, color transitions |
| `--duration-normal` | `300ms` | Card hover, fade-in, stagger |
| `--duration-slow` | `500ms` | Page transitions, hero reveal |
| `--easing-default` | `cubic-bezier(0.4, 0, 0.2, 1)` | UI estándar |
| `--easing-emphasis` | `cubic-bezier(0.16, 1, 0.3, 1)` | Entradas dramáticas, scroll reveals |

Intensidad de movimiento: **5/10** — animaciones sutiles pero presentes. Nada gratuito.

---

## 8. Tono de Voz — Keywords y vocabulario

### Palabras Kioshi (léxico propio)
```
nikkei, tusán, peruano, propósito, conectar, ejecutar,
fabricación digital, diseño paramétrico, editorial, pin,
badge, coleccionable, identidad, cultura portable,
sistema visual, dirección creativa, educador, taller,
ethos, oficio, digital-análogo, laboratorio
```

### Permitido
- Directo, seco cuando corresponde
- Técnico pero accesible
- Peruano sin exotizar
- Conectivista (cruce de disciplinas)

### Prohibido
- "Productivity porn", jerga startup vacía
- Falso táctico / falso militar
- Folclore turístico superficial
- Lenguaje corporativo genérico
- Relleno, fluff, palabras de más
- Frases comando hiperactivas ("Abre. Escribe. Vuelve.")

---

## 9. W3C Design Tokens compatibles

Para integración con `brand-tokenizer` skill y el ecosistema de skills (frontend, brief-tendencias-pdf, copywriting, neuro-presentation-designer, edge-tts):

```json
{
  "meta": {
    "brand": "Kioshi Shimabuku",
    "role": "Diseñador Gráfico · Diseñador de Juguetes · Estratega Visual · Educador",
    "version": "1.0.0",
    "standard": "W3C-DTCG-2025.10",
    "generated": "2026-07-05"
  },
  "color": {
    "black":           { "$value": "#000000", "$type": "color", "$description": "Fondo principal — techwear, minimalismo funcional" },
    "blackSoft":       { "$value": "#1A1A1E", "$type": "color", "$description": "Tarjetas, superficies secundarias" },
    "blackMid":        { "$value": "#303036", "$type": "color", "$description": "Bordes, divisores" },
    "red":             { "$value": "#CC0000", "$type": "color", "$description": "Color héroe — impacto, cultura peruana" },
    "redEmphasis":     { "$value": "#990000", "$type": "color", "$description": "Hover del rojo" },
    "gray700":         { "$value": "#525258", "$type": "color" },
    "gray500":         { "$value": "#808088", "$type": "color" },
    "gray300":         { "$value": "#B0B0B8", "$type": "color" },
    "gray100":         { "$value": "#DBDBE0", "$type": "color" },
    "gold":            { "$value": "#C8A84C", "$type": "color", "$description": "Acento premium — ediciones especiales" },
    "goldSoft":        { "$value": "#DCC78A", "$type": "color" },
    "cream":           { "$value": "#F2EDE6", "$type": "color", "$description": "Fondo claro alternativo" },
    "white":           { "$value": "#FFFFFF", "$type": "color" },
    "whiteOff":        { "$value": "#F8F8FA", "$type": "color" }
  },
  "fontFamily": {
    "display":         { "$value": ["DM Serif Display", "serif"], "$type": "fontFamily" },
    "body":            { "$value": ["Inter", "system-ui", "sans-serif"], "$type": "fontFamily" },
    "mono":            { "$value": ["JetBrains Mono", "SF Mono", "Fira Code", "monospace"], "$type": "fontFamily" }
  },
  "fontWeight": {
    "displayBold":     { "$value": 700, "$type": "fontWeight" },
    "displayRegular":  { "$value": 400, "$type": "fontWeight" },
    "bodyRegular":     { "$value": 400, "$type": "fontWeight" },
    "bodyMedium":      { "$value": 500, "$type": "fontWeight" },
    "bodyBold":        { "$value": 700, "$type": "fontWeight" },
    "monoRegular":     { "$value": 400, "$type": "fontWeight" },
    "monoMedium":      { "$value": 500, "$type": "fontWeight" }
  },
  "dimension": {
    "unit":            { "$value": "8px", "$type": "dimension" },
    "gap":             { "$value": "24px", "$type": "dimension" },
    "containerMax":    { "$value": "1280px", "$type": "dimension" },
    "containerNarrow": { "$value": "960px", "$type": "dimension" },
    "radiusSm":        { "$value": "4px", "$type": "dimension" },
    "radiusMd":        { "$value": "8px", "$type": "dimension" }
  },
  "duration": {
    "fast":            { "$value": "150ms", "$type": "duration" },
    "normal":          { "$value": "300ms", "$type": "duration" },
    "slow":            { "$value": "500ms", "$type": "duration" }
  },
  "brand": {
    "name":            { "$value": "Kioshi Shimabuku", "$type": "string" },
    "role":            { "$value": "Diseñador Gráfico · Diseñador de Juguetes · Estratega Visual · Educador", "$type": "string" },
    "purpose":         { "$value": "Impactar positivamente la cultura peruana a través de la creatividad", "$type": "string" },
    "styleKeywords":   { "$value": ["techwear", "japandi", "minimalismo funcional", "nikkei tusan", "peruano"], "$type": "string" },
    "toneOfVoice":     { "$value": "Directo, sin relleno. Peruano sin vueltas. Práctico, ejecutable, conectivista.", "$type": "string" },
    "projects":        { "$value": ["Metalmorfosis", "Libretácticas", "Llami Claw", "QNTM"], "$type": "string" },
    "motionIntensity": { "$value": 5, "$type": "number" }
  }
}
```

---

## 10. Assets de referencia

| Asset | Tipo | Descripción |
|-------|------|-------------|
| Logo personal | Logotipo | Nombre "Kioshi Shimabuku" en display serif, preferible negro o blanco |
| Symbol | Icono | Por definir — posible monograma KS en geometría japandi |
| Foto perfil | Fotografía | Retrato editorial, fondo negro, iluminación lateral, sin sonrisa forzada |
| Patrón textura | Textura | Microtextura granular tipo "fuzzy skin" o papel japonés |

---

*Source of truth para la landing page Kioshi Shimabuku. Compatible con brand-tokenizer W3C DTCG.*
