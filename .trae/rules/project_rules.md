/// RULES — LOCKED (usar con la PLANTILLA LITERAL pegada por el usuario)

MODO: AISLADO SIN CONTEXTO
- No leas archivos del repositorio. No abras rutas tipo /templates/…. 
- La **única** fuente de verdad es la **plantilla literal** que venga en el mensaje del usuario. 
- Si no hay plantilla literal en el mensaje: responde exactamente **ERROR:NO_INLINE_TEMPLATE**.

CONTRATO DE MAQUETACIÓN (clonar al 100%)
- Mantén **idéntico** el árbol de nodos, clases y estilos inline de la plantilla pegada (no añadir, quitar ni reordenar contenedores).
- Mantén el `<link rel="stylesheet" href="fichas.css">`.
- Mantén estos wrappers y clases (orden exacto): `.sheet > .contenido > .container`, `.header`, `.subtitle`, `.student-info`, `.section`, `.section-title`, `.section-content`, `.prayer-box`, `.bible-quote`, `.story-content`, `.story-image`, `.story-text`, `.activity-box`, `.answer-line`, `.reflection-box`, `.question`.
- Mantén el bloque del logo **idéntico**, con su `<img>` y estilos inline (width 30px, etc.).

QUÉ SÍ PUEDE CAMBIAR (solo contenido):
- `<title>` del documento.
- Textos visibles: H1, subtítulo, oración inicial, cita bíblica, 3 párrafos de historia, “Mensaje principal”, actividad (título, instrucciones, pie/pregunta), 3 preguntas de reflexión, oración final.
- Imagen del personaje: **solo `src` y `alt`** del `<img class="story-image">`.
  - Ruta: `assets/characters/{{slug}}.png`
  - `alt`: nombre del personaje.
  - **No** sustituir por `.illustration` ni tocar tamaños/estilos; el CSS ya define `.story-image`.

QUÉ NO PUEDE CAMBIAR:
- Dimensiones/posición relativas (las decide `fichas.css`).
- Clases, estilos inline existentes, estructura y orden de secciones.
- Campos “Nombre” y “Fecha”.

SALIDA:
- Devuelve **únicamente** el **HTML final** (un archivo). Sin explicaciones ni comentarios extra.

VALIDACIÓN AUTOMÁTICA ANTES DE RESPONDER:
1) Existen y en el mismo orden todos los wrappers y secciones indicados.
2) El enlace a `fichas.css` permanece intacto.
3) Hay exactamente un `<img>` del logo (30px) y un `<img class="story-image">` del personaje.
4) No se introducen clases/estilos nuevos.
5) Solo han variado textos, `<title>`, y `src/alt` del personaje.

ERRORES:
- Si falta la plantilla literal: **ERROR:NO_INLINE_TEMPLATE**.

