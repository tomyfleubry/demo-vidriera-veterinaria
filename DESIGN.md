# DESIGN.md — Vidriera veterinaria "Clínica Veterinaria Alba" (v2)

Sistema de diseño destilado de AniCura (estructura clínica premium) + criterios de la
investigación de videos 2026-10-26 (DESIGN.md antes del código · checklist anti-slop).

## Diales
- Varianza: 6/10 (asimétrico con criterio: hero desplazado, tarjeta flotante, radios variados)
- Movimiento: 5/10 (scroll suave Lenis, reveals GSAP escalonados, contadores, parallax leve; nada gratuito)
- Densidad: 4/10 (aire generoso, una idea por pantalla)

## Tokens
- Color: teal profundo `#0B4F4A` (primario), teal vivo `#0E6A62` (hover/enlaces),
  superficies menta `#E7F4F1` / `#D3ECE6`, tinta `#17322F`, mutado `#5B7370`,
  ámbar `#F2A93B` (solo acentos y estrellas), fondo `#FBFCFB`.
- Tipografía: display **Fraunces** (serif con carácter, titulares) + **Manrope** (texto).
  Escala modular 1.25: 0.875 / 1 / 1.125 / 1.4 / 1.9 / 2.6 rem. Titulares: letter-spacing −0.02em.
- Radios: 14 (chips/íconos), 20 (tarjetas), 28 (paneles grandes). No un solo radio para todo.
- Sombras: suaves en teal `rgba(11,79,74,.10)`, una sola dirección de luz.
- Botones: pastilla, primario teal; WhatsApp verde `#22C064` solo en CTAs de turno (hero, cierre, flotante).

## Reglas anti-slop aplicadas
- Nada de emojis como íconos: set SVG de trazo 1.7 en color de marca.
- Sin gradiente índigo→violeta; sin glassmorphism decorativo (la tarjeta flotante del hero
  es blanca sólida con sombra).
- Tipografía deliberada, nunca el stack del sistema como display.
- Copy específico ("diagnóstico en el día") en vez de adjetivos vacíos; una pantalla = una acción (WhatsApp).
- Equipo con fotos; ningún bloque importante queda solo en texto.

## Movimiento
- Lenis (scroll suave) + GSAP ScrollTrigger (CDN, gratis): reveals por sección,
  contadores animados en la franja de cifras, parallax leve + ken-burns en la foto del hero.
- Todo el movimiento se apaga con `prefers-reduced-motion` y la página se lee completa sin JS.
