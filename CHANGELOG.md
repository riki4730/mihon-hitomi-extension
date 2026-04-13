# Changelog - Extensión Hitomi.la para Mihon

## Versión 2.0.0 (2026-04-13)

### ✨ Nuevas Características

#### Filtros Avanzados
- **Filtro por Tags**: Busca contenido por tags específicos (ej: `schoolgirl`, `romance`)
- **Filtro por Artista**: Encuentra trabajos de artistas específicos
- **Filtro por Grupo**: Filtra por grupos de traducción o creación
- **Filtro por Series**: Busca contenido de series específicas
- **Filtro por Personajes**: Encuentra galerías con personajes específicos

#### Filtros de Categoría
- **Tipo de contenido**: 
  - All (Todos)
  - Doujinshi
  - Manga
  - Artist CG
  - Game CG
  - Anime

#### Filtros de Idioma
Soporte para 10 idiomas principales:
- English
- Japanese
- Spanish
- French
- Korean
- German
- Chinese
- Portuguese
- Italian
- Russian

#### Ordenamiento Mejorado
- Newest (Más recientes)
- Popular Today (Popular hoy)
- Popular Week (Popular esta semana)
- Popular Month (Popular este mes)

### 🚀 Optimización de Rendimiento

#### Optimización de Miniaturas
Nueva configuración de calidad de miniaturas con 3 niveles:
- **Alta**: Imágenes de mayor calidad (más datos)
- **Media**: Balance entre calidad y consumo (predeterminado)
- **Baja**: Ahorro máximo de datos móviles

**Cómo configurar:**
1. Mihon → Extensiones
2. Hitomi.la → Configuración (⚙️)
3. Selecciona "Calidad de miniaturas"

**Ahorro estimado:**
- Baja: ~60% menos datos vs Alta
- Media: ~30% menos datos vs Alta

### 🔧 Mejoras Técnicas

- URLs de imágenes mejoradas con cálculo de subdominios más sofisticado
- Mejor parseo de metadata (tipo, idioma, series, personajes)
- Descripción enriquecida con más información
- Selectores CSS más robustos para cambios del sitio
- Soporte mejorado para lazy loading de imágenes

### 📝 Cómo Usar los Filtros

#### Ejemplo 1: Buscar por artista
```
1. Ir a Hitomi.la en Mihon
2. Tocar el ícono de filtro
3. En "Artista" escribir el nombre
4. Aplicar filtro
```

#### Ejemplo 2: Buscar manga en español
```
1. Abrir filtros
2. En "Tipo" seleccionar "Manga"
3. En "Idiomas" marcar "Spanish"
4. Aplicar
```

#### Ejemplo 3: Combinar múltiples filtros
```
1. Tag: schoolgirl
2. Tipo: Doujinshi
3. Idioma: English
4. Ordenar: Popular Week
```

---

## Versión 1.0.0 (2026-04-12)

### 🎉 Lanzamiento Inicial

- Búsqueda básica de galerías
- Listado de contenido popular
- Listado de últimas actualizaciones
- Visualización de detalles (artista, tags)
- Lectura de capítulos
- Soporte de imágenes WebP
- Marcado como NSFW
- Soporte multi-idioma (lang: "all")
