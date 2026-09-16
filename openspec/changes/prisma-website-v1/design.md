# Diseño: Sitio Web Prisma Media House v1

## Principios de diseño

1. **Limpieza**: Menos es más. Espacio en blanco como elemento de diseño
2. **Profesionalismo**: Transmitir calidad y confianza
3. **Versatilidad**: Appeal tanto para empresas como creadores
4. **Accesibilidad**: Fácil navegación, CTA claro

## Identidad visual

### Logo

**Versión completa** (emblema circular):
- Uso: Hero section, About, footer grande
- Formato: PNG con fondo transparente

**Versión simplificada** (necesaria):
- Uso: Header, favicon, redes sociales
- Elementos: Solo prisma + texto "PRISMA MEDIA HOUSE"
- Formato: PNG, SVG

### Paleta de colores

```
PRIMARIOS
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Azul Marino    #1B2A4A  ████████  Confianza, base
Plata          #C0C0C0  ▓▓▓▓▓▓▓▓  Tecnología, limpieza
Bronce         #B87333  ░░░░░░░░  Elegancia, acento

MODO CLARO
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Fondo          #FFFFFF  ████████  Limpieza
Texto          #1a1a1a  ████████  Legibilidad
Secundario     #6c757d  ▓▓▓▓▓▓▓▓  Texto secundario

MODO OSCURO
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Fondo          #0D1117  ████████  Sofisticación
Texto          #E6EDF3  ▓▓▓▓▓▓▓▓  Legibilidad
Secundario     #8B9497  ░░░░░░░░  Texto secundario

ACENTOS
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Éxito          #28a745  ████████  Confirmaciones
Error          #dc3545  ████████  Errores
WhatsApp       #25D366  ████████  Botón de contacto
```

### Tipografía

```css
/* Principal - Títulos */
font-family: 'Inter', 'Segoe UI', system-ui, sans-serif;

/* Secundaria - Cuerpo */
font-family: 'Inter', 'Segoe UI', system-ui, sans-serif;

/* Tamaños base */
--text-xs:   0.75rem;   /* 12px */
--text-sm:   0.875rem;  /* 14px */
--text-base: 1rem;      /* 16px */
--text-lg:   1.125rem;  /* 18px */
--text-xl:   1.25rem;   /* 20px */
--text-2xl:  1.5rem;    /* 24px */
--text-3xl:  1.875rem;  /* 30px */
--text-4xl:  2.25rem;   /* 36px */
--text-5xl:  3rem;      /* 48px */
```

## Layout y espaciado

### Grid del sitio

```
┌─────────────────────────────────────────────────────────────┐
│  CONTENEDOR PRINCIPAL                                       │
│  max-width: 1200px                                          │
│  margin: 0 auto                                             │
│  padding: 0 1.5rem (mobile) / 0 2rem (desktop)              │
├─────────────────────────────────────────────────────────────┤
│                                                             │
│  HEADER                                                     │
│  height: 72px                                               │
│  position: sticky                                           │
│  backdrop-filter: blur(10px)                                │
│                                                             │
│  HERO                                                       │
│  min-height: 100vh                                          │
│  display: flex                                              │
│  align-items: center                                        │
│                                                             │
│  SECCIONES                                                  │
│  padding: 6rem 0                                            │
│                                                             │
│  FOOTER                                                     │
│  padding: 4rem 0 2rem                                       │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

### Espaciado entre secciones

```
Sección → Siguiente sección: 6rem (96px)
Elemento → Elemento: 2rem (32px)
Título → Párrafo: 1rem (16px)
Párrafo → Párrafo: 1rem (16px)
```

## Componentes

### Header

```
┌─────────────────────────────────────────────────────────────┐
│  [Logo]    Servicios  Portafolio  Nosotros  [🌙/☀️]  [CTA] │
└─────────────────────────────────────────────────────────────┘

Mobile:
┌─────────────────────────────┐
│  [Logo]        [☰]  [🌙/☀️] │
└─────────────────────────────┘
```

- Fijo en scroll
- Fondo semi-transparente con blur
- Logo a la izquierda
- Navegación al centro
- Toggle tema + CTA a la derecha
- Menú hamburguesa en mobile

### Hero

```
┌─────────────────────────────────────────────────────────────┐
│  ░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░ │
│  ░░░░░░░░░░░░░░░ VIDEO DE FONDO ░░░░░░░░░░░░░░░░░░░░░░░░░░░ │
│  ░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░ │
│                                                             │
│              PRODUCCIÓN AUDIOVISUAL                         │
│              PROFESIONAL                                    │
│                                                             │
│              Transformamos tu idea en contenido             │
│              que conecta con tu audiencia.                  │
│                                                             │
│              [ 🟢 Cotiza tu proyecto ]                      │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

- Video de fondo con overlay oscuro
- Texto centrado
- CTA prominente con color WhatsApp
- Animación suave al cargar

### Tarjetas de servicios

```
┌─────────────────┐  ┌─────────────────┐  ┌─────────────────┐
│  [Icono]        │  │  [Icono]        │  │  [Icono]        │
│                 │  │                 │  │                 │
│  Título         │  │  Título         │  │  Título         │
│                 │  │                 │  │                 │
│  Descripción    │  │  Descripción    │  │  Descripción    │
│  breve del      │  │  breve del      │  │  breve del      │
│  servicio.      │  │  servicio.      │  │  servicio.      │
│                 │  │                 │  │                 │
│  [Ver más →]    │  │  [Ver más →]    │  │  [Ver más →]    │
└─────────────────┘  └─────────────────┘  └─────────────────┘
```

- Bordes sutiles
- Sombra ligera en hover
- Icono representativo
- Transición suave

### Botón de WhatsApp (flotante)

```
┌─────────────────────────────────────────────────────────────┐
│                                                             │
│                                         ┌─────────┐         │
│                                         │  💬     │         │
│                                         │ WhatsApp│         │
│                                         └─────────┘         │
│                                              ↑              │
│                                         Fixed bottom-right  │
└─────────────────────────────────────────────────────────────┘
```

- Posición: Fixed, bottom-right
- Color: WhatsApp green (#25D366)
- Icono: WhatsApp SVG
- Hover: Scale ligeramente
- Z-index alto (siempre visible)

### Sección de proceso

```
┌─────────────────────────────────────────────────────────────┐
│                                                             │
│  CÓMO TRABAJAMOS                                            │
│                                                             │
│  ┌─────┐      ┌─────┐      ┌─────┐      ┌─────┐           │
│  │  1  │─────▶│  2  │─────▶│  3  │─────▶│  4  │           │
│  └─────┘      └─────┘      └─────┘      └─────┘           │
│  Contactas     Cotizamos    Produciimos   Entregamos       │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

- Línea conectora entre pasos
- Números circulares
- Animación al scroll (reveal)

## Animaciones

### Transiciones

```css
/* Hover en botones */
transition: all 0.2s ease;

/* Cambio de tema */
transition: background-color 0.3s ease, color 0.3s ease;

/* Aparición de elementos */
animation: fadeInUp 0.6s ease forwards;
```

### Scroll reveal

```css
/* Elementos aparecen al hacer scroll */
.reveal {
  opacity: 0;
  transform: translateY(20px);
  transition: all 0.6s ease;
}

.reveal.active {
  opacity: 1;
  transform: translateY(0);
}
```

## Responsive

### Mobile (< 768px)

- Header: Logo + hamburguesa + toggle tema
- Hero: Texto más pequeño, CTA centrado
- Servicios: 1 columna
- Portafolio: 1-2 columnas
- Proceso: Vertical
- Footer: Stack de elementos

### Tablet (768px - 1024px)

- Header: Logo + nav compacto + toggle
- Hero: Texto mediano
- Servicios: 2 columnas
- Portafolio: 2-3 columnas
- Proceso: Horizontal compacto

### Desktop (> 1024px)

- Header: Logo + nav completo + toggle + CTA
- Hero: Texto grande, layout completo
- Servicios: 3-4 columnas
- Portafolio: 3-4 columnas
- Proceso: Horizontal completo

## Accesibilidad

- Contraste mínimo 4.5:1 (WCAG AA)
- Focus visible en todos los elementos interactivos
- Alt text en todas las imágenes
- Navegación por teclado
- Reduced motion: Respetar prefers-reduced-motion
