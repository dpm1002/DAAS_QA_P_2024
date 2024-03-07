En el proceso de medición la   actividad de identificar entidades del sistema con medidas anómalas requiere de intervalos de valores recomendables también llamados valores umbrales. A partir de ellos, se puede identificar las entidades anómalas comprobando si los valores de sus medidas están dentro de esos intervalos.
La práctica consiste en realizar un experimento empírico, cuyo resultado será un intervalo de valores recomendables para cada una de las métricas de código calculadas por las herramientas recomendadas y que se exponen en clase de teoría.

La práctica consiste en realizar un experimento empírico, cuyo resultado será un intervalo de valores recomendables para cada una de las métricas propuestas en la Tabla 1 del enunciado.

1. Conocer una herramienta de medición de código y las métricas que calcula RefactorIt  o SourceMeter
2. Seleccionar un conjunto de proyectos del  repositorio   GitHub, SourceForge,   o GitLab , preferiblemente dentro del mismo área temática y desarrollados en el Java. Número mínimo cuatro. Utilizad algún criterio de selección de proyectos relacionado con datos medidas externas:  número de instalaciones, estado de  desarrollo estable o maduro, tipo de licencia  …
3. Cargar e instalar los códigos fuentes de las aplicaciones seleccionadas obteniendo los datos a través de los repositorios de control de versiones.
4. Crear un perfil de métricas con la herramienta de medición preferiblemente seleccionando alguna de las métricas vistas en teoría.
5. Para cada proyecto seleccionado, realizar la medición de sus entidades(paquetes, clases y métodos) y exportar los datos en formato csv (comma separated value).
6. Importar los datos en formato csv a una hoja de cálculo y obtener los intervalos recomendados a través de un análisis estadístico descriptivo de los valores de las métricas. 