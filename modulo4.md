### MÓDULO 4: Combinación de Tablas (JOINs) y Subconsultas (1h)

## Concepto de JOINs:
- **Relaciones entre tablas**.

## Tipos de JOINs más comunes:
- Obtener filas coincidentes entre tablas  
  `INNER JOIN`
- Incluir todas las filas de la tabla izquierda  
  `LEFT JOIN` = `LEFT OUTER JOIN`
- Incluir todas las filas de la tabla derecha (mencionar brevemente)  
  `RIGHT JOIN` = `RIGHT OUTER JOIN`

## Subconsultas (Subqueries):
- **¿Qué es una subconsulta?**  
  También se les conoce como consulta interna o anidada, es una consulta SQL que se encuentra dentro de otra consulta SQL. Es una consulta que se ejecuta primero y su resultado es utilizado por la consulta principal.
- **¿Cuándo utilizarlas?**
  + **Filtrar datos basándose en resultados de otra consulta**: Este es el uso más común. Por ejemplo, quieres encontrar todos los clientes que han realizado pedidos en el último mes.  
  Ej.: `SELECT nombre_cliente FROM clientes
WHERE id_cliente IN (SELECT id_cliente FROM pedidos WHERE fecha_pedido >= DATE_SUB(CURRENT_DATE(), INTERVAL 1 MONTH));`
  + **Realizar cálculos agregados para el filtrado**: Si necesitas filtrar por un valor que es el resultado de una función de agregación (como `SUM`, `AVG`, `COUNT`), a menudo una subconsulta es la mejor opción. Por ejemplo, encontrar los productos que tienen un precio superior al precio promedio de todos los productos.  
  Ej.: `SELECT nombre_producto, precio FROM productos
WHERE precio > (SELECT AVG(precio) FROM productos);`
  + **Verificar la existencia de registros relacionados**: Puedes usar `EXISTS` o `NOT EXISTS` para verificar si hay filas relacionadas en otra tabla. Por ejemplo, encontrar vendedores que no han realizado ninguna venta.  
  Ej.: `SELECT nombre_vendedor FROM vendedores
WHERE NOT EXISTS (SELECT 1 FROM ventas WHERE ventas.id_vendedor = vendedores.id_vendedor);`
  + **Crear tablas temporales (tablas derivadas) para uniones o análisis**: Cuando necesitas realizar operaciones intermedias o uniones complejas, definir una subconsulta en la cláusula `FROM` puede ser muy útil.  
  Ej.: `SELECT c.nombre_cliente, SUM(p.total) AS total_comprado FROM clientes c
JOIN (SELECT id_cliente, SUM(cantidad * precio_unitario) AS total
      FROM pedidos
      GROUP BY id_cliente) AS p ON c.id_cliente = p.id_cliente
WHERE p.total > 1000;`
  + **Actualizar o eliminar datos basándose en criterios complejos**: Las subconsultas también se pueden usar en las cláusulas `UPDATE` y `DELETE`.  
  Ej.: `DELETE FROM productos WHERE id_producto IN (SELECT id_producto FROM inventario WHERE stock = 0);`
- Subconsultas en la cláusula `WHERE`.
- Subconsultas como origen de datos.

## Ejercicios Prácticos y Preguntas y Respuestas (15min)
- Resolver un par de problemas que integren los conceptos vistos.
- Sesión abierta para preguntas y respuestas.
