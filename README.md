
# DatosConcordadosARG 
*(Harmonized Economic Classifications of Argentina)*
Clasificaciones armonizadas de actividades productivas en Argentina: CIIU, CLAE, SIPA, y más.

## Descripción

Este repositorio ofrece un conjunto de tablas de correspondencia entre las principales clasificaciones económicas utilizadas en Argentina, incluyendo:
- **CLAE 3 (Ministerio de Producción)**
- **CIIU Internacional**
- **CLANAE (Dirección Provincial de Estadística)**

Estas tablas son ideales para investigadores y desarrolladores que trabajan con datos estadísticos y económicos de Argentina, facilitando el análisis cruzado y la interoperabilidad entre diversas fuentes de datos.

## Características Principales

- **Armonización Completa:** Integra múltiples clasificaciones económicas en un único dataset.
- **Formato CSV Estandarizado:** Facilita el uso en herramientas como Python, R, Excel, y bases de datos SQL.
- **Aplicaciones Académicas y Profesionales:** Pensado para estudios de economía, políticas públicas, y análisis sectorial.

## Contenido del Repositorio

- `concordancias_GPSprod_SIPA_prodPBA_CIIU.csv`: Tabla principal con correspondencias entre clasificaciones económicas.
- `material_util/`: Material complementario para entender la estructura y el propósito del dataset.
- `README.md`: Este archivo con información detallada sobre cómo usar el repositorio.



Archivo principal:
`concordancias_GPSprod_SIPA_prodPBA_CIIU.csv`

## Columnas

Este archivo sirve para unificar las estadísticas productivas de las siguientes fuentes, donde tenemos dos grupos principales:

*** Similares a CIIU ***
* [Secretaria de Transformación Productiva](https://www.produccion.gob.ar/area/secretaria-de-la-transformacion-productiva). Ministerio de la Producción.
    * CLAE 3
    * Descripción CLAE 3
* CIIU (uso internacional)
    * CIIU ID CI4
    * CIIU label CI4
    * CIIU ID CI2
    * CIIU ID CI1
    * CIIU ID CI0

*** Similares entre sí***
* La columna más importante:
    * CLAE ID 2
* [Boletín de empleo registrado](www.trabajo.gob.ar/downloads/estadisticas/oede/nacional_serie_empleo_anual.xlsx). Ministerio de Trabajo.
    * Ramas
    * Descripción 
*  [Producto Bruto Geográfico](http://www.estadistica.ec.gba.gov.ar/dpe/). Direccion Provincial de Estadística, Prov. Buenos Aires
    * Letra 
    * CLANAE 
    * sector 
    * dpe
    * dígitos 
    * sector.1


### Instrucciones

1. Clona el repositorio:
   ```bash
   git clone https://github.com/matuteiglesias/DatosConcordadosARG.git
   cd DatosConcordadosARG
   ```

2. Importa el archivo CSV en tu herramienta preferida:
   - **Python**:
     ```python
     import pandas as pd
     data = pd.read_csv("concordancias_GPSprod_SIPA_prodPBA_CIIU.csv")
     ```
   - **R**:
     ```R
     data <- read.csv("concordancias_GPSprod_SIPA_prodPBA_CIIU.csv")
     ```

3. Consulta la documentación adicional en el directorio `material_util/`.

## Aplicaciones del Dataset

Este dataset es útil para:
- **Investigadores académicos:** Realizar análisis de políticas públicas, comercio exterior, y productividad sectorial.
- **Economistas:** Comparar datos productivos entre diferentes regiones y clasificaciones.
- **Desarrolladores:** Crear aplicaciones que necesiten integrar estadísticas económicas de múltiples fuentes.

## Cita Académica

Si usas este dataset en una publicación, por favor cita de la siguiente manera:

```plaintext
Iglesias, M. (2019). DatosConcordadosARG: Clasificaciones Económicas Armonizadas de Argentina. Repositorio en GitHub. Disponible en: https://github.com/matuteiglesias/DatosConcordadosARG
```

## Recomendaciones

Los nombres de columna corresponden con los de sus fuentes. La palabra 'label' indica una descripción, mientras que 'ID' es un numero identificatorio. Estos ID suelen ser numeros enteros. En caso de ver un decimal '.0' al cargar el dataset, conviene confirmar que se trata de enteros y desechar el punto y decimales.
    
