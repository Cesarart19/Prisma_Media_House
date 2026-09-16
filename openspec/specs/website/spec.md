# Especificación: Sitio Web Prisma Media House

## Descripción

Landing page de una página para Prisma Media House, productora audiovisual en Bogotá. El sitio sirve como presencia digital para captar leads mediante prospección directa, con WhatsApp como canal principal de contacto.

## Requisitos funcionales

### RF-01: Navegación

- Header fijo al hacer scroll
- Logo simplificado (izquierda)
- Navegación: Servicios, Portafolio, Nosotros, Contacto
- Toggle modo oscuro/claro
- CTA WhatsApp (desktop)
- Menú hamburguesa (mobile)
- Smooth scroll al hacer click en navigation links

### RF-02: Hero

- Video de fondo (stock de producción audiovisual)
- Overlay oscuro semi-transparente
- Título principal: "Producción Audiovisual Profesional"
- Subtítulo: "Transformamos tu idea en contenido que conecta con tu audiencia"
- CTA: "Cotiza tu proyecto" → WhatsApp
- Animación de entrada suave

### RF-03: Servicios

- 4 tarjetas de servicios
  1. Producción de Contenido para Empresas
  2. Planes Mensuales de Contenido
  3. Cursos y Entrevistas
  4. Alquiler de Equipos
- Icono representativo por servicio
- Título y descripción breve
- Sin precios (prospección directa)
- Scroll reveal animation

### RF-04: Portafolio

- Grid de imágenes (stock + fotos de equipo)
- Mensaje: "Próximamente nuestros trabajos"
- Responsive (1-4 columnas según dispositivo)

### RF-05: Proceso

- 4 pasos: Contactas → Cotizamos → Produciimos → Entregamos
- Diseño horizontal con línea conectora
- Números circulares
- Animación al scroll

### RF-06: Sobre nosotros

- Misión/Visión breve
- Valores (calidad, creatividad, puntualidad, etc.)
- Equipos que usamos (fotos reales o stock)

### RF-07: CTA final

- "¿Listo para crear contenido?"
- Botón WhatsApp
- Fondo diferenciado

### RF-08: Footer

- Logo
- Redes sociales (Instagram, Facebook, TikTok, YouTube)
- WhatsApp
- Email
- Copyright

### RF-09: Botón WhatsApp flotante

- Posición: Fixed, bottom-right
- Color: WhatsApp green (#25D366)
- Icono: WhatsApp SVG
- Hover: Scale ligeramente
- Siempre visible (z-index alto)

### RF-10: Modo oscuro/claro

- Toggle en header (icono sol/luna)
- Preferencia guardada en localStorage
- Respeta prefers-color-scheme del sistema
- Transición suave (0.3s)
- Todos los componentes respetan el tema

## Requisitos no funcionales

### RNF-01: Performance

- Carga inicial < 3 segundos
- Lighthouse score > 90
- Imágenes optimizadas (WebP/AVIF si es posible)
- Video de hero comprimido
- Lazy loading en imágenes

### RNF-02: Responsive

- Mobile: < 768px (1 columna)
- Tablet: 768px - 1024px (2 columnas)
- Desktop: > 1024px (layout completo)

### RNF-03: SEO

- Meta title descriptivo
- Meta description con keywords
- Open Graph tags
- Sitemap básico
- Favicon
- Apple-touch-icon

### RNF-04: Accesibilidad

- Contraste mínimo 4.5:1 (WCAG AA)
- Focus visible en elementos interactivos
- Alt text en imágenes
- Navegación por teclado
- Respetar prefers-reduced-motion

### RNF-05: Navegador

- Chrome (últimas 2 versiones)
- Firefox (últimas 2 versiones)
- Safari (últimas 2 versiones)
- Edge (últimas 2 versiones)

## Contenido necesario

### Video hero

- Temática: Producción audiovisual, cámaras grabando, luces de estudio
- Duración: 10-30 segundos (loop)
- Calidad: HD (1080p)
- Fuente: Pexels Videos, Coverr (gratis)

### Imágenes stock

- Servicios: Producción, reuniones, cámaras, cursos
- Portafolio: Eventos, videos corporativos, fotos profesionales
- Sobre nosotros: Equipos de filmación, estudios
- Fuente: Unsplash, Pexels, Pixabay (gratis)

### Fotos propias

- Equipos de audio que posee la empresa
- (Temporal: usar stock hasta tener fotos propias)

## URLs de contacto

- WhatsApp: `https://wa.me/57XXXXXXXXXX?text=Hola,%20me%20interesa%20un%20servicio%20de%20producción%20audiovisual`
- Instagram: `(pendiente)`
- Email: `(pendiente)`

##Deploy

- Plataforma: Vercel
- Framework: Astro 5.x
- Repo: GitHub
- Dominio: prisma-media-house.vercel.app (temporal)
- SSL: Automático
- Deploy: Automático en push a main
