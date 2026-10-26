# DESIGN.md — Vidriera peluquería "Estudio Aura" (v2)

Sistema de diseño destilado de Llongueras (cadena premium: tipografía editorial,
servicios por especialidad, reserva simple) + criterios de la investigación de
videos 2026-10-26 (DESIGN.md antes del código · checklist anti-slop).

## Diales
- Varianza: 6/10 (hero desplazado con tarjeta flotante, grillas asimétricas, radios variados)
- Movimiento: 5/10 (Lenis, reveals GSAP escalonados, contadores, ken-burns + parallax en hero)
- Densidad: 4/10 (aire generoso, una idea por pantalla)

## Tokens
- Color: marfil cálido `#FAF6F0` (fondo), espresso `#2B211B` (tinta), cobre `#B07D4F`
  (primario), cobre oscuro `#96683E` (hover), superficies arena `#F2E8DC` / `#EADCC9`,
  mutado `#7A6A5E`. Sin dorado chillón: cobre mate.
- Tipografía: display **Cormorant Garamond** (editorial, titulares grandes con itálica
  de acento) + **Manrope** (texto). Escala modular 1.25. Titulares letter-spacing −0.01em.
- Radios: 14 (chips/íconos), 20 (tarjetas), 28 (paneles). Sombras suaves en espresso
  `rgba(43,33,27,.10)`, una sola dirección de luz.
- Botones: pastilla, primario cobre; WhatsApp verde `#22C064` solo en CTAs de turno
  (hero, cierre, flotante).

## Reglas anti-slop aplicadas
- Cero emojis como íconos: set SVG de trazo 1.7 en color de marca.
- Sin gradiente índigo→violeta, sin glassmorphism decorativo (tarjeta del hero sólida).
- Servicios con fotos reales y tamaños variados, no 3 tarjetas idénticas.
- Copy específico ("balayage sin decolorar de más") en vez de adjetivos vacíos.
- Equipo con fotos; ningún bloque importante queda solo en texto.

## Componente del rubro
- **Comparador antes/después arrastrable** (clip-path): "En proceso / Resultado"
  del color — el componente fijo de peluquería según la investigación.

## Movimiento
- Lenis + GSAP ScrollTrigger por CDN: reveals por sección, contadores en la franja
  de cifras, parallax leve + ken-burns en la foto del hero.
- Se apaga con `prefers-reduced-motion`; la página se lee completa sin JS.

## Datos (ficticios, vidriera)
- Marca: **Estudio Aura — Peluquería & Color**. Av. Santa Fe 2450, Recoleta (ficticio).
- Teléfono placeholder +54 9 11 0000-0000 (wa.me/5491100000000), a reemplazar por el
  cliente real. Equipo ficticio: Martina Ríos (color), Camila Duarte (corte y peinado),
  Valentina Sosa (tratamientos). Horario ficticio: mar–sáb 9:00–20:00.
- Fotos: Pexels (libres), verificadas JPEG. noindex/nofollow. Español argentino (voseo).
