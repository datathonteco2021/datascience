# datascience

# 📱: CATER 📱:

## El desafío: desarrollar un modelo que prediga que clientes van a cambiar su dispositivo móvil (terminal) 
El área comercial a este tipo de acción le dice CATER (CAmbio TERminal).

Partiendo de las información de un conjunto de usuarios de Personal correspondientes 5 meses del 2020 y un mes 2021, el desafío consiste en predecir **que clientes son mas propensos a cambiar su terminal**.

El CATER puede darse por la compra de una terminal en nuestras tiendas (SELL OUT) o bien por un cambio o compra en otro tipo de tiendas (cambio de emei), por lo que identificamos a ambos casos como CATER para el desarrollo del modelo.
El universo son clientes del segmento ABONOS: Pospago y Cuentas Claras, Individuos y soho.


## Datasets :open_file_folder:
Para el desarrollo del modelo, se proveen los siguientes conjuntos de datos:
* **cater_muestra.csv**
* **cater_validaciones.csv**
* **metadata.csv**

Estos archivos pueden ser descargados desde [aquí]( https://drive.google.com/drive/folders/1cvvpl_s2nKkuRuhUmTyWLOfJjAzagq8Y?usp=sharing).

Target=1 se considera a los clientes que hayan realizado un CATER a los dos meses posteriores subsiguientes desde el momento de sacar la foto de la información, por ejemplo para la foto de informacion del mes de agosto 2020 se considera 1 al cliente que realizó un cater durante Octubre 2020.

La distribución del target para los distintos periodos es

![image](https://user-images.githubusercontent.com/59797580/140841918-f4bdd249-481d-4906-b8b0-17e0dfdb20c2.png)


##### ** cater_muestra.csv**
Este dataset contiene los  features correspondiente a una muestra aleatoria de más de 170 mil clientes y su correspondiente target. 
##### ** cater_validaciones.csv**
Este dataset contiene los  features correspondiente a una muestra aleatoria de más de 30 mil clientes, pero las columnas target y sus asociadas están vacías. 


El diccionario de variables está en metadata.csv 


## Evaluación :white_check_mark:
Se deberá entregar el  listado clientes de la base cater_validaciones.csv con un valor de probabilidad/score que represente a la chance de realizar un CATER.
- Los valores del target del set de *test* es privado, lo cual significa que los participantes no tendrán acceso a él.

### Métrica
Las predicciones serán evaluadas utilizando la métrica de ** precision_al 10% ** 

## Entregables :paperclip:
### Recomendaciones

Las recomendaciones deben enviarse en un archivo csv con la siguiente estructura: 

- Una columna que identifica a cada perfil con su código de identificación (**cliente_id**).
- Otra columna con el valor de probabilidad/score 

Los valores del csv deberán estar separados por comas, y las variables no deben tener encabezado. Para garantizar la concordancia de las predicciones con el set de testeo
