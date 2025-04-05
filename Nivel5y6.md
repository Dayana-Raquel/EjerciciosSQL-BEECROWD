# EjerciciosSQL-BEECROWD 
--- 
## Nivel 5: 
--- 

### 34. SEPTEMBER RENTALS(Alquileres de Septiembre) 
El videoclub está preparando su informe semestral y necesita tu ayuda. Solo tienes que seleccionar el nombre de los clientes y la fecha de alquiler, de entre los alquileres realizados en septiembre de 2016.
![Tabla100](imagenes/Tabla100.png) 
![Tabla101](imagenes/Tabla101.png) 
![Tabla102](imagenes/Tabla102.png) 

**Solución:**
![Consulta34](imagenes/Consulta34.png) 

**Explicación:** 
* *Se realiza una unión (JOIN) entre las tablas customers y rentals utilizando la clave foránea id_customers.*

*Se filtran las filas cuya fecha de alquiler (rentals_date) esté entre el 1 y el 30 de septiembre de 2016, inclusive.

*Es importante asegurarse de que las fechas estén en el formato YYYY-MM-DD para evitar errores de formato de fecha.* 
---

### 35. NO RENTAL(Sin Alquiler) 
El videoclub planea realizar una promoción para clientes que aún no han alquilado.
Su tarea es proporcionarnos el ID y el nombre de los clientes que aún no han alquilado. Ordene la salida por ID.
![Tabla107](imagenes/Tabla103.png) 
![Tabla106](imagenes/Tabla104.png) 
![Tabla105](imagenes/Tabla105.png) 

**Solución:**
![Consulta35](imagenes/Consulta35.png) 

**Explicación:** 
* *Se seleccionan los clientes que no tienen registros en la tabla de ubicaciones, utilizando una subconsulta con NOT EXISTS.* 
---


### 36. LEAGUE(Liga) 
La Liga Internacional de Excavaciones Subterráneas es un éxito entre los deportes alternativos. Sin embargo, el personal encargado de organizar los eventos no entiende nada de informática; solo saben excavar y las reglas del deporte. Por ello, te contrataron para resolver el problema de la Liga.
Selecciona a los tres primeros clasificados con la frase inicial "Podio:" y selecciona a los dos últimos, que descenderán a una liga inferior con la frase inicial "Degradado:".
![Tabla106](imagenes/Tabla106.png) 
![Tabla107](imagenes/Tabla107.png) 
![Tabla108](imagenes/Tabla108.png) 

**Solución:**
![Consulta36](imagenes/Consulta36.png) 

**Explicación:** 
* *Se combinan dos consultas: una para los tres primeros lugares y otra para los dos últimos, utilizando UNION ALL y CONCAT para formatear los nombres.* 
---

### 37. STUDENTS GRADES(Calificaciones de los estudiantes) 
El semestre terminó en la Universidad de Transilvania del Sur. Se cerraron todos los grados, y solo Alquimia 104 no ha publicado su lista de estudiantes aprobados.
Por lo tanto, debe mostrar la palabra "Aprobado:" junto al nombre del estudiante y la calificación para aquellos aprobados (calificación ≥7).
Recuerde ordenar la lista por grado (primero las calificaciones más altas).
![Tabla109](imagenes/Tabla109.png) 
![Tabla110](imagenes/Tabla110.png) 
![Tabla111](imagenes/Tabla111.png) 

**Solución:**
![Consulta37](imagenes/Consulta37.png) 

**Explicación:** 
* *Se calculan las notas promedio de los estudiantes y se filtran aquellos con promedio mayor o igual a 7.0.* 
---

### 38. RICHARD'S MULTIVERSE(El Multiverso de Richard) 
Richard es un científico famoso por su teoría del multiverso, donde describe cada conjunto hipotético de universos paralelos mediante una base de datos. Gracias a eso, ahora tienes un trabajo.
Como primera tarea, debes seleccionar cada Richard de las dimensiones C875 y C774, junto con su probabilidad de existencia (el famoso factor N) con tres decimales de precisión.
Recuerda que el factor N se calcula multiplicando el valor omega por 1618. Los datos deben ordenarse por el valor omega más bajo.

![Tabla112](imagenes/Tabla112.png) 
![Tabla113](imagenes/Tabla113.png) 
![Tabla114](imagenes/Tabla114.png) 

**Solución:**
![Consulta38](imagenes/Consulta38.png) 

**Explicación:** 
* *Se seleccionan registros de vida en dimensiones específicas cuyo nombre comienza con 'Richard', calculando el "Fator N" como el producto de omega por 1.618.* 
---

### 39. THE SENSOR MESSAGE(El mensaje del sensor) 
Un sensor captura la temperatura ambiente cada minuto. Los registros también tienen un marcador que, cada vez que la temperatura cambia, aumenta con respecto a la última captura. Cuando el sensor almacena 15 registros, prepara un mensaje para enviarlo a la computadora central. Para reducir el tamaño del mensaje, el sensor compacta los registros de temperatura cercanos y suma el número de registros compactados. Cree una consulta para resolver este problema, mostrando la temperatura y el número de registros coincidentes.

![Tabla115](imagenes/Tabla115.png) 
![Tabla116](imagenes/Tabla116.png) 
![Tabla117](imagenes/Tabla117.png) 

**Solución:**
![Consulta39](imagenes/Consulta39.png) 

**Explicación:** 
* *Se utiliza una CTE para seleccionar sensores con temperaturas entre 20 y 30 grados, ordenando los resultados por ID de sensor.* 
---

### 40. PACKAGE DELIVERY(Entrega de paquetes)
Trabaja para una empresa de mensajería y necesita indicar urgentemente el año y el nombre de todos los clientes que enviaron y recibieron paquetes azules o desde el año 2015. Además, debe indicar que la dirección del remitente o destinatario no es de Taiwán. Además, debe ordenar el resultado por año de forma decreciente. 

![Tabla118](imagenes/Tabla118.png) 
![Tabla119](imagenes/Tabla119.png) 
![Tabla120](imagenes/Tabla120.png) 

**Solución:**
![Consulta40](imagenes/Consulta40.png) 

**Explicación:** 
* *Se extraen los años y nombres de clientes que enviaron o recibieron paquetes azules, asegurando que no haya duplicados con DISTINCT.* 
---
