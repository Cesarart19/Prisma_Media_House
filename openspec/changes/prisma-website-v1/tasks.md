# Tareas: Sitio Web Prisma Media House v1

## Fase 0: Preparación del proyecto

- [ ] Inicializar proyecto Astro
- [ ] Configurar estructura de carpetas
- [ ] Configurar CSS variables y reset global
- [ ] Configurar tipografía (Inter de Google Fonts)
- [ ] Preparar logo simplificado para header
- [ ] Buscar y descargar video de stock para hero
- [ ] Buscar y descargar imágenes de stock para servicios/portafolio
- [ ] Buscar y descargar fotos de equipos de audio

## Fase 1: Layout base y header

- [ ] Crear BaseLayout.astro (estructura HTML base)
- [ ] Crear Header.astro
  - Logo simplificado
  - Navegación (Servicios, Portafolio, Nosotros, Contacto)
  - Toggle modo oscuro/claro
  - CTA WhatsApp (desktop)
  - Menú hamburguesa (mobile)
- [ ] Implementar lógica de tema (localStorage + prefers-color-scheme)
- [ ] Estilos del header (fijo, blur, responsive)

## Fase 2: Hero section

- [ ] Crear Hero.astro
  - Video de fondo con overlay
  - Título principal
  - Subtítulo
  - CTA WhatsApp
- [ ] Estilos del hero (100vh, centrado, overlay)
- [ ] Animación de entrada

## Fase 3: Servicios

- [ ] Crear Services.astro
  - Tarjeta: Producción de Contenido para Empresas
  - Tarjeta: Planes Mensuales de Contenido
  - Tarjeta: Cursos y Entrevistas
  - Tarjeta: Alquiler de Equipos
- [ ] Estilos de tarjetas (grid, hover, iconos)
- [ ] Iconos SVG para cada servicio
- [ ] Scroll reveal animation

## Fase 4: Portafolio (placeholder)

- [ ] Crear Portfolio.astro
  - Grid de imágenes stock
  - Mensaje: "Próximamente nuestros trabajos"
- [ ] Estilos del grid responsive
- [ ] Lightbox simple (opcional)

## Fase 5: Proceso

- [ ] Crear Process.astro
  - Paso 1: Contactas
  - Paso 2: Cotizamos
  - Paso 3: Produciimos
  - Paso 4: Entregamos
- [ ] Diseño de pasos con línea conectora
- [ ] Animación de scroll reveal

## Fase 6: Sobre nosotros

- [ ] Crear About.astro
  - Misión/Visión breve
  - Valores
  - Equipos que usamos (fotos)
- [ ] Estilos de la sección

## Fase 7: CTA final

- [ ] Crear CTA final (parte de About o componente separado)
  - "¿Listo para crear contenido?"
  - Botón WhatsApp
- [ ] Estilos del CTA

## Fase 8: Footer

- [ ] Crear Footer.astro
  - Logo
  - Redes sociales (links)
  - WhatsApp
  - Email
  - Copyright
- [ ] Estilos del footer

## Fase 9: Botón WhatsApp flotante

- [ ] Crear WhatsAppButton.astro
  - Posición fixed bottom-right
  - Icono WhatsApp SVG
  - Link a WhatsApp con mensaje predefinido
  - Hover effect
- [ ] Z-index y positioning

## Fase 10: SEO y meta tags

- [ ] Agregar meta title
- [ ] Agregar meta description
- [ ] Agregar Open Graph tags
- [ ] Agregar favicon
- [ ] Agregar apple-touch-icon
- [ ] Agregar sitemap básico

## Fase 11: Responsive y testing

- [ ] Probar en mobile (< 768px)
- [ ] Probar en tablet (768px - 1024px)
- [ ] Probar en desktop (> 1024px)
- [ ] Probar modo oscuro/claro
- [ ] Probar navegación
- [ ] Probar CTA WhatsApp
- [ ] Verificar performance (Lighthouse)

## Fase 12: Deploy

- [ ] Crear repositorio en GitHub
- [ ] Push a GitHub
- [ ] Conectar a Vercel
- [ ] Configurar dominio
- [ ] Verificar deploy exitoso
- [ ] Probar URL final

---

## Estimación de tiempo

| Fase | Tiempo estimado |
|------|-----------------|
| Fase 0 | 30 min |
| Fase 1 | 45 min |
| Fase 2 | 30 min |
| Fase 3 | 45 min |
| Fase 4 | 20 min |
| Fase 5 | 30 min |
| Fase 6 | 20 min |
| Fase 7 | 10 min |
| Fase 8 | 20 min |
| Fase 9 | 15 min |
| Fase 10 | 15 min |
| Fase 11 | 30 min |
| Fase 12 | 15 min |
| **Total** | **~5 horas** |

## Notas

- Las imágenes de stock se buscarán en Unsplash, Pexels o Pixabay (gratis)
- El video de hero se buscará en Pexels Videos o Coverr (gratis)
- Las fotos de equipos se buscarán en Unsplash con keywords específicas
- El logo simplificado se creará a partir del logo actual
- Se usará Inter como tipografía principal (Google Fonts)
