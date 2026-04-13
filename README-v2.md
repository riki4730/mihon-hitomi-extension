# Extensión Hitomi.la para Mihon - v2.0

Esta es una extensión personalizada para Mihon (fork de Tachiyomi) que permite acceder al contenido de Hitomi.la con **filtros avanzados** y **optimización de miniaturas**.

⚠️ **ADVERTENCIA**: Esta extensión está marcada como NSFW (No Safe For Work) ya que Hitomi.la contiene contenido para adultos.

## 🆕 Novedades en v2.0

### ✨ Filtros Avanzados

- **🏷️ Filtro por Tags**: Busca por tags específicos (schoolgirl, romance, etc.)
- **🎨 Filtro por Artista**: Encuentra trabajos de artistas específicos
- **👥 Filtro por Grupo**: Filtra por grupos de traducción
- **📺 Filtro por Series**: Busca contenido de series específicas
- **👤 Filtro por Personajes**: Encuentra personajes favoritos

### 📊 Filtros de Categoría

- **Tipo**: All, Doujinshi, Manga, Artist CG, Game CG, Anime
- **Idiomas**: 10 idiomas (English, Japanese, Spanish, French, Korean, German, Chinese, Portuguese, Italian, Russian)
- **Ordenamiento**: Newest, Popular Today, Popular Week, Popular Month

### 🚀 Optimización de Miniaturas

Ahorra datos móviles con 3 niveles de calidad:
- **Alta**: Máxima calidad (~100% datos)
- **Media**: Balance perfecto (~70% datos) ⭐ Predeterminado
- **Baja**: Ahorro máximo (~40% datos)

**Configuración:**
Mihon → Extensiones → Hitomi.la → ⚙️ → Calidad de miniaturas

## Características

- ✅ Búsqueda avanzada con múltiples filtros
- ✅ Listado de contenido popular y reciente
- ✅ Visualización de detalles completos
- ✅ Lectura optimizada de capítulos
- ✅ Soporte de imágenes WebP
- ✅ Marcado como NSFW
- ✅ Multi-idioma (lang: "all")
- ✅ Ahorro de datos móviles

## Instalación

### Opción 1: Instalación directa del APK

1. Descarga el archivo `hitomi-extension-v2.0.apk`
2. Instálalo en tu dispositivo Android
3. Abre Mihon y la extensión aparecerá automáticamente

### Opción 2: Añadir repositorio personalizado (RECOMENDADO)

#### Paso 1: La extensión ya está en GitHub

El repositorio está en: `https://github.com/riki4730/mihon-hitomi-extension`

Los archivos necesarios ya están configurados:
- `hitomi-extension-v2.0.apk`
- `index.min.json` (con la URL correcta)
- `README.md`
- `CHANGELOG.md`

#### Paso 2: Configurar Mihon

1. Abre **Mihon**
2. Ve a **Ajustes** (⚙️) → **Extensiones**
3. Toca en el ícono de los **tres puntos** (⋮) en la esquina superior derecha
4. Selecciona **Repositorios de extensiones**
5. Toca el botón **+** (añadir repositorio)
6. Ingresa la URL:
   ```
   https://raw.githubusercontent.com/riki4730/mihon-hitomi-extension/main/index.min.json
   ```
7. Toca **Añadir**
8. Vuelve a la pantalla de extensiones
9. Actualiza la lista (desliza hacia abajo)
10. Verás **Hitomi.la v2.0** en la lista
11. Toca **Instalar**

#### Paso 3: Activar contenido NSFW (si es necesario)

Si no ves la extensión:

1. Ve a **Ajustes** → **General**
2. Activa **Mostrar contenido NSFW**
3. Vuelve a la lista de extensiones

## 📖 Cómo Usar los Filtros

### Ejemplo 1: Buscar manga en español de un artista

1. Abre **Hitomi.la** en Mihon
2. Toca el ícono de **filtro** 🔍
3. Configura:
   - **Artista**: nombre-del-artista
   - **Tipo**: Manga
   - **Idiomas**: ✓ Spanish
4. Toca **Aplicar**

### Ejemplo 2: Buscar por tag popular del mes

1. Abre los **filtros**
2. Configura:
   - **Tag**: schoolgirl (o el que prefieras)
   - **Ordenar por**: Popular Month
3. **Aplicar**

### Ejemplo 3: Buscar contenido de una serie específica

1. Filtros:
   - **Series**: nombre-de-la-serie
   - **Idiomas**: ✓ English, ✓ Japanese
2. **Aplicar**

### Sintaxis de Búsqueda Avanzada

También puedes escribir directamente en la búsqueda:
```
tag:schoolgirl artist:nombre type:doujinshi language:spanish
```

## ⚙️ Configuración de Ahorro de Datos

### ¿Cuántos datos ahorro?

**Ejemplo con 100 galerías navegadas:**

| Calidad | Datos por miniatura | Total estimado |
|---------|---------------------|----------------|
| Alta    | ~50 KB             | ~5 MB          |
| Media   | ~35 KB             | ~3.5 MB ⭐     |
| Baja    | ~20 KB             | ~2 MB          |

**Recomendación:**
- **WiFi**: Alta
- **Datos ilimitados**: Media
- **Plan limitado**: Baja

## Estructura del código

```
hitomi-extension-v2/
├── build.gradle                    # v2.0.0
├── src/
│   └── main/
│       ├── AndroidManifest.xml    # Marcado NSFW
│       ├── java/
│       │   └── eu/kanade/tachiyomi/extension/hitomi/
│       │       └── Hitomi.kt      # 400+ líneas con filtros
│       └── res/
│           └── mipmap-*/
│               └── ic_launcher.png
```

## Nuevas Características v2.0

### Filtros Implementados

```kotlin
// Filtros de texto
- TagFilter("Tag")
- ArtistFilter("Artista")
- GroupFilter("Grupo")
- SeriesFilter("Series")
- CharacterFilter("Personaje")

// Filtros de selección
- TypeFilter("Tipo", ["All", "Doujinshi", "Manga", ...])
- LanguageFilterList("Idiomas", [10 idiomas])
- SortFilter("Ordenar por", [4 opciones])
```

### Sistema de Optimización de Miniaturas

```kotlin
private fun optimizeThumbnailUrl(url: String): String {
    when (thumbnailQuality) {
        "high" -> // Máxima resolución
        "medium" -> // Balance (default)
        "low" -> // Miniatura pequeña
    }
}
```

### Construcción Mejorada de URLs

```kotlin
private fun calculateSubdomain(galleryId: String, page: Int): String {
    // Distribución inteligente entre subdomains a, b, c
    val hash = (id + page).toString().hashCode()
    return subdomains[Math.abs(hash) % subdomains.size]
}
```

## Problemas conocidos

1. **URLs de imágenes**: Si las imágenes no cargan, Hitomi.la puede haber cambiado su sistema.

2. **Filtros muy específicos**: Combinaciones muy restrictivas pueden no devolver resultados.

3. **Rate limiting**: Hitomi.la puede limitar requests rápidos.

## Solución de problemas

### Los filtros no funcionan
- Verifica la sintaxis (minúsculas, guiones en lugar de espacios)
- Ejemplo correcto: `artist:artist-name` no `artist:Artist Name`

### Las miniaturas se ven pixeladas
- Ve a Configuración de la extensión
- Cambia "Calidad de miniaturas" a "Alta"

### Consume muchos datos
- Cambia la calidad a "Baja" en configuración
- Considera usar WiFi para navegar

### La extensión no aparece después de actualizar
1. Desinstala la versión 1.0
2. Actualiza la lista de extensiones
3. Instala la versión 2.0

## Actualización desde v1.0

1. Abre Mihon → Extensiones
2. Si usaste repositorio, verás "Actualización disponible"
3. Toca "Actualizar"
4. O descarga el nuevo APK e instala sobre la versión anterior

## Comparación v1.0 vs v2.0

| Característica | v1.0 | v2.0 |
|---------------|------|------|
| Búsqueda básica | ✅ | ✅ |
| Filtro por tags | ❌ | ✅ |
| Filtro por artista | ❌ | ✅ |
| Filtros de idioma | ❌ | ✅ |
| Ordenamiento | ❌ | ✅ |
| Optimización datos | ❌ | ✅ |
| Configuración | ❌ | ✅ |
| Metadata enriquecida | Básica | Completa |

## Roadmap Futuro (v2.1+)

- [ ] Caché de búsquedas recientes
- [ ] Historial de filtros usados
- [ ] Sugerencias de tags populares
- [ ] Modo de vista compacta
- [ ] Integración con listas de favoritos

## Contribuir

Si encuentras bugs o tienes sugerencias:
1. Reporta issues en GitHub
2. Incluye versión de Mihon y Android
3. Describe el problema detalladamente

## Disclaimer

Esta extensión se proporciona únicamente con fines educativos. El acceso a Hitomi.la está sujeto a los términos del sitio y las leyes locales. Asegúrate de cumplir con todas las regulaciones pertinentes.

## Licencia

Código de dominio público. Úsalo bajo tu propia responsabilidad.

---

**Versión**: 2.0.0  
**Última actualización**: 13 de Abril, 2026  
**Autor**: riki4730  
**Repositorio**: https://github.com/riki4730/mihon-hitomi-extension
