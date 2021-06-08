# Estudio sobre la diabetes

Se pretende realizar varios análisis que permitan conocer mejor la diabetes. Se plantean varias cuestiones que se abordarán en detalle en la sección de análisis:

* Identificación de varios grupos de personas en base a los distintos parámetros de estudio.
* Evaluación de de la asunción de que la genealogía de la diabetes en el diagnostico de la enfermedad para comprobar si es realmente un factor relevante.
* Generación de un modelo que permita determinar la probabilidad de diagnóstico de la diabetes en base a unos parámetros de entrada.

Este proyecto ha sido realizado en el contexto de la Práctica 2 de las asignatura "Tipología y Ciclo de Vida de los Datos" en el Máster de Ciencia de datos de la UOC.

## Dependencias y requerimientos previos
El proyecto está desarrollado como un informe dinámico en formado *R Markdown* de *R studio*. Se requiere la intstalación previa de los paquetes:

* ggplot2
* gridExtra
* ggcorrplot
* ggdendro
* GGally
* VIM
* dplyr
* pROC


## Estructura de carpetas y ficheros

La estructura de carpetas y ficheros dispone de los siguientes elementos:

* **res (folder)**: contiene el juego de datos previo y posterior a su limpieza.
* **src (folder)**: contiene el informe dinámico en formato *R Markdown* ("insulinStudy.Rmd") y la bibliografía del mismo ("bibliografia.bib").
* **README.md**: fichero README con documentación básica.
* **LICENSE (file)**: fichero que contiene la licencia de la solución.
* **Practica2.pdf (file)**: Informe del caso de estudio.

## Dataset

El presente estudio emplea el juego de datos *Diabetes Data Set*, disponible en *https://www.kaggle.com/mathchi/diabetes-data-set*. Se trata de un dataset de una fuente altamente contrastada (*National Institute of Diabetes and Digestive and Kidney Diseases*) y se ofrece información detallada sobre múltiples variables recogidas de las personas de estudio (número de embarazos, presión sanguínea distólica, doblez de piel, nivel de insulina, índice de masa corporal, valor de genealogía de diabetes, edad, diabetes diagnosticada). El conjunto de datos está centrado en un grupo de personas que comparten características comunes: mujeres nativas americanas Pima de al menos 21 años de edad.

En el directorio *res/* se incorpora la versión original de los datos ("diabetes.csv"), así como la versión preprocesada ("diabetes.csv"). El preprocesado de los datos ha consistido en:

1. Búsqueda de datos faltantes.
2. Detección de outliers.
3. Imputación de datos faltantes. 
4. Estudio de reducción de la dimensionalidad.

La estructura de ambos ficheros es similar:
* Formato CSV
* Separador de campos: coma (,)
* Contiene 768 observaciones de 9 variables

## Documentación detallada

El documento "Practica2.pdf" ofrece documentación detallada sobre la solución: contexto, descripción del conjunto de datos, representación gráfica, contenido, casos de estudio y agradecimientos.

## Autores 
[Autores del proyecto](https://github.com/pablo-rvs/insulinStudy/wiki/Autores)
