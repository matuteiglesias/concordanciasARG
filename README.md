
# concordanciasARG
Compilación de tablas de actividades productivas usadas por distintas oficinas públicas argentinas.

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

## Proyecto Colectivo

Si tu trabajo usa estadísticas económicas en Argentina, animate a usar y colaborar en el archivo `concordancias_GPSprod_SIPA_prodPBA_CIIU.csv`. Colaborando podemos facilitar y potenciar los esfuerzos individuales.
Pull request!

## Recomendaciones

Los nombres de columna corresponden con los de sus fuentes. La palabra 'label' indica una descripción, mientras que 'ID' es un numero identificatorio. Estos ID suelen ser numeros enteros. En caso de ver un decimal '.0' al cargar el dataset, conviene confirmar que se trata de enteros y desechar el punto y decimales.
    
