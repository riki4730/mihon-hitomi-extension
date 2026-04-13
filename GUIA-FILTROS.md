# 🎯 Guía Completa de Filtros - Hitomi.la Extension v2.0

## 📋 Índice
1. [Acceso a Filtros](#acceso-a-filtros)
2. [Filtros Disponibles](#filtros-disponibles)
3. [Ejemplos Prácticos](#ejemplos-prácticos)
4. [Sintaxis de Búsqueda](#sintaxis-de-búsqueda)
5. [Trucos y Tips](#trucos-y-tips)

---

## Acceso a Filtros

### En Mihon

1. Abre **Mihon**
2. Ve a **Navegar** (pestaña inferior)
3. Selecciona **Hitomi.la**
4. Toca el ícono de **🔍 Filtro** (arriba a la derecha)

---

## Filtros Disponibles

### 🏷️ Filtro de Tag
**Qué es**: Etiquetas que describen el contenido (género, temática, etc.)

**Cómo usar**:
- Toca el campo "Tag"
- Escribe el tag (en inglés, minúsculas)
- Ejemplos: `schoolgirl`, `romance`, `fantasy`

**Tags populares**:
```
schoolgirl, teacher, glasses, swimsuit, 
stockings, uniform, cosplay, maid, nurse,
fantasy, romance, comedy, drama
```

---

### 🎨 Filtro de Artista
**Qué es**: Encuentra trabajos de un artista específico

**Cómo usar**:
- Campo "Artista"
- Escribe el nombre (usar guiones en lugar de espacios)
- Ejemplo: `artist-name` o `artist_name`

**Tip**: Si no sabes el nombre exacto:
1. Busca una galería del artista
2. Mira el nombre en los detalles
3. Copia el formato exacto

---

### 👥 Filtro de Grupo
**Qué es**: Grupos de traducción o equipos de creación

**Cómo usar**:
- Campo "Grupo"
- Formato: `group-name`

---

### 📺 Filtro de Series
**Qué es**: Contenido basado en series/anime/manga específicos

**Cómo usar**:
- Campo "Series"
- Ejemplos: `naruto`, `one-piece`, `pokemon`

**Series populares**:
```
touhou, fate, kantai-collection, azur-lane,
girls-frontline, granblue-fantasy, pokemon,
fire-emblem, idolmaster, love-live
```

---

### 👤 Filtro de Personajes
**Qué es**: Busca por personajes específicos

**Cómo usar**:
- Campo "Personaje"
- Formato: `character-name`

---

### 📁 Filtro de Tipo
**Qué es**: Categoría del contenido

**Opciones**:
- **All**: Todo el contenido
- **Doujinshi**: Obras derivadas amateur
- **Manga**: Manga original
- **Artist CG**: Arte digital de artistas
- **Game CG**: CG de videojuegos
- **Anime**: Capturas/arte de anime

**Cómo usar**:
1. Toca "Tipo"
2. Selecciona una opción
3. Solo puedes elegir una a la vez

---

### 🌍 Filtros de Idioma
**Qué es**: Filtra por idioma del contenido

**Idiomas disponibles**:
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

**Cómo usar**:
1. Expande "Idiomas"
2. Marca uno o varios ✓
3. Puedes combinar múltiples idiomas

**Ejemplo**: Buscar en inglés Y español
```
✓ English
✓ Spanish
```

---

### 📊 Ordenamiento
**Qué es**: Ordena los resultados

**Opciones**:
- **Newest**: Más recientes (predeterminado)
- **Popular Today**: Lo más popular hoy
- **Popular Week**: Popular esta semana
- **Popular Month**: Popular este mes

**Tip**: Usa "Popular Week" para encontrar contenido de calidad

---

## Ejemplos Prácticos

### Ejemplo 1: Manga en español
```
Configuración:
├─ Tipo: Manga
└─ Idiomas: ✓ Spanish

Resultado: Solo mangas en español
```

### Ejemplo 2: Contenido popular de una serie
```
Configuración:
├─ Series: touhou
├─ Ordenar: Popular Month
└─ Idiomas: ✓ English

Resultado: Touhou más popular del mes en inglés
```

### Ejemplo 3: Artista específico, solo doujinshi
```
Configuración:
├─ Artista: nombre-artista
└─ Tipo: Doujinshi

Resultado: Solo doujinshi de ese artista
```

### Ejemplo 4: Tag + Idioma + Ordenamiento
```
Configuración:
├─ Tag: schoolgirl
├─ Tipo: Doujinshi
├─ Idiomas: ✓ English, ✓ Japanese
└─ Ordenar: Popular Week

Resultado: Doujinshi de schoolgirl populares 
           esta semana en inglés o japonés
```

### Ejemplo 5: Búsqueda por personaje de serie
```
Configuración:
├─ Series: fate
├─ Personaje: saber
└─ Ordenar: Popular Today

Resultado: Contenido de Saber (Fate) 
           popular hoy
```

---

## Sintaxis de Búsqueda

También puedes escribir directamente en la barra de búsqueda:

### Formato General
```
[término] tipo:[categoría] tag:[tag] artist:[artista] language:[idioma]
```

### Ejemplos de Sintaxis

**Buscar por tag y artista**:
```
tag:schoolgirl artist:artist-name
```

**Buscar manga en español**:
```
type:manga language:spanish
```

**Combinar múltiples filtros**:
```
tag:romance series:touhou type:doujinshi language:english
```

**Buscar por personaje y grupo**:
```
character:character-name group:group-name
```

### Reglas de Sintaxis

1. **Minúsculas**: Todo en minúsculas
   - ✅ `language:spanish`
   - ❌ `language:Spanish`

2. **Guiones**: Usa guiones para espacios
   - ✅ `artist:artist-name`
   - ❌ `artist:artist name`

3. **Sin espacios extras**: Pega el prefijo al valor
   - ✅ `tag:schoolgirl`
   - ❌ `tag: schoolgirl`

4. **Separar con espacios**: Entre diferentes filtros
   - ✅ `tag:romance language:english`
   - ❌ `tag:romancelanguage:english`

---

## Trucos y Tips

### 🎯 Tip 1: Búsquedas Incrementales
Empieza con filtros amplios y ve especificando:

```
Paso 1: type:doujinshi
Paso 2: + language:spanish
Paso 3: + tag:romance
Paso 4: + sort:popular-week
```

### 🎯 Tip 2: Descubrir Tags
1. Abre cualquier galería
2. Mira la sección de "Tags"
3. Toca un tag que te interese
4. Mihon buscará automáticamente con ese tag

### 🎯 Tip 3: Guardar Búsquedas Frecuentes
Anota tus combinaciones favoritas:

```
Favorito 1: tag:schoolgirl type:doujinshi language:english
Favorito 2: series:touhou sort:popular-month
Favorito 3: artist:favorite-artist sort:newest
```

### 🎯 Tip 4: Encontrar Artistas
Si te gusta una galería:
1. Abre los detalles
2. Mira el artista
3. Toca en el nombre del artista
4. O filtra manualmente por ese artista

### 🎯 Tip 5: Explorar Series Populares
```
Paso 1: No uses filtros, solo navega "Popular Month"
Paso 2: Mira qué series aparecen más
Paso 3: Filtra por la serie que te interese
```

### 🎯 Tip 6: Ahorro de Datos + Búsqueda
Para ahorrar datos al explorar:
1. Configura miniaturas en "Baja"
2. Usa filtros específicos para reducir resultados
3. Ordena por "Popular" para ver lo mejor primero

### 🎯 Tip 7: Búsqueda Multiidioma
Si hablas varios idiomas:
```
✓ English
✓ Spanish
✓ Portuguese

Resultado: 3x más contenido disponible
```

---

## 🚨 Problemas Comunes

### "No se encontraron resultados"

**Posibles causas**:
1. Filtros demasiado específicos
2. Sintaxis incorrecta
3. Tag/artista no existe

**Solución**:
- Reduce filtros (quita uno por uno)
- Verifica ortografía
- Usa solo el filtro principal primero

### "Los filtros no se aplican"

**Solución**:
1. Asegúrate de tocar "Aplicar" o "Buscar"
2. Cierra y vuelve a abrir la extensión
3. Actualiza la lista de extensiones

### "Aparece contenido no relacionado"

**Posible causa**: Búsqueda por texto + filtros

**Solución**:
- Si usas la barra de búsqueda, déjala vacía
- Solo usa los filtros
- O usa sintaxis completa

---

## 📊 Tabla de Referencia Rápida

| Quiero | Filtros a Usar |
|--------|----------------|
| Manga en mi idioma | Tipo: Manga, Idioma: [tu idioma] |
| Lo más popular ahora | Ordenar: Popular Today |
| Contenido de un anime | Series: [nombre-anime] |
| Artista favorito | Artista: [nombre-artista] |
| Tag específico | Tag: [nombre-tag] |
| Combinar todo | Todos los anteriores juntos |

---

## 🎓 Ejercicios Prácticos

Prueba estas búsquedas para dominar los filtros:

### Ejercicio 1: Básico
```
Objetivo: Encontrar doujinshi en inglés
Filtros: 
├─ Tipo: Doujinshi
└─ Idiomas: ✓ English
```

### Ejercicio 2: Intermedio
```
Objetivo: Manga de fantasía popular en español
Filtros:
├─ Tag: fantasy
├─ Tipo: Manga
├─ Idiomas: ✓ Spanish
└─ Ordenar: Popular Month
```

### Ejercicio 3: Avanzado
```
Objetivo: Contenido de Touhou de un artista específico
Filtros:
├─ Series: touhou
├─ Artista: [descubre uno que te guste]
├─ Tipo: Doujinshi
└─ Ordenar: Newest
```

---

¡Ahora eres un experto en filtros de Hitomi.la! 🎉

**Recuerda**: La práctica hace al maestro. Experimenta con diferentes combinaciones para encontrar exactamente lo que buscas.
