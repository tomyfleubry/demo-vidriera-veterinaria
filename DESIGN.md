---
name: "Clínica Veterinaria Alba — Clínica práctica"
description: "Recepción clínica cercana, con datos claros y acciones inmediatas."
colors: {"teal":"#0b4f4a","teal-2":"#0e6a62","mint":"#e7f4f1","mint-2":"#d3ece6","ink":"#17322f","muted":"#5b7370","bg":"#fbfcfb","card":"#ffffff","amber":"#f2a93b","wa":"#22c064","amber-light":"#ffd98a","inverse-text":"#eafaf6","footer-bg":"#0a3d39","footer-text":"#cfe8e2","urgent-wash":"rgba(242,169,59,.12)"}
typography: {"display":{"fontFamily":"Fraunces, serif","fontSize":"45px","fontWeight":600,"lineHeight":1.15,"letterSpacing":"-0.02em"},"headline":{"fontFamily":"Fraunces, serif","fontSize":"40px","fontWeight":600,"lineHeight":1.15,"letterSpacing":"-0.02em"},"title":{"fontFamily":"Fraunces, serif","fontSize":"23px","fontWeight":600,"lineHeight":1.2,"letterSpacing":"-0.02em"},"body":{"fontFamily":"Manrope, sans-serif","fontSize":"16px","fontWeight":400,"lineHeight":1.65},"label":{"fontFamily":"Manrope, sans-serif","fontSize":"14px","fontWeight":600,"lineHeight":1.65},"button":{"fontFamily":"Manrope, sans-serif","fontSize":"15px","fontWeight":700,"lineHeight":1.4}}
rounded: {"sm":"14px","md":"20px","lg":"28px","pill":"999px","thumbnail":"10px","circle":"50%"}
spacing: {"12":"12px","20":"20px","24":"24px","28":"28px","32":"32px","55":"55px","80":"80px"}
components: {"button-primary":{"backgroundColor":"{colors.teal}","textColor":"{colors.card}","typography":"{typography.button}","rounded":"{rounded.pill}","padding":"12px 22px"},"button-primary-hover":{"backgroundColor":"{colors.teal-2}"},"button-wa":{"backgroundColor":"{colors.wa}","textColor":"{colors.ink}","typography":"{typography.button}","rounded":"{rounded.pill}","padding":"12px 22px"},"button-wa-hover":{"backgroundColor":"{colors.mint-2}"},"button-emergency":{"backgroundColor":"{colors.amber}","textColor":"{colors.ink}","typography":"{typography.button}","rounded":"{rounded.pill}","padding":"12px 22px"},"button-emergency-hover":{"backgroundColor":"{colors.amber-light}"},"button-ghost":{"backgroundColor":"{colors.card}","textColor":"{colors.teal}","typography":"{typography.button}","rounded":"{rounded.pill}","padding":"12px 22px"},"button-ghost-hover":{"backgroundColor":"{colors.mint}"},"data-card":{"backgroundColor":"{colors.card}","textColor":"{colors.ink}","rounded":"{rounded.md}","padding":"30px"},"specialty-row":{"textColor":"{colors.ink}","padding":"30px 0"},"navigation":{"backgroundColor":"{colors.card}","textColor":"{colors.ink}","typography":"{typography.label}"}}
---

# Design System: Clínica Veterinaria Alba — Clínica práctica

## Overview

**Creative North Star: "Clínica práctica"**

La recepción organiza el recorrido: datos prácticos y decisión entre turno y urgencia al abrir, luego cada servicio con su consulta preparada. Fraunces aporta calidez; Manrope sostiene la lectura y las acciones. La tarjeta de datos es deliberadamente el foco del hero.

Tomas fijó identidad, estructura, contenido y orden antes del HTML, y eligió expresamente una tabla con diez servicios/áreas. Esta actualización concilia ese sistema con el código final; no elige otra dirección. La copia inmutable anterior al código permanece en ../../.pipeline/alba-clinica-practica/DESIGN-primero.md. El molde de esta vidriera se mantiene diferenciado de Mora, Aura, Bruma y las otras muestras.

**Key Characteristics:**
- Datos y acciones antes de la fotografía en móvil.
- Paleta original teal, menta, blanco y ámbar; fotografía clínica ilustrativa.
- Información abierta y una acción asociada a cada fila.
- Profundidad suave en la tarjeta funcional; apoyos planos.

**Procedencia.** PRODUCT.md conserva los hechos confirmados de esta vidriera ficticia. El frontmatter captura valores reales del CSS final y es normativo. La intención previa de lectura (16px, interlínea 1.6 y medida orientativa de 65ch) se conserva como antecedente: el cuerpo implementado usa 1.65, la bajada móvil 1.6, la bajada 62ch y el texto secundario 70ch. El piso previo de botones de 44px se conserva; las alturas reales son mayores.

qa-local.json registra PASS en 1440, 768, 430 y 390px: sin overflow de página, diez áreas, diecisiete enlaces WhatsApp y doce imágenes. finish-review.md pidió auxiliares de 13px y estrellas SVG; finish-verdict.md puntuó ambos resolved, con disposition ship limitado a esos dos fixes. Este pase documental cotejó código y registros; no repitió QA ni la inspección de capturas. El detector corrió una vez antes del lote y no se repitió.

## Colors

Paleta clínica cercana: teal profundo, menta tranquila, superficies claras y ámbar operativo. Los valores exactos viven en el frontmatter.

### Primary

- **Teal clínico** (teal): títulos, marca, botones por especialidad, franja de cifras, topbar y cierre.
- **Teal de interacción** (teal-2): hover primario, etiquetas, iconos y foco global.

### Secondary

- **Ámbar de urgencia** (amber): acciones urgentes y selección de texto; amber-light ilumina su hover y el énfasis de topbar.
- **Verde WhatsApp** (wa): reserva y acción fija; hover en menta de apoyo.

### Neutral

- **Menta clínica / de apoyo** (mint, mint-2): hero, equipo, bordes y estados suaves.
- **Tinta clínica / secundaria** (ink, muted): lectura y detalles.
- **Fondo claro / blanco funcional** (bg, card): suelo y tarjeta/header.
- **Inverso suave** (inverse-text): topbar y leyendas sobre teal.
- **Teal y menta de pie** (footer-bg, footer-text): footer conservado.
- **Lavado urgente** (urgent-wash): ámbar al 12% sobre el fondo.

**The Original Palette Rule.** Conservar los colores de Alba; el ámbar identifica urgencia sin introducir rojo.

Las rampas tonales del sidecar son muestras generadas para el panel; no amplían la paleta implementada.

## Typography

**Display Font:** Fraunces, respaldo serif; hoja existente con pesos 500/600/700 y eje óptico 9–144. Los titulares usan 600.
**Body Font:** Manrope, respaldo sans-serif; hoja existente 400–800, cuerpo 400 y acciones 700.

- **Display:** token de escritorio; titular 45px, 39px hasta 1100px, 34px hasta 760px y 31px hasta 400px. Medida 20ch, 23ch móvil; énfasis cursivo original.
- **Headline:** sección 40px/32px móvil. Tarjeta 29/25px, banda urgente 30/29px, proceso 36/31px y cierre 42/35px.
- **Title:** filas 23px con interlínea 1.2, 24px móvil. H3 general 24px; pasos, instalaciones y equipo conservan ajustes de 21–23px por bloque y anchura.
- **Body:** 16px/1.65. Bajada 16px y 15px/1.6 móvil, máximo 62ch; secundario 70ch y cierre 60ch. Descripciones de filas abiertas.
- **Label:** navegación 14px/600; kicker 15px/700; roles 14px/700 y 13px móvil.
- **Button:** 15px/700, interlínea 1.4. Header móvil 13px; tarjeta 17px escritorio, 14px móvil y 13px hasta 400px.
- **Auxiliares:** los corregidos quedan en 13px como mínimo. Descriptor de marca 13px/700/1.5, tracking .07em; se oculta solo en el header hasta 760px y permanece completo en el footer. La antigua mención a 11px quedó superada por esa corrección. La nota del rating usa 13px/1.5.

## Layout

Contenedor de hasta 1140px, ancho disponible menos 64px; hasta 760px resta 40px. Bloques principales con 80px verticales, 55px móvil. El espaciado del frontmatter recoge medidas repetidas observadas, sin imponer una escala nueva.

Hero con 44px/52px de aire vertical, grilla 1.12fr/.88fr, dos filas y separación 28px/48px: titular y bajada a izquierda, foto debajo; tarjeta a derecha sobre ambas filas. Hasta 1100px la separación es 28px. Hasta 760px es una columna, con titular, tarjeta y foto en ese orden, aire 27px/35px y foto 3:2.

### Orden aprobado de esta vidriera

1. **Hero:** suelo menta y tarjeta blanca protagonista. «Pedir turno» y «Urgencias 24 h», esta última ámbar con tinta clínica. En 430px los datos/acciones preceden a la foto. Sin contadores ni rating flotante al abrir.
2. **Urgencias:** banda inmediatamente posterior, ámbar al 12%, texto teal y botón ámbar grande; textos actuales conservados.
3. **Especialidades:** fondo claro; «Todo lo que tu mascota necesita, en un solo lugar». Tabla visual continua de diez filas (tres servicios y siete áreas), con nombre, descripción, prestaciones y turno por fila. «Especialistas que trabajan en equipo» y su introducción permanecen. Grooming queda estático como apoyo del bloque, con título y prestaciones; se retira la instrucción del control eliminado, sin reescribirla.
4. **Cifras:** franja fina teal, cifras blancas, una fila y overflow interno en celular. Conserva +15, +12.000, 4,9/5, 24/7 e internación propia. 6 y 14 permanecen en las introducciones de especialidades/equipo.
5. **Proceso:** cuatro pasos 01–04 horizontales, dos columnas móviles, fondo claro y sin tarjetas pesadas. Textos e imágenes de instalaciones quedan como apoyo dentro del bloque, sin añadir otro tramo principal.
6. **Equipo:** menta, cuatro fotografías en fila, dos columnas móviles; nombres, roles, descripciones y opiniones ficticias preservados.
7. **Cierre:** teal profundo, titular/texto original y turno.
8. **Footer:** fondo y botón urgente conservados, aclaración ficticia literal y 6rem de aire inferior.

Filas en .9fr/1.5fr/auto, gap 30px; hasta 1100px, 1fr/1.25fr/auto y 22px. Hasta 760px se apilan nombre, contenido y acción. Instalaciones: tres columnas, luego una con foto de 110px junto al texto. Equipo: cuatro/dos columnas; opiniones: tres/una. Las cifras desplazan su contenedor, sin overflow de página en 430px según QA.

Header sticky; navegación oculta hasta 1100px, sin menú alternativo añadido. CTA de cabecera en una línea. Anclas con scroll-margin-top de 120px. Breakpoints observados: max-width 1100, 760 y 400px.

**The Reception Focus Rule.** La tarjeta de datos sigue siendo el foco del hero; no agrandar el titular ni cambiar la composición para desplazarla.

## Elevation & Depth

Bandas, fotografía y reglas menta de 1px construyen profundidad. La tarjeta usa la sombra teal suave de --shadow; la acción fija de WhatsApp, sombra negra compacta. Ambas expresiones exactas están en extensions.shadows del sidecar. Proceso, grooming, instalaciones, equipo y opiniones permanecen abiertos.

**The Soft Depth Rule.** La sombra teal sostiene la tarjeta funcional; no añadir vidrio decorativo ni tarjetas pesadas a los apoyos.

## Shapes

Fotografía y marca usan radio pequeño (14px); tarjeta funcional mediano (20px), acciones pastilla (999px), flotante circular y miniaturas de servicio (10px). El radio original de 28px sigue declarado aunque este molde no lo aplica a una superficie visible. No usarlo para inventar nuevos contenedores. La foto del hero conserva su proporción original 3:2 para no cortar caras ni perro; no hay animales recortados ni siluetas decorativas.

## Components

### Buttons

Pastillas de peso 700 con icono SVG junto al texto. Base teal/blanco; WhatsApp verde/tinta; urgencia ámbar/tinta. Ghost está definido en CSS (blanco/teal, borde menta de 1px y hover menta), aunque no se instancia en esta página.

Altura mínima base 48px; filas con ancho mínimo 130px. Tarjeta: 57px turno y 64px urgencia; móvil, ambas 54px. Banda urgente: 60px y ancho completo móvil. Hover: fondo del token y translateY(-2px), transición .2s. Foco global: contorno teal de 3px, offset 5px; cierre/footer usan ámbar.

### Cards / Containers

Tarjeta de datos blanca, radio mediano y sombra teal; padding 30px, 26px hasta 1100px, 22px hasta 760px y 20px hasta 400px. Lista abierta con iconos, gap 19px/12px móvil. Acciones al pie mediante margen automático, padding superior 28px; móvil en dos columnas con 22px superiores. El espacio de escritorio entre datos y acciones forma parte de la composición aceptada: no rellenarlo.

### Navigation

Marca Fraunces; enlaces Manrope 14px/600, gap 20px; hover subrayado con offset 5px y foco global. Header blanco con regla menta; topbar teal con urgencia y contacto. CTA y auxiliares móviles corregidos a 13px. El descriptor completo «Clínica y hospital veterinario» permanece en footer.

### Filas, proceso y opiniones

Diez filas abiertas: Consulta y medicina preventiva; Vacunación y planes de salud; Traumatología y curaciones; Medicina interna; Cirugía general y de tejidos blandos; Oftalmología; Cardiología; Odontología; Medicina felina; Diagnóstico por imágenes y laboratorio propio. Tres primeras con miniatura; siete áreas sin fotos grandes ni paneles ocultos. Borde superior menta y borde inferior en la última fila. No hay inputs ni formularios que documentar.

Se conservan las seis URLs originales a https://wa.me/5491100000000. Solo las etiquetas del hero/urgencias cambian según el brief; se añade una urgencia en hero y diez enlaces con nombres exactos y el mensaje «Hola! Quiero pedir un turno de [ESPECIALIDAD] para mi mascota.». Número, cierre, footer y flotante no cambian. No se contacta a nadie.

Cifras en Fraunces con números tabulares. Proceso como lista ordenada con numeración CSS 01–04 en Fraunces de 45px y nombres H3. Cada opinión mantiene cinco estrellas SVG de 16px en teal de interacción, grupo con nombre accesible «5 de 5» y SVG decorativos ocultos; textos y valoraciones intactos.

### Fotografías y procedencia

| Archivo | Uso actual |
|---|---|
| p6234611.jpg | Clínica del hero, sin recortes de animales, proporción 3:2. |
| p7469229.jpg | Miniatura de Consulta y medicina preventiva. |
| p7469223.jpg | Miniatura de Vacunación y planes de salud; archivo reemplazado. |
| p7474857.jpg | Miniatura de Traumatología; corrección anterior intacta. |
| p6816860.jpg | Grooming estático, sin comparación. |
| p6235232.jpg | Consultorios y diagnóstico, apoyo del proceso. |
| p6235649.jpg | Diagnóstico, apoyo de Quirófano e internación; no acredita una cirugía. |
| p6816869.jpg | Espacio felino, apoyo del proceso. |
| equipo-1.jpg a equipo-4.jpg | Cuatro perfiles actuales, intactos e ilustrativos. |

**Reemplazo de «VOLUNTEER».** El registro previo consigna que img/p7469223.jpg fue sobrescrito con **A Veterinarian Checking a Dog**, **Tima Miroshnichenko**, [Pexels 6234622](https://www.pexels.com/photo/a-veterinarian-checking-a-dog-6234622/), bajo [licencia Pexels](https://www.pexels.com/license/). Se eligió, decodificó y abrió antes del HTML. JPEG de 1400px de una revisión bucal de un perro: es una consulta, no prueba una vacuna. Según la selección registrada, no hay palabras legibles en la ropa ni marca de otra clínica y no lleva barbijo. Se conserva sin retoque.

p7469274.jpg se retiró de la página por la remera con texto; queda sin uso y se sustituyó por p6235649.jpg ya existente. Los otros JPEG quedan guardados sin uso. No se incorporaron fotos nuevas fuera del reemplazo exigido. Las restantes fotos son heredadas de Pexels: el registro no conserva todas las URLs/autores y no se inventan atribuciones. Se retiraron del footer créditos de recortes de hero eliminados; permanece el crédito de consulta. Todas son ilustrativas.

### Movimiento y accesibilidad

GSAP 3.12.5, ScrollTrigger y Lenis 1.1.14 existentes, sin nuevas librerías: entradas leves desde contenido visible, contadores originales y movimiento suave de la foto. Las expresiones exactas están en extensions.motion. prefers-reduced-motion apaga movimiento y transiciones; sin JS todo queda legible y enlazado.

No quedan filtros, roles tab/tabpanel, slider ni eventos de comparación. Se conservan es-AR, noindex/nofollow y la aclaración literal: «Vidriera de demostración de Nexvia IA · Marca, personas y datos ficticios.»

## Do's and Don'ts

### Do:

- **Do** conservar paleta, Fraunces/Manrope, voseo, textos y carácter de recepción elegido por Tomas.
- **Do** mantener diez filas visibles con nombres, descripciones, prestaciones y mensajes de turno exactos.
- **Do** mantener datos y las dos acciones antes de la foto en móvil, foco visible y movimiento reducido.
- **Do** conservar fotografía clínica 3:2, perfiles y opiniones ficticias, cifras y aclaración literal del footer.

### Don't:

- **Don't** sustituir la tarjeta protagonista por un hero de titular o foto mayor.
- **Don't** reintroducir comparador, filtros, pastillas de selección, paneles ocultos, roles tab/tabpanel ni instrucciones de arrastre.
- **Don't** añadir rojo, vidrio decorativo, tarjetas pesadas de proceso ni fotos grandes de especialidad.
- **Don't** inventar precios, pacientes, prestaciones, atribuciones o prueba social, ni reutilizar este molde en las otras vidrieras.
- **Don't** usar estrellas tipográficas: conservar cinco SVG por opinión y el nombre accesible «5 de 5».

### Corrección del ícono de WhatsApp

Se reemplaza el trazado heredado por el SVG de WhatsApp de Bootstrap Icons (MIT),
con viewBox16×16 propio en cada aparición, proporción centrada, fill currentColor
y sin stroke. Las18apariciones incluyen17enlaces y el dato de contacto. Se
conservan tamaños y colores por contexto; sin cambios de textos, enlaces ni diseño.
Licencia y procedencia en THIRD-PARTY-LICENSES.txt.
