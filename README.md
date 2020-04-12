# Tipología y ciclo de vida de los datos: Práctica 1

## Descripción

El objetivo de esta práctica es la aplicación de distintas técnicas de extracción de datos para la generación de un _dataset_ que será utilizado más adelante con fines analíticos. 
El conjunto de datos generado contiene los precios mensuales de varias materias primas obtenidas de mercados mayoristas y fabricantes, así como precios agregados e índices de precios (generales y agrícolas) con periodicidad igual o menor (trimestral y anual). Algunas de las variables incluyen el mes y año, el nombre del producto y su precio en euros. El rango temporal se sitúa entre los años 2017 y 2019, ambos incluidos, aunque no se dispone de todos los datos en esos tres años.


## Miembros del equipo

La práctica ha sido realizada por **Jesús González Leal** y **Francisco Enrique Lorente Banegas**.

## Ficheros del código fuente

* **src/Scraping_All.py**: punto de entrada. Llama a los distintos métodos de extracción de datos (_web scraping_, API) para los orígenes elegidos y los une en el dataset final _Eurostat_Infaoliva_MercadosCentrales_20170101_20191231.csv_.
* **src/Scraping_MercaAlicante.py**: contiene la implementación de los métodos que extraen datos de la web de Mercalicante y generan el dataset correspondiente.
* **src/Scraping_MercaMadrid.py**: contiene la implementación de los métodos que extraen datos de la web de Mercamadrid y generan el dataset correspondiente.
* **src/genera_dataset_eurostat_infaoliva.py**: llama a los métodos implementados en **scraper_aceite.py** y **api_eurostat.py** y une los resultados en un único dataset.
* **src/scraper_aceite.py**: contiene la implementación de los métodos que extraen datos de la web de Infaoliva y generan el dataset correspondiente.
* **src/api_eurostat.py**: contiene la implementación de los métodos que extraen datos de las estadísticas seleccionadas de Eurostat y generan el dataset correspondiente.
* **src/tools.py**: contiene la implementación de distintos métodos útiles para el conjunto del código.

## Recursos
1. Subirats, L., Calvo, M. (2018). _Web Scraping_. Editorial UOC.
1. Lawson, R. (2015). _Web Scraping with Python_. Packt Publishing Ltd. Chapter 2. Scraping the Data.
