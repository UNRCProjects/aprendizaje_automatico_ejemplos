# Carpeta `DB` — datos para los ejemplos

Aquí van los **archivos de datos** (CSV, SQLite, etc.) que usan los notebooks o scripts de las demás carpetas, para no duplicar archivos pesados en cada práctica.

## Cómo agregar la base de datos

1. **Coloca el archivo** de datos dentro de esta carpeta `DB/` (o en un subdirectorio, por ejemplo `DB/datasets/nombre_del_conjunto/`).
2. **Usa un nombre claro**: sin espacios raros si puedes evitarlo (por ejemplo `ventas_2024.csv` en lugar de `copia de datos final v2.csv`).
3. **No subas datos personales o confidenciales** sin permiso; si la práctica usa datos sintéticos o públicos, indícalo en un comentario o en el README del tema.
4. **En tu código**, referencia la ruta relativa al notebook o script, por ejemplo:
   - Desde la raíz del repo: `DB/mi_archivo.csv`
   - O con `pathlib` / `os.path` para que funcione en distintos sistemas.

Para más detalle paso a paso, abre también **`como_agregar_datos.md`** en esta misma carpeta.

## Contenido esperado

- Archivos de datos (`.csv`, `.parquet`, `.db`, etc.).
- Opcionalmente subcarpetas por tema o por fuente.

Si una práctica concreta espera un nombre de archivo fijo, el `README` de esa carpeta lo indicará.
