 La plantilla vive en /templates/plantilla_ficha.html y **debe leerse** en cada generación.
- Prohibido añadir o quitar secciones. Solo rellenar tokens.
- Si el archivo no existe, responde: ERROR:NO_TEMPLATE_FOUND.

## Ilustraciones (color)
- Preferencia: **color** (line art + color plano). Si sólo hay B/N CC0/DP, usar `image_gen` para colorear o recrear a color.
- Origen permitido: Wikimedia Commons, Openclipart, Pixabay (licencia Pixabay), Rawpixel Public Domain, Met Museum (OASC), Rijksmuseum, Cleveland Museum of Art.
- Archivo final: PNG, ≥1200×1600 px, sRGB, fondo transparente o blanco, guardado en `/assets/characters/<slug>.png`.
- Registrar licencia en `/assets/characters/<slug>.license.json` {source_url,title,author,license}.
- Insertar en la plantilla sustituyendo `.illustration` por `<img>` 120×160 (CSS ya dado).
- Contenido seguro para niños; sin sangre; paleta suave; sin degradados intensos.
