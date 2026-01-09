# AAST_PJ – Análisis Sísmico y RSAM

Este repositorio contiene notebooks para análisis, modelación y evaluación  
de datos sísmicos y RSAM asociados al proyecto **AAST_PJ**.

Los datos no están incluidos en el repositorio.

---

## Estructura del proyecto

```

AAST_PJ/
├── notebooks/        Notebooks del proyecto
├── data/             Datos CKELAR (no incluidos)
├── processed_data/   Datos procesados (no incluidos)
├── figures/          Figuras generadas (no incluidas)
├── tables/           Tablas de resultados (no incluidas)
├── config.yaml       Configuración de rutas locales
└── environment.yml   Entorno conda reproducible

````

---

## Acceso a datos

Los datos utilizados pertenecen a **CKELAR**.  
Para acceder a ellos se requiere autorización del  
**Profesor Pablo Salazar**.

Una vez obtenidos los datos, deben almacenarse localmente  
y configurarse las rutas en el archivo `config.yaml`.

---

## Instalación del entorno (Conda)

El proyecto requiere **conda**.

Crear el entorno:
```bash
conda env create -f environment.yml
````

Activar el entorno:

```bash
conda activate AAST_PJ
```

---

## Configuración

Antes de ejecutar los notebooks:

1. Abrir `config.yaml`
2. Definir las rutas locales a:

   * Datos CKELAR
   * Directorios de salida (`processed_data`, `figures`, `tables`)

Ejemplo de `config.yaml`:

```yaml
data_root: /ruta/a/datos_ckelar
processed_data: /ruta/a/processed_data
figures: /ruta/a/figures
tables: /ruta/a/tables
```

---

## Ejecución

1. Activar el entorno conda
2. Verificar `config.yaml`
3. Ejecutar los notebooks desde la carpeta `notebooks`

```bash
jupyter notebook
```

---

## Notas

* Los datos no se descargan automáticamente
* Los resultados no se versionan
* El proyecto asume que los datos existen localmente
* Diseñado para reproducibilidad controlada

---

## Autor

Nicolás Henríquez Pedraza

