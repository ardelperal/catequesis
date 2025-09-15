# Proyecto de Catequesis - Fichas de Personajes Bíblicos

Este proyecto contiene fichas interactivas de personajes bíblicos para catequesis, diseñadas especialmente para niños de 12-13 años en el curso de Confirmación.

## 📁 Estructura del Proyecto

```
catequesis/
├── fichas/              # Fichas HTML de personajes bíblicos
├── assets/characters/   # Ilustraciones y archivos de licencia
├── templates/           # Plantillas HTML base
├── .gitignore          # Archivos ignorados por Git
├── mcps.example        # Configuración MCP de ejemplo
└── README.md           # Este archivo
```

## 🚀 Configuración Inicial

1. **Copia el archivo de configuración:**
   ```bash
   cp mcps.example mcps
   ```

2. **Configura tu token de GitHub (opcional):**
   - Edita el archivo `mcps`
   - Reemplaza `TU_TOKEN_AQUI` con tu token personal de GitHub
   - El archivo `mcps` está en `.gitignore` para proteger tus credenciales

## 📖 Fichas Disponibles

### Personajes del Antiguo Testamento
- **Patriarcas:** Aarón, Abraham, Daniel, David, José, Moisés
- **Profetas:** Elías, Eliseo, Ezequiel, Isaías, Jeremías
- **Otros:** Débora, Ester, Gedeón, Jonás, Rut, Sansón, Salomón

### Personajes del Nuevo Testamento
- **Jesús:** Nacimiento, Bautismo, Tentaciones, Milagros, Transfiguración, Última Cena, Pasión y Muerte, Resurrección, Ascensión
- **Apóstoles:** Pedro, Juan, Santiago, Pablo
- **Otros:** Juan Bautista, María, María Magdalena

## 🎨 Características de las Fichas

- **Diseño moderno** con gradientes y tipografía atractiva
- **Texto justificado** para mejor legibilidad
- **Ilustraciones coloridas** de cada personaje
- **Secciones organizadas:** Oración inicial, historia, actividad creativa, reflexión
- **Compatibilidad de impresión** en formato A4
- **Emojis** para hacer más atractivo el contenido

## 🖼️ Ilustraciones

Las ilustraciones están almacenadas en `assets/characters/` con:
- Formato PNG de alta calidad (≥1200×1600 px)
- Archivos de licencia correspondientes (.license.json)
- Contenido apropiado para niños

## 📝 Plantillas

Las plantillas base están en `templates/`:
- `plantilla_ficha.html` - Plantilla principal
- `plantilla_apostoles.html` - Para apóstoles
- `plantilla_jesus.html` - Para eventos de Jesús
- `plantilla_patriarcas.html` - Para patriarcas
- `plantilla_profetas.html` - Para profetas

## 🔧 Desarrollo

Para contribuir al proyecto:

1. Clona el repositorio
2. Configura el archivo `mcps` según tus necesidades
3. Usa las plantillas existentes para crear nuevas fichas
4. Mantén la consistencia en el formato y estilo

## 📄 Licencia

Este proyecto está diseñado para uso educativo en contextos de catequesis católica. Las ilustraciones tienen sus respectivas licencias documentadas en los archivos `.license.json`.

## 🤝 Contribuciones

Las contribuciones son bienvenidas. Por favor:
- Mantén el formato estándar de las fichas
- Incluye ilustraciones apropiadas con sus licencias
- Verifica la fidelidad doctrinal del contenido
- Prueba la compatibilidad de impresión

---

*Proyecto desarrollado para la formación catequética de jóvenes en preparación para el sacramento de la Confirmación.*