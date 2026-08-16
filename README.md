¿Cuántas filas devuelve cada consulta y por qué son distintas? Explicá con ejemplos concretos de los datos qué filas se eliminaron con UNION.

En el caso de la consulta Union devuelve 11 filas y en el caso del UNION ALL devuelve 14 ya que en el primer caso elimina las consultas de los productos 103, 104 y 106 que se repite en ambas tiendas.

¿Por qué UNION ALL es más eficiente que UNION? ¿Qué operación adicional realiza UNION internamente que consume más recursos?
Debido a que el UNION ALL devuelve todos los resultados, en cambio el UNION elimina los duplicados.

¿En qué casos de negocio usarías cada uno? Dá al menos dos ejemplos reales distintos a los del ejercicio.
UNION lo utilizaria en caso que quiera ver todos los clientes que tiene la empresa o productos sin distinguir cada tienda. Mirar la norma a nivel global.
Mientras que UNION ALL lo haría si quisiera ver todas las ventas que se realizaron entre ambas tiendas, sin importar que haya cosas duplicadas.

¿Qué pasa si las columnas de ambas consultas no coinciden en número o tipo? ¿Qué error genera SQL?
Te da un error de sintaxis ya que deben coincidir las columnas en la union,