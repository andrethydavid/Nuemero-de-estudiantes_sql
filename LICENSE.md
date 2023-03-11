# PRIMERO 

Proyecto estudaintes 
Vamos medir el comportamiento de ellos con sus estudios diarios

# FUNCIONES BASICAS 

```

SELECT *
FROM platzi.alumnos AS alumnos
FETCH FIRST 5 ROWS ONLY;

```
![image](https://user-images.githubusercontent.com/72534486/224216209-29a7aa3e-fe2c-4947-9115-785ad18befc4.png)


```

SELECT *
FROM platzi.alumnos
LIMIT 5;


```

![image](https://user-images.githubusercontent.com/72534486/224216422-a324277c-fe08-4317-8326-19b29f303d9b.png)


#  windows functions

```

SELECT *
FROM (
	SELECT ROW_NUMBER () OVER() AS row_id, *
	FROM platzi.alumnos
 )AS alumnos_with_row_nums
 WHERE row_id < 6
;

```
![image](https://user-images.githubusercontent.com/72534486/224216898-ea7dff20-f8d9-4f90-981d-16fe53933128.png)

.
