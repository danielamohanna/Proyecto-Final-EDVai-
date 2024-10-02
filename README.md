# Proyecto-Final-EDVai-
### Licorerias en Iowa
Proyecto final del Bootcamp Data Analysis - EDVai Septiembre 2024


------------

#### Dataset
Se utilizo el dataset publico 'iowa_liquor_sales' de GCP (Google Cloud Platform).

![Dataset bronce](https://github.com/user-attachments/assets/2658e0a5-1a67-45f2-89c9-229f1e1e6f80)

------------

#### Plan de metricas

![Plan de metricas](https://github.com/user-attachments/assets/0db39c71-6404-41b7-91af-724c8dce35c0)


------------

#### Objetivos

1) Poder ver los condados con mayor consumo de botellas.
2) Ver el ingreso de dichas ventas.
3) Conocer la variedad de licores consumidos dentro de Iowa
4) Poder discriminar por condado cuantas tiendas tiene, sus proveedores, cantidad de botellas vendidas y el profit de las mismas.


------------


------------

## Proceso de armado

El dataset pasa por un proceso de ETL 

![Capas Bronce-Silver-Gold](https://github.com/user-attachments/assets/4b135eb4-46d0-4f39-aa05-92f73b0ac373)

##### Las querys que se utilizaron para la creacion de tablas en la etapa "Silver":

_Creacion de la Fact Table Information_

![Creacion FactTable](https://github.com/user-attachments/assets/5e109b38-0ef2-4587-b7e0-700f242a36e0)

_Creacion de la DimTable Condado_

![Creacion DimCondado](https://github.com/user-attachments/assets/b19b7e73-bd25-405d-bd4b-02965bac78f5)


_Creacion de la DimTable Categoria_

![Creacion DimCategoria](https://github.com/user-attachments/assets/ebab0b71-742a-4199-b1a6-114a4fdf5568)



------------


#### De esta manera generamos el _DER_

![Copy of Modelo de datos Delivery](https://github.com/user-attachments/assets/86364f39-22f8-47cc-b366-ab957ea53ebf)



------------

#### Pasamos a Power BI

Se hace la correspondiente conexcion del dataset con Power BI para su modelado final.


![Carga en PBI](https://github.com/user-attachments/assets/d7f2f719-8558-4442-84f7-8341d8867fda)



------------


Y se realizan las siguientes _DAX_ que nos van a dar los resultados necesarios para lograr los objetivos:

- _Botellas Vendidas_

> ![DAX Botellas vendidas](https://github.com/user-attachments/assets/c91b9499-4bc4-46e3-8248-779ca60728c6)

- _Total Categorias_

> ![DAX Categoria](https://github.com/user-attachments/assets/c12fdd97-dba7-4298-956a-f4d7295a283b)

- _Total Condados_

> ![DAX Condados](https://github.com/user-attachments/assets/6e48be6b-c81f-450f-ad7d-f2e8453e90b2)

- _Total Proveedores_

> ![DAX Total proveedores](https://github.com/user-attachments/assets/740ed516-b5a4-4d05-ac53-460e85f98be4)

- _Total Tiendas_

> ![DAX Total tiendas](https://github.com/user-attachments/assets/3694cc72-7f6d-471c-9451-a8490193f06e)


------------


------------


####Desarrollo del dashboard

La eleccion del fondo fue totalmente subjetiva, por eso el color queriendo hacer referencia al alcohol, como el Whishky o Champagne, con una ilustración que parezca liquido.

Y para poder responder a los objetivos elegí las siguientes visualizaciones:

##### - Tres Tarjetas 
De las cuales la de _Tiendas_ y _Proveedores_ estan conectadas con las otras tablas para ir mostrando las estadisticas deseadas.

![etiqueta tiendas](https://github.com/user-attachments/assets/426c188f-ae50-488a-b28c-9cd0c5c1ebc3) ![etiqueta proveedores](https://github.com/user-attachments/assets/d8c2baeb-76fb-40ed-83f4-a7ba3aa8af79) 

![etiqueta licores](https://github.com/user-attachments/assets/e5e1bb30-79ca-49c0-8a5b-cba2b93857a0)

##### - Dos Segmentaciones de Datos
Para poder buscar de manera especifica la informacion que querramos por condado, por licor o por ambos.

![segmentacion condado](https://github.com/user-attachments/assets/4c0b7e2a-f6ff-46b0-a36d-e6348565eb51) 

![segmentacion licores](https://github.com/user-attachments/assets/ef43e4c3-e217-4705-80bb-9b0b51f2779a)

##### - Dos Graficos de Barras Apiladas
Que nos muestran en orden descendente la cantidad de botellas vendidas y el total de esas ventas.

![graficos botella](https://github.com/user-attachments/assets/ba383fd6-600e-454e-a52c-296494312f1c)

![graficos profit](https://github.com/user-attachments/assets/d35fe634-fe7f-48f9-8392-0acffe23a502)


------------


------------

### Conclusión 

Con el dashborad creado podemos responder:

> 1) Poder ver los condados con mayor consumo de botellas:

Top 5 condados que mas cantidad de botellas consumen: 
- Polk
- Linn
- Scott
- Black Hawk
- Johnson

> 2) Ver el ingreso de dichas ventas:

- Polk: 74.525.715
- Linn: 29.047.509
- Scott: 23.671.987
- Johnson: 19.951.854
- Black Hawk: 18.638.839

> 3) Conocer la variedad de licores consumidos dentro de Iowa.

Hay una variedad de 88 licores consumidos en el estado de Iowa.

> 4) Poder discriminar por condado cuantas tiendas tiene, sus proveedores, cantidad de botellas vendidas y el profit de las mismas.

Esto es posible dada las interacciones entre las visualizaciones dentro de Power BI.


------------


------------

#### Links

[Plan de metricas](https://docs.google.com/spreadsheets/d/1psw-AfYKo22d12-FGllV50YzXXV3PYvgAYOIC864kiI/edit?gid=0#gid=0)
