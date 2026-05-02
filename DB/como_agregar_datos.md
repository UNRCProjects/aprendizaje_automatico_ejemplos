# Cómo agregar datos en la carpeta `DB`

Guía breve para alumnos y para quien mantenga el repositorio.

## Objetivo

Centralizar los **conjuntos de datos** en un solo sitio (`DB/`) para que todos los ejemplos apunten a las mismas rutas y no se repitan copias del mismo archivo.

## Pasos

1. Descarga o genera el archivo de datos que pida el ejercicio.
2. Muévelo a la carpeta **`DB`** del proyecto (arrastrando en el explorador de archivos o con el terminal).
3. Comprueba en el enunciado o en el notebook **qué nombre de archivo** espera el código. Si hace falta, renombra el archivo para que coincida.
4. Al ejecutar el notebook o script, asegúrate de que el **directorio de trabajo** sea la raíz del repositorio (o ajusta la ruta en el código según te indique el docente).

## Ejemplo de ruta en Python

```python
from pathlib import Path

raiz = Path(__file__).resolve().parents[1]  # si el script está en una subcarpeta
# o, desde un notebook en la raíz:
ruta_csv = Path("DB") / "ejemplo.csv"
```

## Notas

- Si el archivo es muy grande, considera **Git LFS** o almacenamiento externo; pregunta al docente antes de subir binarios enormes al repositorio.
- Para datos sensibles, usa **solo conjuntos anonimizados o públicos** autorizados para la clase.
