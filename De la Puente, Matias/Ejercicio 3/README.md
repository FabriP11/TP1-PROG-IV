# Ejercicio 3

Desarrollar una API con ExpressJS para administrar tareas y su estado de avance.
Cada tarea deberá contar con un nombre y un estado que indique si fue
completada, y esta información se conservará en un arreglo interno.

No podrán existir tareas con el mismo nombre. La API deberá facilitar consultas
que permitan diferenciar las tareas completadas de las pendientes.

Definir y fundamentar las decisiones de diseño necesarias para modelar la
información y exponer la funcionalidad requerida.





Desarrolle una API con ExpressJS para administrar tareas y su estado.. Cada tarea se guarda en un arreglo interno con su nombre y un valor booleano que indica si está completada o pendiente y no se permiten tareas con nombres repetidos.
Para crear tareas se utiliza POST /tareas y para consultarlas GET /tareas y s e puede filtrar por estado usando GET /tareas?estado=completadas o GET /tareas?estado=pendientes...
Valido que el nombre no esté vacío, que no exista otra tarea con el mismo nombre y que el estado utilizado en los filtros sea válido.