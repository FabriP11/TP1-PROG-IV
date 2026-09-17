# Ejercicio 2

Desarrollar una API con ExpressJS para administrar la información académica de
los alumnos de una materia y sus calificaciones. Cada alumno deberá contar con
un nombre y tres notas, que se conservarán en un arreglo interno. No podrán
existir alumnos con el mismo nombre al crear o modificar los registros.

Al consultar las notas de un alumno, la API deberá informar su promedio y su
condición académica: reprobado para promedios menores a 6, aprobado para
promedios de 6 o 7 y promocionado para promedios de 8 o más. El promedio y la
condición son datos derivados, por lo que no deberán almacenarse en el arreglo
interno.

Definir y fundamentar las decisiones de diseño necesarias para modelar la
información y exponer la funcionalidad requerida.




Utilice un ID para identificar a cada alumno de forma única y los siguientes endpoints:
POST /alumnos para crear
GET /alumnos para listar
GET /alumnos/:id para consultar uno
PUT /alumnos/:id para modificar

Corroboro que el nombre sea válido que no esté repetido y que existan exactamente tres notas numéricas entre 0 y 10.
El promedio se calcula al consultar: menor que 6: Reprobado... desde 6 hasta menos de 8: Aprobado y 8 o más: Promocionado