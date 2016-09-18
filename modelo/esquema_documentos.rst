.. _parte_del_documento:

******
PARTE
******

ESQUEMA GLOBAL DE DOCUMENTO

El documento estará estructurado con la siguiente jerarquía de niveles:

* Parte (agrupa Capítulos)
* Capítulo (agrupa Secciones)
* Sección (Separa porciones de texto normal)

Se utilizará en un archivo ``hijo`` del documento principal (normalmente index.rst) para identifcar las partes del documento. Es considerado la división más grande.
En ella se insertarán los Capítulos y las Secciones. Todas las letras se escriben con mayúsculas.

Cuando se utiliza en un archivo que es ``hijo`` del principal, es decir, que forma parte de la ``toctree`` de otro, se convierte en Capítulo de esa Parte.

Ej::

	En el archivo ``provincias.rst`` que está referenciado o indexado
	en el masterdoc (index.rst), se tiene la siguiente toctree:

		toctree::
			maxdepth: 2
			numbered:

			cercado.rst
			marban.rst


	Entonces, si en los archivos cercado.rst y marban.rst se utiliza el
	asterísco encima y debajo, el contenido de cada archivo se convierten
	en Capítulos consecutivos de la	parte y su cotenido, representada por
	el archivo provincias.rst.

.. _capitulo_del_documento:

CAPÍTULO
*********

ES LA DIVISIÓN PARA EXPLICAR COSAS INDEPENDIENTES PERO RELACIONADAS ENTRE SÍ Y CON EL TEMA DE LA :ref:`parte_del_documento`

Siguiendo el ejemplo anterior, cada Capítulo lo formarían cada una de las provincias, escritas o desarrolladas en archivos independientes. Todas las letras se escriben con mayúsculas.

.. _seccion_del_documento:

Sección
========

*Inicio de texto normal como puntos a tratar*

Se puede escribir con mayúscula inicial y el resto en minúsculas o como la función en LibreOffice Calc ``nompropio()``, es decir todas las letras iniciales en mayúsculas.

.. _sub_seccion_del_documento:

Sub Sección
------------

División primaria de cada sección para dar mayor claridad al texto normal.

.. _sub_sub_seccion_del_documento:

Sub Sub Sección
................


Ir a :ref:`parte_del_documento`