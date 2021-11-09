# datascience

# 📱: Recomendador 📱:

## El desafío: desarrollar un modelo que prediga que clientes van a cambiar su dispositivo móvil (terminal) el área comercial le dice CATER (CAmbio TERminal).
Partiendo de las información de un conjunto de usuarios de Personal correspondientes 5 meses del 2020 y   un mes 2021 que no contiene la información del target, el desafío consiste en predecir **que clientes son mas propensos a cambiar su terminal**.

## Datasets :open_file_folder:
Para el desarrollo del modelo, se proveen los siguientes conjuntos de datos:
* **cater_muestra.csv**
* **cater_validaciones.csv**

* **metadata.csv**

Estos archivos pueden ser descargados desde [aquí]( https://drive.google.com/drive/folders/1cvvpl_s2nKkuRuhUmTyWLOfJjAzagq8Y?usp=sharing).

La distribución del target para los distintos periodos es
mes	Target 0	Target 1
202008	97,32%	2,68%
202009	94,73%	5,27%
202010	95,23%	4,77%
202011	93,01%	6,99%
202012	94,01%	5,99%
202101	95,68%	4,32%
General	95,05%	4,95%

##### ** cater_muestra.csv**
Este dataset contiene los  features correspondiente a una muestra aleatoria de más de 170 mil clientes. 
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
