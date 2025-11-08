# 📘 Diccionario de Datos - Proyecto Geoespacial

Este documento describe las variables contenidas en los siguientes datasets: **Cuerpos de Agua**, **Cursos de Agua**, **Microbasurales** y **Zonas Inundables**. Incluye tipo de dato, unidad de medida y observaciones relevantes para análisis espacial y ambiental.

---

## 🟦 Dataset: `du_techo_cuerpos_de_agua.csv`

| Variable      | Tipo de Dato         | Unidad / Formato         | Descripción |
|---------------|----------------------|---------------------------|-------------|
| `WKT`         | Geométrica (MULTIPOLYGON) | Coordenadas geográficas (EPSG:4326) | Representa la forma y ubicación del cuerpo de agua |
| `id`          | Numérica (entera)    | -                         | Identificador único del polígono |
| `provincia`   | Categórica nominal   | -                         | Provincia donde se ubica el cuerpo de agua |
| `departamen`  | Categórica nominal   | -                         | Departamento administrativo |
| `localidad`   | Categórica nominal   | -                         | Localidad específica |
| `tipo`        | Categórica nominal   | -                         | Tipo de cuerpo de agua (`Espejo`, `Laguna`, `Humedal`, etc.) |

---

## 🟦 Dataset: `du_techo_cursos_de_agua.csv`

| Variable      | Tipo de Dato         | Unidad / Formato         | Descripción |
|---------------|----------------------|---------------------------|-------------|
| `WKT`         | Geométrica (MULTILINESTRING) | Coordenadas geográficas (EPSG:4326) | Representa el trazado del curso de agua |
| `id`          | Numérica (entera)    | -                         | Identificador único del curso |
| `id_linea`    | Numérica (entera)    | -                         | Identificador de línea hidrográfica |
| `provinicia`  | Categórica nominal   | -                         | Provincia (error ortográfico: debería ser `provincia`) |
| `departamen`  | Categórica nominal   | -                         | Departamento |
| `localidad`   | Categórica nominal   | -                         | Localidad |

---

## 🟦 Dataset: `du_techo_microbasurales.csv`

| Variable      | Tipo de Dato         | Unidad / Formato         | Descripción |
|---------------|----------------------|---------------------------|-------------|
| `WKT`         | Geométrica (MULTIPOINT) | Coordenadas geográficas (EPSG:4326) | Ubicación puntual del microbasural |
| `id`          | Numérica (entera)    | -                         | Identificador del punto |
| `id_punto`    | Numérica (entera)    | -                         | Identificador alternativo del punto |
| `provincia`   | Categórica nominal   | -                         | Provincia |
| `departamen`  | Categórica nominal   | -                         | Departamento |
| `localidad`   | Categórica nominal   | -                         | Localidad |

---

## 🟦 Dataset: `du_techo_zonas_inundables.csv`

| Variable      | Tipo de Dato         | Unidad / Formato         | Descripción |
|---------------|----------------------|---------------------------|-------------|
| `WKT`         | Geométrica (MULTIPOLYGON) | Coordenadas geográficas (EPSG:4326) | Área inundable delimitada |
| `id`          | Numérica (entera)    | -                         | Identificador del polígono |
| `id_poligon`  | Numérica (entera)    | -                         | Identificador alternativo del polígono |
| `se_inunda_`  | Categórica ordinal   | -                         | Indica si el barrio se inunda (`SÍ, TODO EL BARRIO`, `SÓLO EN UN SECTOR`, etc.) |
| `con_que_fr`  | Categórica ordinal   | -                         | Frecuencia de inundación (`CADA VEZ QUE LLUEVE FUERTE`, `OCASIONALMENTE`, etc.) |
| `provinicia`  | Categórica nominal   | -                         | Provincia (error ortográfico) |
| `departamen`  | Categórica nominal   | -                         | Departamento |
| `localidad`   | Categórica nominal   | -                         | Localidad |

---

## 🧭 Notas Técnicas

- **Sistema de coordenadas**: EPSG:4326 (latitud/longitud).
- **Errores ortográficos**: `provinicia` y `departamen` deberían corregirse a `provincia` y `departamento`.
- **Normalización sugerida**:
  - Unificar valores en `tipo`, `se_inunda_`, `con_que_fr` para facilitar análisis.
  - Validar duplicados en `id` vs `id_punto` o `id_poligon`.

---

Este diccionario puede ser extendido con ejemplos, valores únicos por variable, o enlaces a visualizaciones. Ideal para documentación técnica, informes académicos o proyectos colaborativos.

