# Rutas FIFA 2026 — Guadalajara

Página web interactiva para visualizar rutas de traslado en Guadalajara durante el evento FIFA 2026.

## 📋 Características

- ✅ **Mapa interactivo** con 15 ubicaciones (aeropuertos, hoteles, estadios, etc.)
- ✅ **3 rutas preestablecidas** para cada combinación origen-destino (Principal, Secundaria, Terciaria)
- ✅ **Información detallada** de cada ruta (distancia, tiempo estimado, instrucciones paso a paso)
- ✅ **Links directos a Google Maps** para cada ruta
- ✅ **Diseño responsivo** para escritorio y móvil
- ✅ **Mapa OpenStreetMap** sin necesidad de claves de API

## 🚀 Despliegue en GitHub Pages

### Opción 1: Despliegue automático (Recomendado)

1. **Crea un repositorio en GitHub**
   - Ve a https://github.com/new
   - Nombre del repositorio: `rutas-fifa-2026` (o el que prefieras)
   - Selecciona "Public"
   - Haz clic en "Create repository"

2. **Sube los archivos**
   ```bash
   # Clona el repositorio
   git clone https://github.com/tu-usuario/rutas-fifa-2026.git
   cd rutas-fifa-2026
   
   # Copia los archivos
   cp index.html .
   
   # Sube los cambios
   git add .
   git commit -m "Agregar página de rutas FIFA 2026"
   git push origin main
   ```

3. **Habilita GitHub Pages**
   - Ve a tu repositorio en GitHub
   - Abre "Settings" → "Pages"
   - En "Source", selecciona "Deploy from a branch"
   - Selecciona "main" como rama
   - Haz clic en "Save"

4. **Accede a tu sitio**
   - Tu sitio estará disponible en: `https://tu-usuario.github.io/rutas-fifa-2026/`

### Opción 2: Despliegue manual

1. **Descarga este archivo (`index.html`)**
2. **Sube a tu servidor web** (cualquier hosting que soporte HTML estático)
3. **Accede a través de tu dominio**

## 📁 Estructura de archivos

```
rutas-fifa-2026/
├── index.html          # Página principal (único archivo necesario)
└── README.md           # Este archivo
```

## 🗺️ Ubicaciones incluidas

1. ✈️ Aeropuerto Internacional de Guadalajara
2. 🛡️ Base Aérea Militar de Zapopan
3. ✈️ Aeropuerto Puerto Vallarta
4. 🏨 Hyatt Regency Andares
5. 🏨 Hilton Midtown
6. 🏨 JW Marriott
7. 🏨 Grand Fiesta Americana
8. 🏨 The Westin
9. 🏨 AC Hotel Expo
10. 🏨 Fiesta Inn Expo
11. 🏨 Ibis Guadalajara
12. 🏟️ Estadio Guadalajara
13. 🏟️ Estadio Jalisco
14. 🏋️ Sports Arena Club
15. ⚽ Academia AGA

## 🛣️ Rutas disponibles

Cada combinación de origen-destino incluye 3 rutas preestablecidas:

- **Ruta Principal** (🔴 Roja): Ruta más directa y rápida
- **Ruta Secundaria** (🔵 Azul): Ruta alternativa
- **Ruta Terciaria** (🟢 Verde): Ruta de contingencia

### Combinaciones de rutas

- Aeropuerto GDL → Hyatt, Hilton, JW Marriott, Fiesta Americana, Westin, AC Hotel, Fiesta Inn, Ibis
- Base Aérea → Hyatt, Hilton
- Estadio Guadalajara → Hyatt, Hilton

## 🔧 Personalización

Para agregar nuevas ubicaciones o rutas, edita el archivo `index.html`:

### Agregar una nueva ubicación

Busca la sección `const UBICACIONES = {` y agrega:

```javascript
'mi_ubicacion': {
    nombre: '📍 Mi Ubicación',
    lat: 20.6597,
    lng: -103.3496
}
```

### Agregar nuevas rutas

Busca la sección `const RUTAS = {` y agrega:

```javascript
'origen|destino': {
    principal: {
        distancia: '25 km',
        tiempo: '45 min',
        descripcion: 'Descripción de la ruta...',
        url: 'https://www.google.com/maps/dir/...'
    },
    secundaria: { ... },
    terciaria: { ... }
}
```

## 📱 Compatibilidad

- ✅ Chrome/Chromium
- ✅ Firefox
- ✅ Safari
- ✅ Edge
- ✅ Navegadores móviles (iOS Safari, Chrome Mobile)

## 📦 Dependencias externas

- **Leaflet.js** (Mapas interactivos)
- **OpenStreetMap** (Tiles de mapa)

Ambas se cargan desde CDN, no requieren instalación local.

## 📄 Licencia

Uso interno para el Plan de Seguridad en Traslados FIFA 2026 Guadalajara.

## 📞 Soporte

Para reportar problemas o sugerencias, contacta al equipo de desarrollo.

---

**Última actualización:** Abril 2026
