# SQL: Lenguaje de Consultas Estructuradas - 4h

## A QUIÉN ESTÁ DIRIJIDO:
Este curso está diseñado para principiantes y personas que deseen reforzar sus conocimientos en la creación de consultas SQL para extraer y manipular datos de bases de datos relacionales.

## TEMARIO:

### [MÓDULO :one:: Introducción a las Bases de Datos y SQL (45min)](https://github.com/mauricioge/sql/blob/main/modulo1.md)
- **¿Qué es una Base de Datos Relacional?**
  + Conceptos clave.
  + Ejemplos de sistemas de gestión de bases de datos relacionales (RDBMS)
- **¿Qué es SQL y para qué sirve?**
  + Definición y propósito del lenguaje SQL.
  + Categorías de comandos SQL: DDL, DML, DCL, TCL.
- **Entorno de Trabajo (Demostración Rápida)**
  + Instalación y configuración de un Cliente SQL (DBeaver, MySQL Workbench o PHPMyAdmin).
  + Conexión a una base de datos de ejemplo.
  + Concepto de `SELECT` simple para ver una tabla.

### MÓDULO :two:: Consultas Básicas de Selección (1h 15min)
- **Sentencia `SELECT`**
  + Seleccionar todas las columnas (`SELECT *`).
  + Seleccionar columnas específicas (`SELECT columna1, columna2`).
  + Alias de columnas (`AS`).
- **Sentencia `FROM`**
- **Filtrado de Datos con `WHERE`:**
  + Operadores de comparación (`=`, `!=`, `<`, `>`, `<=`, `>=`).
  + Operadores lógicos (`AND`, `OR`, `NOT`).
  + `BETWEEN` y `NOT BETWEEN`.
  + `IN` y `NOT IN`.
  + `LIKE` y `NOT LIKE` (uso de `%` y `_`).
  + `IS NULL` y `IS NOT NULL`.
- **Sentencia `INSERT INTO`**
- **Sentencia `UPDATE`**
- **Sentencia `DELETE`**
- **Ordenamiento de Resultados (`ORDER BY`):**
  + Orden ascendente (`ASC`) y descendente (`DESC`).
  + Ordenar usando múltiples columnas.
- **Limitando Resultados (`LIMIT` / `TOP`):**
  + Cómo obtener un número específico de filas.

### MÓDULO :three:: Agregación y Agrupación de Datos (1h)
- **Funciones de Agregación:**
  + `COUNT()`: Contar filas.
  + `SUM()`: Sumar valores numéricos.
  + `AVG()`: Calcular el promedio.
  + `MIN()`: Encontrar el valor mínimo.
  + `MAX()`: Encontrar el valor máximo.
- **Agrupación de Resultados (`GROUP BY`):**
  + Agrupar datos por una o más columnas.
  + Uso de funciones de agregación con `GROUP BY`.
- **Filtrado de Grupos (`HAVING`):**
  + Diferencia entre `WHERE` y `HAVING`.
  + Filtrar resultados después de la agrupación.

### MÓDULO :four:: Combinación de Tablas (JOINs) y Subconsultas (1h)
- **Concepto de JOINs:**
  + Relaciones entre tablas.
- **Tipos de JOINs más comunes:**
  + `INNER JOIN`: Obtener filas coincidentes entre tablas.
  + `LEFT JOIN` (o `LEFT OUTER JOIN`): Incluir todas las filas de la tabla izquierda.
  + `RIGHT JOIN` (o `RIGHT OUTER JOIN`): Incluir todas las filas de la tabla derecha (mencionar brevemente).
- **Subconsultas (Subqueries):**
  + Concepto y cuándo utilizarlas.
  + Subconsultas en la cláusula `WHERE`.
  + Subconsultas como origen de datos.
- **Ejercicios Prácticos y Preguntas y Respuestas (15min)**
  + Resolver un par de problemas que integren los conceptos vistos.
  + Sesión abierta para preguntas y respuestas.

## Consideraciones Adicionales para el Curso:
- **Práctica Constante:** Es fundamental que cada módulo incluya ejercicios prácticos para que los participantes puedan aplicar lo aprendido.
- **Base de Datos de Ejemplo:** Utiliza una base de datos sencilla y consistente (por ejemplo, Northwind, Sakila o una base de datos creada específicamente para el curso con pocas tablas).
- **Demostraciones en Vivo:** Realiza demostraciones en tiempo real de cada concepto.
- **Recursos Adicionales:** Proporciona materiales de apoyo, como una guía de referencia rápida de SQL, enlaces a documentación oficial o plataformas de práctica online.
Espero que este temario te sea de gran utilidad para crear tu curso de SQL. ¡Mucho éxito!
