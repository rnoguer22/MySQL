# MySQL

[Pincha aqui para acceder al link de este repositorio](https://github.com/rnoguer22/MySQL.git)

Ruben Nogueras Gonzalez 
Pelayo Huerta Mijares

---

[Base de datos de coches de segunda mano](https://www.kaggle.com/datasets/datamarket/venta-de-coches)

---

## ÍNDICE
- [Select](#1)
- [Select into](#2)
- [Where](#3)
- [Delete](#4)
- [Update](#5)
- [Max](#6)
- [Order by](#7)
- [Isnull](#8)
- [Operador Between y and](#9)
- [Drop table](#10)

## SENTENCIAS:

---

#### Select

Con la sentecia select podemos seleccionar elementos de diferentes campos, pudiendo así hacer un filtrado de datos. El comando se usa de la siguiente manera : ```SELECT``` el nombre de los campos que queremos seleccionar ```from``` el nombre de nuestra base de datos. En el ejemplo hemos seleccionado el nombre de la marca y el modelo de cada coche:

<img width="352" alt="Captura de pantalla 2023-03-22 a las 18 27 38" src="https://user-images.githubusercontent.com/91721764/226988434-7aaebb91-252b-44ee-80fc-67302da92d64.png">

Y este sería una parte de nuestro resultado:

<img width="517" alt="Captura de pantalla 2023-03-22 a las 18 28 56" src="https://user-images.githubusercontent.com/91721764/226988644-f52983c7-b8e6-48db-8cf5-ca9552d0a62d.png">

---

#### Select into

Con la sentencia ```select into``` podemos seleccionar una tabla de una base de datos, y hacer lo que queramos con dicha seleccion

<img width="191" alt="image" src="https://user-images.githubusercontent.com/91721762/226993199-f04595d0-fc4e-4487-ad5c-0a38f555da5c.png">

Por ejemplo, nosotros hemos seleccionado el campo field3, que es el campo referente a la marca, y hemos añadido el valor Ferrari, como podemos ver

<img width="635" alt="image" src="https://user-images.githubusercontent.com/91721762/226994091-05c64157-b2f3-4726-97e8-e3cbbbd0d60c.png">

Como podemos ver, como no hemos indicado que valores añadimos en los demas campos, nos lo ha rellenado con valores nulos por defecto

---

#### Where

Con la sentencia where podemos seleccionar una condicion mas especifica, por ejemplo, podemos seleccionar, dentro del campo donde se encuentra el modelo del coche, el modelo en especifico que estamos buscando

<img width="295" alt="image" src="https://user-images.githubusercontent.com/91721762/226992416-a162d33a-a03f-4b9a-a913-376a362296e0.png">

Por ejemplo, nosotros, que somos amantes de los Ford Mustang, estamos buscando los mustang que se encuentran en nuestra base de datos

<img width="629" alt="image" src="https://user-images.githubusercontent.com/91721762/226992705-4ae93e6c-32cc-474b-ad03-b774d6623977.png">

---

#### Delete

Con la sentencia delete podemos eliminar campos o registros aplicando determinadas condiciones. Se usa de la siguiente forma: ```DELETE from``` nombre de la base de datos ```where``` una condición. En nuestro ejemplo eliminamos todos los coches de la marca Citroen:

<img width="388" alt="Captura de pantalla 2023-03-22 a las 18 35 56" src="https://user-images.githubusercontent.com/91721764/226991428-0ff04541-8615-4941-a4a7-15776a71e1e1.png">

Ahora si en nuestra base de datos buscamos en el campo de marcas Citroen, vemos que no obtenemos ningún dato:

<img width="947" alt="Captura de pantalla 2023-03-22 a las 18 41 56" src="https://user-images.githubusercontent.com/91721764/226991848-7a177feb-626d-44f4-ba9c-79358ceb14c9.png">

#### Update

Con la sentencia update podemos actualizar el valor de determinadas celdas. Se usa de la siguiente forma: 
```UPDATE```el nombre de la base de datos
```SET```el campo que queremos cambiar = nuevo valor
En nuestro ejemplo cambiamos el color de todos los coches a dorado:

<img width="200" alt="Captura de pantalla 2023-03-22 a las 18 52 29" src="https://user-images.githubusercontent.com/91721764/226995422-5a2cb569-6c8f-45eb-b43e-39d4e8791e76.png">

Y este es el resultado:

<img width="382" alt="Captura de pantalla 2023-03-22 a las 18 52 18" src="https://user-images.githubusercontent.com/91721764/226995498-7f5d2c7e-f86a-4c99-bb01-8605f023594b.png">

Además, podemos añadir condiciones con el comado ```WHERE```. En nuestro caso pintamos a todos los Ford de azul:

<img width="260" alt="Captura de pantalla 2023-03-22 a las 18 58 45" src="https://user-images.githubusercontent.com/91721764/226995886-79dd4da8-a3a9-4c0c-b902-614e374ade16.png">

<img width="215" alt="Captura de pantalla 2023-03-22 a las 19 02 28" src="https://user-images.githubusercontent.com/91721764/226996727-94ba859e-f4bf-4797-b04c-2b608c372a39.png">

#### Max

El comando ```max``` nos devuelve el valor maximo de una tabla, de un campo de una tabla, etc.

Por ejemplo, escojamos el vehiculo con el precio mas alto:

<img width="143" alt="image" src="https://user-images.githubusercontent.com/91721762/226996995-6c7fb462-0d20-48e8-a9bb-55404bf2d84b.png">

Y su valor es 99999:

<img width="88" alt="image" src="https://user-images.githubusercontent.com/91721762/226997439-c449a667-d448-4d63-850d-b75765fd6f51.png">

#### Order by

El comando ```ORDER BY``` no sirve para ordenar un campo por orden alfabético o de mayor a menor. Podemos determinar si queremos ordenar los datos de forma ascendente con ```ASC``` o descendente ```DESC```. Se usa de la siguiente forma: 

```SELECT * from``` nombre de la base de datos
```ORDER BY``` nombre del campo que queremos ordenar ```ASC/DESC```

EN nuestro ejemplo ordenamos los coches por provincias:

<img width="225" alt="Captura de pantalla 2023-03-22 a las 19 05 19" src="https://user-images.githubusercontent.com/91721764/226998394-6e596742-0808-439c-a22c-d11926c1c5be.png">

<img width="357" alt="Captura de pantalla 2023-03-22 a las 19 10 29" src="https://user-images.githubusercontent.com/91721764/226998501-6b177f1f-1136-48d0-922f-e3cdd7a3ec84.png">

#### Isnull

El comando ```ISNULL``` podemos localizar los valores nulos de diferentes campos. Se usa de la siguiente forma: 

```SELECT``` nombre del campo que queremos seleccionar
```WHERE``` nombre del campo condicion ```ISNULL```

En nuestro ejemplo seleccionamos las marcas de los coches que no están registrados en ninguna provincia:

<img width="240" alt="Captura de pantalla 2023-03-22 a las 19 14 09" src="https://user-images.githubusercontent.com/91721764/226999964-14f6b33c-ce56-4863-aac6-7cf777905ebe.png">

<img width="104" alt="Captura de pantalla 2023-03-22 a las 19 17 29" src="https://user-images.githubusercontent.com/91721764/227000038-543d10df-bec5-4e46-9b02-1ee5b1ed0462.png">

---

#### Operador BETWEEN y AND

Con el operador ```BETWEEN``` podemos seleccionar los valores que esten dentro del intervalo que queramos, por ejemplo, vamos a seleccionar la marca y el modelo de los coches que cuesten entre 50000 y 60000 euros:

El codigo seria el siguiente:

<img width="241" alt="image" src="https://user-images.githubusercontent.com/91721762/227000759-7f77b527-e8dc-4281-b3f5-cb50f54cedb3.png">

Y el resultado es 

<img width="222" alt="image" src="https://user-images.githubusercontent.com/91721762/227000873-ab5d225d-257e-4e06-8a4c-9d792ac39f55.png">

---

#### Drop table

Con el operador ```DROP TABLE``` eliminamos todos los datos almacenados en nuestra tabla. Se usa de la siguiente forma: ```DROP TABLE``` nombre de la tabla. 

<img width="228" alt="Captura de pantalla 2023-03-22 a las 19 20 21" src="https://user-images.githubusercontent.com/91721764/227001377-d719441b-83a6-4b20-a28e-2761cb7609c5.png">

Y vemos que efectivamente eliminamos la tabla completamente:

<img width="397" alt="Captura de pantalla 2023-03-22 a las 19 20 33" src="https://user-images.githubusercontent.com/91721764/227001488-fb65b25d-a046-4877-bcf5-e8e984caf661.png">

