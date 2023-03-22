# MySQL

[Pincha aqui para acceder al link de este repositorio](https://github.com/rnoguer22/MySQL.git)

Ruben Nogueras Gonzalez
Pelayo Huerta Mijares

---

[Base de datos de coches de segunda mano](https://www.kaggle.com/datasets/datamarket/venta-de-coches)

---

## Sentencias:

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





