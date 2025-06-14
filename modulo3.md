# MÓDULO 3: Agregación y Agrupación de Resultados (1h)

## Funciones de Agregación

- **¿Qué son las funciones de agregación?**  
  Son funciones que realizan un cálculo **sobre un conjunto de filas** y devuelven un único valor resumido.
- **Contar filas con `COUNT()`**:  
  `SELECT COUNT(*) FROM tabla;`
- **Contar valores únicos con `COUNT(DISTINCT)`**:  
  `SELECT COUNT(DISTINCT columna) FROM tabla;`
- **Sumar valores numéricos con `SUM()`**:  
  `SELECT SUM(columna) FROM tabla;`
- **Calcular el promedio con `AVG()`**:  
  `SELECT AVG(columna) FROM tabla;`
- **Encontrar el valor mínimo con `MIN()`**:  
  `SELECT MIN(columna) FROM tabla;`
- **Encontrar el valor máximo con `MAX()`**:  
  `SELECT MAX(columna) FROM tabla;`

## Funciones de Agrupación

- **¿Qué son las funciones de agrupación?**  
  Son funciones que agrupan filas a partir de un atributo y aplican una función a cada grupo.
- **Agrupación de Resultados con `GROUP BY`:**
  + Agrupar datos por una o más columnas  
    `SELECT columna1, columna2, ... FROM tabla GROUP BY columna1, columna2;`
  + Uso de funciones de agregación con `GROUP BY`  
    `SELECT columna1, funcion_agregacion(columna2) FROM tabla GROUP BY columna1;`
- **Filtrado de Grupos con `HAVING`:**
  + Diferencia entre `WHERE` y `HAVING`  
    `SELECT `
  + Filtrar resultados después de la agrupación.
