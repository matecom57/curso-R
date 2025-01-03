C01-Manas
=========

1 What Is Data Science?
-----------------------

Vivimos en la era de los datos. En la actualidad, los datos están a nuestro alrededor y se recopilan a niveles sin precedentes. Los datos pueden presentarse en forma de datos de red o de grafos: una gran cantidad de información en una red social con mil millones de usuarios, páginas web indexadas por un motor de búsqueda, transacciones de compras de una empresa de comercio electrónico o una gran red de sensores inalámbricos. La cantidad de datos que generamos es enorme: en 2012, todos los días creamos 2,5 quintillones de bytes o 2,5 millones de terabytes de datos. La tasa de crecimiento es aún más asombrosa: el 90% de los datos del mundo se generaron en los últimos dos años [1].


Los datos no son muy útiles por sí solos a menos que se conviertan en conocimiento. Este conocimiento se presenta en forma de insights, que pueden brindar mucha información sobre el proceso subyacente. Las corporaciones se orientan cada vez más a los datos: utilizan insights de los datos para impulsar sus decisiones comerciales. Una nueva clase de aplicaciones es el producto de datos [2], que va un paso más allá al convertir el insight de los datos en un producto de consumo utilizable.


Algunos de los ejemplos destacados de productos de datos incluyen:



Tendencias de gripe en Google: al analizar los registros de consultas del motor de búsqueda, Google puede rastrear la prevalencia de la gripe más rápido que los Centros para el Control y la Prevención de Enfermedades (CDC).



Motor de recomendaciones de Netflix: al observar las calificaciones de películas y los patrones de visualización de pares de usuarios, el motor de recomendaciones de Netflix puede predecir con precisión las calificaciones de las películas que un usuario no ha visto antes.



La metodología de extracción de información a partir de datos se denomina ciencia de datos. Históricamente, la ciencia de datos se ha conocido con diferentes nombres: en sus inicios, se la conocía simplemente como estadística, y luego se la conoció como análisis de datos. Existe una diferencia importante entre la ciencia de datos y la estadística y el análisis de datos. La ciencia de datos es una disciplina multidisciplinaria: es una combinación de análisis estadístico, programación y experiencia en el dominio [3]. Cada uno de estos aspectos es importante:

Statistical skills are essential in applying the right kind of statistical methodology along with interpreting the results.

Las habilidades estadísticas son esenciales para aplicar el tipo correcto de metodología estadística e interpretar los resultados.


Programming skills are essential to implement the analysis methodology, combine data from multiple sources and especially, working with large-scale datasets.

Las habilidades de programación son esenciales para implementar la metodología de análisis, combinar datos de múltiples fuentes y, especialmente, trabajar con conjuntos de datos a gran escala.

Domain expertise is essential in identifying the problems that need to be solved, forming hypotheses about the solutions, and most importantly understanding how the insights of the analysis should be applied.

El conocimiento del dominio es esencial para identificar los problemas que necesitan resolverse, formular hipótesis sobre las soluciones y, lo más importante, comprender cómo deben aplicarse los conocimientos del análisis.



En los últimos años, la ciencia de datos ha surgido como una disciplina por derecho propio.



Sin embargo, no existe un conjunto estandarizado de herramientas que se utilicen en el análisis. Los científicos de datos utilizan una variedad de lenguajes y herramientas de programación en su trabajo, a veces incluso utilizan una combinación de herramientas heterogéneas para realizar un único análisis. Esto aumenta la curva de aprendizaje para los nuevos científicos de datos. El entorno de programación R presenta un gran conjunto homogéneo de herramientas para la mayoría de las tareas de ciencia de datos.


1.2 Why R?
----------


El entorno de programación R se está convirtiendo cada vez más en una solución integral para la ciencia de datos. R se creó por primera vez en 1993 y ha evolucionado hasta convertirse en un producto estable. Se está convirtiendo en el estándar de facto para el análisis de datos en el ámbito académico y la industria.



La primera ventaja de utilizar R es que se trata de un software de código abierto. Tiene muchas ventajas respecto de otras plataformas estadísticas comerciales como MATLAB, SAS y SPSS. Además, R funciona en la mayoría de las plataformas: GNU/Linux, OS X, Windows.



R tiene sus raíces en la comunidad estadística, ya que fue creado por estadísticos para estadísticos. Esto se refleja en el diseño del lenguaje de programación: muchos de sus elementos básicos están orientados al análisis estadístico. La segunda ventaja de usar R es que la cantidad de código que necesitamos escribir en R es muy pequeña en comparación con otros lenguajes de programación. Hay muchos tipos de datos y funciones de alto nivel disponibles en R que ocultan los detalles de implementación de bajo nivel al programador. Aunque existen sistemas R que se utilizan en producción con una complejidad significativa, para la mayoría de las tareas de análisis de datos, necesitamos escribir solo unas pocas líneas de código.



R se puede utilizar como un entorno interactivo o no interactivo. Podemos utilizar R como una consola interactiva, donde podemos probar sentencias individuales y observar el resultado directamente. Esto resulta útil para explorar los datos, donde el resultado de la primera sentencia puede indicar qué paso dar a continuación. Sin embargo, R también se puede utilizar para ejecutar un script que contenga un conjunto de sentencias en un entorno no interactivo.



El beneficio final de usar R es el conjunto de paquetes de R. La razón más importante de la creciente popularidad de R es su vasta biblioteca de paquetes llamada Red Integral de Archivos de R, o más comúnmente conocida como CRAN.1 La mayoría de los métodos de análisis estadístico suelen tener una implementación de código abierto en forma de un paquete de R. R cuenta con el respaldo de una comunidad vibrante y un ecosistema creciente de desarrolladores de paquetes.


1.3 Goal of This Book
---------------------


Sin embargo, debido a su enfoque estadístico, R es una de las herramientas más difíciles de dominar, especialmente para programadores sin conocimientos previos de estadística. En comparación con otros lenguajes de programación, hay relativamente pocos recursos para aprender R. Todos los paquetes de R cuentan con documentación, pero normalmente está estructurada como material de referencia. La mayor parte de la documentación presupone un buen conocimiento de los fundamentos de la estadística.



El objetivo de este libro es presentar a los lectores algunas de las técnicas útiles de la ciencia de datos y su implementación con el lenguaje de programación R. En términos del contenido, el libro intenta lograr un equilibrio entre el cómo: procesos y metodologías específicos, y también habla del por qué: repasa la intuición detrás de cómo funciona una técnica particular, para que el lector pueda aplicarla al problema en cuestión.



El libro no presupone que el lector esté familiarizado con las estadísticas. Repasaremos los conceptos de estadística necesarios a medida que sean necesarios. El libro presupone que el lector está familiarizado con la programación: es competente en al menos un lenguaje de programación. En el Apéndice proporcionamos una descripción general del lenguaje de programación R y el entorno de desarrollo.



Este libro no pretende sustituir a un libro de texto de estadística. No entraremos en detalles teóricos profundos de los métodos, incluidas las fórmulas matemáticas. El enfoque del libro es práctico; con el objetivo de cubrir cómo implementar estas técnicas en R. Para obtener una comprensión más profunda de las metodologías subyacentes, remitimos al lector a libros de texto sobre estadística [4].



El alcance de este libro no es enciclopédico: existen cientos de metodologías de ciencia de datos que se utilizan en la práctica. En este libro solo cubrimos algunas de las más importantes que ayudarán al lector a iniciarse en la ciencia de datos. Todas las metodologías que cubrimos en este libro también son temas bastante detallados por sí mismos: cada uno merece un volumen separado. Nuestro objetivo es cubrir los fundamentos y algunas de las técnicas más útiles con el objetivo de proporcionar al usuario una buena comprensión de la metodología y los pasos para implementarla en R. La mejor manera de aprender el análisis de datos es probándolo en un conjunto de datos e interpretando los resultados. En cada capítulo de este libro, aplicamos un conjunto de metodologías a un conjunto de datos del mundo real.



La ciencia de datos se está volviendo omnipresente: está encontrando aplicaciones en todas las áreas del dominio. En este libro, no nos centramos en un solo dominio, como la econometría, la genética o los datos web. Nuestro objetivo es proporcionar herramientas para analizar cualquier tipo de datos. Cuando se trata de cuestiones específicas de un dominio en particular, remitimos al lector a otros libros sobre análisis de datos disponibles en la serie UseR!.


1.4 Book Overview
-----------------

In Chapter 2, we provide an overview of the R programming language. The readers who are already familiar with R can skim through it.

En el Capítulo 2, ofrecemos una descripción general del lenguaje de programación R. Los lectores que ya están familiarizados con R pueden hojearlo.


The remainder of the book is divided into individual chapters each covering a data science methodology. In Chap. 3, we start with getting the data into R and look at some of the data preprocessing tasks. In Chap. 4, we look at data visualization techniques. Next, in Chap. 5, we look at exploratory data analysis which can tell us about how the data is distributed. Chapters 6—Regression and 7—Classification, form the core of the book. In Chap. 6, we look at creating statistical models to predict numerical variables, while in Chap. 7, we look at analogous statistical models to predict categorical or class variables. In Chap. 8, we look at analyzing unstructured text data.

El resto del libro está dividido en capítulos individuales, cada uno de los cuales cubre una metodología de ciencia de datos. En el capítulo 3, comenzamos con la introducción de los datos en R y observamos algunas de las tareas de preprocesamiento de datos. En el capítulo 4, analizamos las técnicas de visualización de datos. A continuación, en el capítulo 5, analizamos el análisis exploratorio de datos que puede indicarnos cómo se distribuyen los datos. Los capítulos 6 (Regresión) y 7 (Clasificación) forman el núcleo del libro. En el capítulo 6, analizamos la creación de modelos estadísticos para predecir variables numéricas, mientras que en el capítulo 7, analizamos modelos estadísticos análogos para predecir variables categóricas o de clase. En el capítulo 8, analizamos el análisis de datos de texto no estructurados.


References

Big data, for better or worse: 90% of world’s data generated over last two years. www.sciencedaily.com/releases/2013/05/130522085217.htm, May 2013.
Patil, D. J. (2012). Data Jujitsu: The art of turning data into product. O’Reilly Radar.
Drew Conway. The data science venn diagram. http://drewconway.com/zia/2013/3/26/the-data-science-venn-diagram.
Casella, G., & Berger, R. (2001). Statistical inference. Duxbury Resource Center



