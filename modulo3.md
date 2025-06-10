# MÓDULO :three:: Agregación y Agrupación de Resultdos (1h)

## Funciones de Agregación

- **`COUNT()`**: Contar filas  
  `SELECT COUNT(*) FROM tabla;`
- **`COUNT(DISTINCT)`**: Contar valores únicos  
  `SELECT COUNT(DISTINCT columna) FROM tabla;`
- **`SUM()`**: Sumar valores numéricos  
  `SELECT SUM(columna) FROM tabla;`
- **`AVG()`**: Calcular el promedio  
  `SELECT AVG(columna) FROM tabla;`
- **`MIN()`**: Encontrar el valor mínimo  
  `SELECT MIN(columna) FROM tabla;`
- **`MAX()`**: Encontrar el valor máximo  
  `SELECT MAX(columna) FROM tabla;`

## Funciones de Agrupación

- **Agrupación de Resultados con `GROUP BY`:**
  + Agrupar datos por una o más columnas  
    `SELECT columna1, columna2, ... FROM tabla GROUP BY columna1, columna2;`
  + Uso de funciones de agregación con `GROUP BY`  
    `SELECT columna1, funcion_agregacion(columna2) FROM tabla GROUP BY columna1;`
- **Filtrado de Grupos con `HAVING`:**
  + Diferencia entre `WHERE` y `HAVING`  
    `SELECT `
  + Filtrar resultados después de la agrupación.
