# Ejercicio 1

Desarrollar una API con ExpressJS para resolver consultas sobre perímetros y
superficies de rectángulos. La solución deberá permitir distinguir, cuando
corresponda, los casos que también constituyen cuadrados.

Definir y fundamentar las decisiones de diseño necesarias para modelar la
información y exponer la funcionalidad requerida.


Utilice el método GET con el recurso `/rectangulos` ya que la API realiza
una consulta y no necesita guardar ni modificar información.

La base y la altura se reciben por medio de query parameters: GET /rectangulos?base=5&altura=3

A partir de estos valores se calculan el perímetro y la superficie y también se determina el tipo de figura comparando la base con la altura.

Valido que ambos parámetros estén presentes, sean numéricos y mayores que cero.
En caso de que los datos sean inválidos se devuelve un código HTTP 400.