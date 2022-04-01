# Operadores Comparacion Oracle
#### operadores relacionales, simbolos que nos permiten realizar operaciones matematicas unir cadena de caracteres, hacer comparaciones, entre otras.

#### tenemos los siguientes Tipos de operadores.
* [x] Operadores relacionales o de comparacion
  * Igual  :  = 
  * Distinto a : !=
  * Mayor :  >
  * Menor :  <
  * Mayor o Igual :  >=
  * Menor o Igual :  <=
* [ ] Operadores Aritmeticos
* [ ] Operadores de concatenación
* [ ] Operadores logicos

```sql
select * from articulos;
```
 | CODIGO            | NOMBRE           |  DESCRIPCION   |   PRECIO   |
 | ------------------|:----------------:|---------------:|-----------:|
 | 1            | impresora           |  Epson Stylus C45   |   400.80   |
 | 2            | impresora           |  Epson Stylus C85   |   500   |
 | 3            | monitor           |  Samsung 14   |   800   |
 | 4            | teclado           |  ingles Biswal   |   100   |
 | 5            | teclado           |  español Biswal   |   90   |
 | 6            | mouse           |  Genius   |   20   |
 | 7            | mouse           |  teclado blanco   |   30   |
 | 8            | Computadora           |  Dell   |   2000   |

#### Ejemplos :

> " = " : nos traera todo los datos que contengan el nombre monitor
```sql
select * from articulos where nombre = 'monitor';
```
| CODIGO            | NOMBRE           |  DESCRIPCION   |   PRECIO   |
| ------------------|:----------------:|---------------:|-----------:|
| 3            | monitor           |  Samsung 14   |   800   |


> " != " : nos traera los datos que su nombre sea diferente de monitor.
```sql
select * from articulos where nombre != 'monitor';
```
 | CODIGO            | NOMBRE           |  DESCRIPCION   |   PRECIO   |
 | ------------------|:----------------:|---------------:|-----------:|
 | 1            | impresora           |  Epson Stylus C45   |   400.80   |
 | 2            | impresora           |  Epson Stylus C85   |   500   |
 | 4            | teclado           |  ingles Biswal   |   100   |
 | 5            | teclado           |  español Biswal   |   90   |
 | 6            | mouse           |  Genius   |   20   |
 | 7            | mouse           |  teclado blanco   |   30   |
 | 8            | Computadora           |  Dell   |   2000   |


> " > " : traera todo los articulos cuyo precio sea **mayor** que .
```sql
select * from articulos where precio > 100;
```
 | CODIGO            | NOMBRE           |  DESCRIPCION   |   PRECIO   |
 | ------------------|:----------------:|---------------:|-----------:|
 | 1            | impresora           |  Epson Stylus C45   |   400.80   |
 | 2            | impresora           |  Epson Stylus C85   |   500   |
 | 3            | monitor           |  Samsung 14   |   800   |
 | 8            | Computadora           |  Dell   |   2000   |

> " < " : traera todo los articulos cuyo precio sea ** menor** que...
```sql
select * from articulos where precio < 100;
```
 | CODIGO            | NOMBRE           |  DESCRIPCION   |   PRECIO   |
 | ------------------|:----------------:|---------------:|-----------:|
 | 5            | teclado           |  español Biswal   |   90   |
 | 6            | mouse           |  Genius   |   20   |
 | 7            | mouse           |  teclado blanco   |   30   |


> " >= " : traera todo los articulos cuyo precio sea **mayor o igual ** que...
```sql
select * from articulos where precio >= 100;
```
 | CODIGO            | NOMBRE           |  DESCRIPCION   |   PRECIO   |
 | ------------------|:----------------:|---------------:|-----------:|
 | 1            | impresora           |  Epson Stylus C45   |   400.80   |
 | 2            | impresora           |  Epson Stylus C85   |   500   |
 | 3            | monitor           |  Samsung 14   |   800   |
 | 4            | teclado           |  ingles Biswal   |   100   |
 | 8            | Computadora           |  Dell   |   2000   |
 
 > " <= " : traera todo los articulos cuyo precio sea **menor o igual ** que...
```sql
select * from articulos where precio <= 100;
```
 | CODIGO            | NOMBRE           |  DESCRIPCION   |   PRECIO   |
 | ------------------|:----------------:|---------------:|-----------:|
 | 4            | teclado           |  ingles Biswal   |   100   |
 | 5            | teclado           |  español Biswal   |   90   |
 | 6            | mouse           |  Genius   |   20   |
 | 7            | mouse           |  teclado blanco   |   30   |

