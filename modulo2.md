# MÓDULO 2: Consultas Básicas (CRUD) (1h 15min)

## CRUD
- **C**reate (Crear): INSERT INTO
- **R**ead (Leer): SELECT
- **U**pdate (Actualizar): UPDATE
- **D**elete (Eliminar): DELETE

## Sentencias `SELECT` y `FROM`
- **Seleccionar todas las columnas en una tabla**  
  `SELECT * FROM tabla`
- **Seleccionar columnas específicas en una tabla**  
  `SELECT columna1, columna2 FROM tabla`
- **Renombrar (alias de) columnas**  
  `SELECT columna1 AS nuevo_nombre FROM tabla`

## Filtrar Resultados con `WHERE`:
- **Operadores de comparación**:  
  `=`, `!=`, `<`, `>`, `<=`, `>=`
- **Operadores lógicos**:  
  `AND`, `OR`, `NOT`
- **Operador ENTRE**:  
  `BETWEEN` / `NOT BETWEEN`
- **Operador EN**:  
  `IN` / `NOT IN`
- **Operador SIMILAR A**:  
  `LIKE` / `NOT LIKE` (uso de `%` y `_`)
- **Operador ES NULO**:  
  `IS NULL` / `IS NOT NULL`

## Sentencia `INSERT INTO`
- **Insertar un registro en una tabla**  
  `INSERT INTO tabla (columna1, columna2) VALUES (valor1, valor2)`

## Sentencias `UPDATE` y `SET`
- **Actualizar TODOS los registros en una tabla**  
  `UPDATE tabla SET columna1 = valor1, columna2 = valor2`
- **Actualizar uno o más registros en una tabla con condición**  
  `UPDATE tabla SET columna1 = valor1, columna2 = valor2 WHERE condicion`

## Sentencias `DELETE` y `WHERE`
- **Eliminar TODOS los registros en una tabla**  
  `DELETE FROM tabla`
- **Eliminar uno o más registros en una tabla con condición**  
  `DELETE FROM tabla WHERE condicion`

## Ordenar Resultados con `ORDER BY`:
- **Orden ascendente `ASC`**  
  `ORDER BY columna1 ASC`
- **Orden descendente `DESC`**  
  `ORDER BY columna1 DESC`
- **Ordenar usando más de una columna**  
  `ORDER BY columna1 ASC, columna2 DESC`

## Limitar Resultados con `LIMIT` / `TOP`:
- **Solicitar un número específico de filas**  
  `SELECT * FROM tabla LIMIT 10`