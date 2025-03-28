# EjerciciosSQL-BEECROWD 
--- 
## Nivel 3: 
--- 

### 17. CATEGORIES(Categorías) 
Cuando los datos fueron migrados a la base de datos, hubo un pequeño malentendido con el DBA. Tu jefe necesita que selecciones el ID y el nombre de los productos, cuya categoría comience con **"super"**. 
![Tabla49](Tabla49.png) 
![Tabla50](Tabla50.png) 
![Tabla51](Tabla51.png) 

**Solución:**
![Consulta17](Consulta17.png) 

**Explicación:** 
* *Se realiza un JOIN entre la tabla de productos y la de categorías, filtrando aquellas cuyo nombre empiece con “super”.* 
--- 

### 18. AVERAGE VALUE OF PRODUCTS (Valor promedio de los productos) 
En la empresa donde trabajas se está realizando una encuesta sobre los valores de los productos que se comercializan. Para ayudar a la industria que está realizando esta encuesta, debes calcular y mostrar el valor promedio del precio de los productos. 
**NOTA:** Muestra el valor con dos dígitos después del punto. 
![Tabla52](Tabla52.png) 
![Tabla53](Tabla53.png) 
![Tabla54](Tabla54.png) 

**Solución:** 
![Consulta18](Consulta18.png) 

**Explicación:** 
* *Se utiliza la función AVG para obtener el promedio y la función ROUND para redondear el resultado a dos decimales.* 
--- 

### 19. IMPORTED PRODUCTS (Productos Importados) 
El sector de importaciones de la empresa necesita un informe sobre la importación de productos de nuestros proveedores Sansul. Tu tarea es mostrar el nombre de los productos, el nombre del proveedor y el nombre de la categoría, para aquellos productos suministrados por el proveedor **'Sansul SA'** y cuya categoría sea **'Imported'**. 

![Tabla55](Tabla55.png) 
![Tabla56](Tabla56.png) 
![Tabla57](Tabla57.png) 

**Solución:** 
![Consulta19](Consulta19.png) 

**Explicación:** 
* *Se unen las tres tablas y se filtra tanto por el nombre del proveedor como por el de la categoría.* 
--- 
### 20. ORDERS IN FIRST HALF (Pedidos del primer semestre) 
La auditoría financiera de la empresa nos solicita un informe correspondiente a la primera mitad de 2016. Muestra el nombre del cliente y el número del pedido para los clientes que realizaron pedidos en la primera mitad de 2016. 
![Tabla58](Tabla58.png) 
![Tabla59](Tabla59.png) 
![Tabla60](Tabla60.png) 

**Solución:** 
![Consulta20](Consulta20.png) 

**Explicación:** 
* *Se utiliza la cláusula BETWEEN para filtrar las fechas correspondientes a la primera mitad del año.* 
---

### 21. AMOUNTS BETWEEN 10 AND 20 (Cantidades entre 10 y 20) 
Al entregar el informe sobre la cantidad de productos en stock de la empresa, una parte del informe se ha corrompido, por lo que el encargado de inventario pidió ayuda. Él quiere que muestres el nombre de los productos cuya cantidad se encuentre entre 10 y 20 y cuyo proveedor comience con la letra **'P'**. 
![Tabla61](Tabla61.png) 
![Tabla62](Tabla62.png) 
![Tabla63](Tabla63.png) 

**Solución:** 
![Consulta21](Consulta21.png) 

**Explicación:** 
* *Se filtra tanto por el patrón en el nombre del proveedor como por el rango de la cantidad del producto.* 
--- 

### 22. NUMBER OF CITIES PER CUSTOMERS (Número de ciudades por cliente) 
La junta directiva de la empresa te pidió un informe sencillo sobre cuántas ciudades ha alcanzado la empresa. Para ello, debes mostrar el número de ciudades distintas que aparecen en la tabla de clientes. 
![Tabla4](Tabla64.png) 
![Tabla5](Tabla65.png) 
![Tabla6](Tabla66.png) 

**Solución:** 
![Consulta2](Consulta22.png) 

**Explicación:** 
* *Se utiliza la función COUNT combinada con DISTINCT para contar únicamente las ciudades únicas.*
--- 

### 23. NUMBER OF CHARACTERS (Caracteres de Números)
La Organización Global de Caracteres en los Nombres de las Personas (GOCPN) realizó un censo para determinar cuántos caracteres tienen los nombres de las personas. Para ayudar a la GOCPN, debes mostrar el número de caracteres de cada nombre, ordenados de mayor a menor. 
![Tabla4](Tabla67.png) 
![Tabla5](Tabla68.png) 
![Tabla6](Tabla69.png) 

**Solución:** 
![Consulta2](Consulta23.png) 

**Explicación:** 
* *Se utiliza la función CHARACTER_LENGTH para obtener la longitud de cada nombre y se ordena el resultado de forma descendente.* 
--- 

### 24. TAXES (Impuestos)
Vas a la reunión internacional de impuestos personales y tu propuesta es: Todo individuo con ingresos superiores a 3000 debe pagar un impuesto al gobierno, que equivale al 10% de sus ingresos. Muestra el nombre y el valor del impuesto de cada persona que gana más de 3000, con dos decimales de precisión. 
![Tabla4](Tabla70.png) 
![Tabla5](Tabla71.png) 
![Tabla6](Tabla72.png) 

**Solución:** 
![Consulta2](Consulta24.png) 

**Explicación:** 
* *Se filtra por salario y se calcula el impuesto multiplicando el salario por 0.10, redondeando el resultado a dos decimales.* 
--- 

### 25. MOST FREQUENT (Más frecuentes)
Dada una tabla de una sola columna con valores enteros, ¿cuál es el valor más frecuente, es decir, la moda estadística de los valores? 
![Tabla4](Tabla73.png) 
![Tabla5](Tabla74.png) 
![Tabla6](Tabla75.png) 

**Solución:** 
![Consulta2](Consulta25.png) 

**Explicación:** 
* *Se agrupan los registros por la columna indicada y se cuenta la frecuencia de cada valor, devolviendo el que tiene mayor ocurrencia.* 
--- 
