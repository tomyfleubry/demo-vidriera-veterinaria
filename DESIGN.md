# DESIGN.md — Vidriera veterinaria "Clínica Veterinaria Alba" (v3)

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
- Botones: pastilla, primario teal; WhatsApp verde `#22C064` en CTAs de turno.
  La extensión v3 suma un CTA ámbar de urgencias en el footer.

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

## Extensión v3 — técnicas de Mora, identidad Alba

La identidad sigue siendo teal `#0B4F4A` / `#0E6A62`, ámbar `#F2A93B`,
Fraunces y Manrope. Se conserva la composición clínica y todo el contenido
fuera de los ocho ajustes solicitados. Mora aporta técnicas, no sus colores.

- **Hero:** la foto clínica existente toma un remate en arco. Un perro blanco
  y un gato atigrado de Pexels, con alfa real y contornos suaves, cruzan su
  borde inferior. Dos escalas y apoyo en una misma base; sin círculos, bordes
  de sticker ni fondos rectangulares. La valoración conserva una tarjeta
  blanca sólida sin cruzarse con los animales. El titular, texto y CTA no cambian.
- **Datos del hero:** tres columnas iguales; cada dato ocupa dos líneas con
  el mismo ritmo en 430 px. «Internación propia» no queda aislada.
- **Prueba social:** se afina la franja existente en cuatro datos: +15 años,
  +12.000 pacientes, 4,9/5 y guardia 24/7. Son cifras ya presentes. Los datos
  de seis especialidades y 14 profesionales se conservan en sus secciones.
- **Especialidades:** píldoras teal sobre menta, con estado activo sólido y
  foco visible. En móvil hay desplazamiento horizontal dentro del control.
  Siete paneles (las seis especialidades existentes y diagnóstico), cada uno
  con foto grande y contenido breve. No se suman prestaciones. La foto es
  ilustrativa, no se presenta como registro de un procedimiento específico.
  Tabs con teclado, ARIA y contenido completo como alternativa sin JS.
- **Urgencias:** secuencia real en lista ordenada 01–04: estabilización,
  diagnóstico, internación si hace falta y alta acompañada. Números Fraunces
  en teal, texto Manrope; cuatro columnas en escritorio, lista en celular.
- **Grooming:** círculo ámbar de 60 px, flechas SVG y anillo blanco para
  separar el control de las fotos. Divisor más ancho, etiquetas «Antes» y
  «Después» sobre superficies teal sólidas. Se preservan ambos archivos,
  el arrastre y los incrementos de cuatro puntos con flechas.
- **Footer:** CTA «Urgencias 24 h» con el mismo WhatsApp ficticio.
- **Movimiento:** las nuevas entradas usan el `data-reveal` existente; los
  filtros cambian contenido sin depender de GSAP. Se conservan versiones,
  integración de Lenis y la corrección del doble suavizado de la rueda.

### Invariantes de esta extensión

Anclas a 120 px; padding inferior de footer a 6rem; CTA del header sin
partirse; sin overflow de página a 430 px. Se preservan los archivos de
Traumatología `img/p7474857.jpg`, equipo `img/equipo-2.jpg` y grooming,
el nombre, dirección, horarios, WhatsApp placeholder y aclaración de vidriera.

### Nuevas fotos: recortes del hero

| Archivo | Autor y fuente | Tratamiento |
|---|---|---|
| `img/hero-perro.webp` | Jay Brand, [Studio Portrait of a Fluffy White Dog on Black Background](https://www.pexels.com/photo/studio-portrait-of-a-fluffy-white-dog-on-black-background-37427164/) | Recorte de fondo con asistencia de imagen, alfa orgánico; WebP optimizado. |
| `img/hero-gato.webp` | Jem Perez, [Sitting Cat on White Background](https://www.pexels.com/photo/sitting-cat-on-white-background-16260957/) | Recorte de fondo con asistencia de imagen, alfa orgánico; WebP optimizado. |

Ambas fotos bajo [licencia Pexels](https://www.pexels.com/license/).
Son imágenes ilustrativas para una marca ficticia; no son pacientes de Alba.
Los paneles reutilizan las fotos de Pexels ya presentes en el proyecto.
