# Guía de Estilo — Kioshi Shimabuku Portfolio

## Paleta de Colores

| Token | Valor | Uso |
|-------|-------|-----|
| `--ks-black` | `#000000` | Fondos oscuros, texto principal |
| `--ks-white` | `#ffffff` | Fondos claros, texto inverso |
| `--ks-mint` | `#4ade80` | Acentos sobre fondos oscuros, hover states |
| `--ks-mint-dark` | `#22c55e` | Labels pequeños sobre fondos claros |
| `--ks-gray-500` | `#6e6e78` | Texto secundario, descripciones |
| `--ks-gray-300` | `#9e9ea8` | Bordes, separadores |

## Tipografía

- **Font:** Source Code Pro (Google Fonts)
- **Headings:** 700 (Bold)
- **Body:** 400 (Regular)
- **Monospace** para todo — consistencia tipográfica total

## Principios de Diseño

1. **Sin gradientes** — uso de overlays sólidos
2. **Sin glassmorphism** — fondos opacos con alta opacidad
3. **Márgenes generosos** — espaciado `clamp(4rem, 10vw, 8rem)` entre secciones
4. **Imágenes con lazy loading** — performance primero
5. **Hover states sutiles** — transformaciones mínimas y cambios de borde
6. **Accesibilidad visible** — focus rings, skip link y contraste por contexto

## Componentes

### Service Card
- Fondo: `--ks-white-off`
- Borde: `1px solid --color-border`
- Icono: Símbolo geométrico (◆ ● ■), NO emoji
- Hover: `translateY(-2px)` + borde negro

### Project Card
- Imagen: aspect-ratio 4:3, object-fit cover
- Hover: `translateY(-4px)`
- Fallback: `.project-placeholder`, fondo `--ks-black-soft` con texto centrado

### Label
- Uppercase, letter-spacing 0.15em
- Color: `--color-accent-readable` en fondos claros
- Color: `--color-accent` en fondos oscuros
- Font-size: 0.75rem

### Navigation
- Header fijo con `scroll-padding-top` y `scroll-margin-top`
- Mobile nav con `aria-controls`, `aria-expanded` e `inert` cuando está cerrado
- Skip link para saltar directo al contenido
