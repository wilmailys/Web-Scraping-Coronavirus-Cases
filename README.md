# Web-Scraping-Coronavirus-Cases

Se seleccionó una página web con detalle de los casos de coronavirus para 223 países, donde se refleja: total de casos, casos nuevos, muertes totales, pacientes recuperados, los recuperados recientemente, los casos activos, los que se encuentran en una situación crítica y la población de cada uno de los países. 
Url: https://www.worldometers.info/coronavirus/#main_table


Proceso de extracción de datos:

-Cargar la página web que contiene los datos.
-Localizar los datos dentro de la página y extraerlos.
-Organizar los datos en un marco de datos
-Exportar los datos a un archivo csv

Detalle del proceso:
-Se usó como herramienta de trabajo Jupyter Notebook.
-Se importaron los módulos necesarios destacando BeautifulSoup  y Pandas.
-A través del módulo requests determinamos si la solicitud de la página es exitosa es decir si se puede proceder a la extracción de datos. 
-Se extrajo el  HTML
-Se analizó el HTML
-Se usó SELECT para definir los elementos requeridos. 
-Se creó una variable para cada uno de los ítems.
-Se usó nth-child para seleccionar cada grupo de hermanos y con ayuda de un for que me permitiera iterar por cada una de las filas basada en su estructura principal. 
-Se determinó la longitud para cada una de las columnas con el propósito de ser almacenados posteriormente en un marco de  datos. 
-Se define la forma de la tabla para determinar la cantidad de datos aproximada extraída. 
Por último se guarda la información en un archivo CSV para una mejor visualización.

Dificultades: 
-Desechar la información que no es necesaria. 
-Seleccionar cada grupo de hermanos en esta oportunidad necesitaba  el segundo hijo en la estructura jerárquica que se pudo resolver con la clase nth-child().

    
