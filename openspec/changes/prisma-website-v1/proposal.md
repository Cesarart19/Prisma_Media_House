# Propuesta: Sitio Web Prisma Media House v1

## Resumen

Crear el sitio web de presentación para **Prisma Media House**, una productora audiovisual en Bogotá. El sitio servirá como presencia digital para captar leads mediante prospección directa, con botón de WhatsApp como canal de contacto principal.

## Contexto

- **Negocio nuevo**: No hay cartera de clientes ni portafolio propio
- **Estrategia**: Prospección activa (contactar clientes directamente)
- **Mercado**: Bogotá, Colombia - público variado (empresas, influencers, creadores, restaurantes, gimnasios, etc.)
- **Presupuesto**: Initial phase - máxima eficiencia con recursos disponibles

## Objetivos

1. **Presencia digital**: Tener un sitio profesional que genere credibilidad
2. **Lead generation**: Botón de WhatsApp para contacto directo
3. **SEO básico**: Posicionarse para búsquedas locales de servicios audiovisuales
4. **Portafolio temporal**: Mostrar trabajos con contenido stock mientras se genera contenido propio

## Alcance

### Incluido

- [ ] Sitio web de una página (landing page)
- [ ] Diseño responsive (móvil, tablet, desktop)
- [ ] Modo oscuro/claro con toggle
- [ ] Header fijo con logo simplificado
- [ ] Hero con video de fondo (stock)
- [ ] Sección de servicios (sin precios)
- [ ] Portafolio placeholder (imágenes stock + fotos de equipo)
- [ ] Sección "Cómo trabajamos"
- [ ] Sección "Sobre nosotros"
- [ ] CTA con botón de WhatsApp (flotante)
- [ ] Footer con redes sociales
- [ ] SEO básico (meta titles, descriptions, Open Graph)
- [ ] Deploy en Vercel

### No incluido (futuro)

- [ ] Sistema de cotización en línea
- [ ] Blog
- [ ] Multiidioma
- [ ] Formulario de contacto tradicional
- [ ] Galería de videos interactiva

## Especificación Técnica

### Stack

```
Framework:  Astro 5.x
Lenguajes:  HTML5, CSS3, JavaScript (mínimo)
Deploy:     Vercel
Assets:     Imágenes stock + fotos propias
```

### Estructura del sitio

```
┌─────────────────────────────────────────────────────────────┐
│  HEADER FIJO                                                │
│  Logo (simplificado) | Nav | Botón WhatsApp                 │
├─────────────────────────────────────────────────────────────┤
│  HERO                                                       │
│  Video de fondo | Tagline | CTA WhatsApp                    │
├─────────────────────────────────────────────────────────────┤
│  SERVICIOS                                                  │
│  Producción | Planes mensuales | Cursos | Alquiler          │
├─────────────────────────────────────────────────────────────┤
│  PORTAFOLIO                                                 │
│  Imágenes stock + fotos de equipo (placeholder)             │
├─────────────────────────────────────────────────────────────┤
│  CÓMO TRABAJAMOS                                            │
│  4 pasos: Contacto → Cotización → Producción → Entrega      │
├─────────────────────────────────────────────────────────────┤
│  SOBRE NOSOTROS                                             │
│  Misión, valores, equipos que usamos                        │
├─────────────────────────────────────────────────────────────┤
│  CTA FINAL                                                  │
│  "¿Listo para crear contenido?" → WhatsApp                  │
├─────────────────────────────────────────────────────────────┤
│  FOOTER                                                     │
│  Redes sociales | WhatsApp | Email                          │
└─────────────────────────────────────────────────────────────┘
```

### Paleta de colores

```css
:root {
  /* Primarios */
  --color-primary: #1B2A4A;        /* Azul marino - confianza */
  --color-secondary: #C0C0C0;      /* Plata - tecnología */
  --color-accent: #B87333;         /* Bronce - elegancia */
  
  /* Neutros modo claro */
  --color-bg-light: #FFFFFF;
  --color-text-light: #1a1a1a;
  
  /* Neutros modo oscuro */
  --color-bg-dark: #0D1117;
  --color-text-dark: #E6EDF3;
  
  /* Transiciones */
  --transition-theme: 0.3s ease;
}
```

### Modo oscuro/claro

- Toggle en header (icono sol/luna)
- Preferencia guardada en localStorage
- Respeta prefers-color-scheme del sistema
- Transición suave entre modos

### Responsive breakpoints

```css
/* Mobile:  < 768px   - 1 columna */
/* Tablet:  768-1024px - 2 columnas */
/* Desktop: > 1024px   - layout completo */
```

## Servicios a mostrar

### 1. Producción de Contenido para Empresas
- Videos corporativos, institucionales, promocionales
- Videos de productos, testimoniales, entrevistas
- Contenido para redes sociales
- Cobertura de eventos
- (Sin precios en web)

### 2. Planes Mensuales de Contenido
- Servicio recurrente para empresas
- Grabación + edición + distribución
- Contenido mensual constante
- (Sin precios en web)

### 3. Cursos y Entrevistas
- Producción de cursos online
- Entrevistas empresariales
- Podcasts con video
- (Sin precios en web)

### 4. Alquiler de Equipos
- Cámaras, iluminación, audio
- Preferiblemente con operador
- (Sin precios en web)

## Contenido necesario (stock)

### Hero
- Video de fondo: Ambiente de producción audiovisual, cámaras grabando, luces de estudio

### Servicios
- Imágenes representativas de cada servicio
- Estilo profesional, moderno

### Portafolio
- Imágenes de trabajos audiovisuales (corporativos, eventos, etc.)
- Estilo variado para mostrar versatilidad

### Sobre nosotros
- Fotos de equipos de filmación (cámaras, luces, trípodes)
- Imágenes de estudio/espacio de trabajo

## SEO básico

### Title
```
Prisma Media House | Productora Audiovisual en Bogotá
```

### Meta Description
```
Productora audiovisual profesional en Bogotá. Producción de videos corporativos, planes de contenido mensuales, cursos, entrevistas y más. Cotiza tu proyecto.
```

### Open Graph
- Título descriptivo
- Imagen de preview (logo + nombre)
- Descripción para redes sociales

## Deployment

### Vercel
- Repo conectado a GitHub
- Deploy automático en push a main
- Dominio gratuito de Vercel (prisma-media-house.vercel.app)
- SSL incluido
- Edge network global

## Criterios de éxito

1. ✅ Sitio carga en < 3 segundos
2. ✅ Puntuación Lighthouse > 90
3. ✅ Responsive en todos los dispositivos
4. ✅ Modo oscuro/claro funcional
5. ✅ Botón WhatsApp funciona correctamente
6. ✅ SEO básico implementado
7. ✅ Deploy exitoso en Vercel

## Riesgos conocidos

| Riesgo | Impacto | Mitigación |
|--------|---------|------------|
| Sin portafolio propio | Medio | Usar stock + fotos de equipo |
| Sin logo simplificado | Alto | Crear versión simplificada del logo actual |
| Contenido stock genérico | Medio | Seleccionar imágenes de alta calidad y coherentes |
| SEO sin contenido blog | Bajo | Enfocar en SEO local + redes sociales |

## Próximos pasos después del lanzamiento

1. Crear versión simplificada del logo
2. Tomar fotos de equipos propios
3. Generar primeros trabajos para portafolio real
4. Agregar sección de blog para SEO
5. Implementar formulario de contacto alternativo
