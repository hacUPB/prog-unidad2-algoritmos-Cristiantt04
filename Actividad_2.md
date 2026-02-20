# Representación de algoritmos
![](Images/Imagen6.png)

Existen dos tipos principales:

1. **Cualitativos**: Describen pasos a través de palabras. Por ejemplo, las instrucciones para preparar una receta de cocina, como "mezclar los ingredientes" u "hornear durante 30 minutos", constituyen un algoritmo cualitativo.
2. **Cuantitativos**: Incluyen cálculos numéricos. Por ejemplo, un algoritmo para calcular el volumen de una caja: `Volumen = Largo * Ancho * Alto`.

# Ejercicio 1 
![Simbolos](Images/Imagen7.png)

# Ejercicio 2 
- Construye un algoritmo que, al recibir como datos el ID del empleado y los seis primeros sueldos del año, calcule el ingreso total semestral y el promedio mensual, e imprima el ID del empleado, el ingreso total y el promedio mensual.

#### Datos de entrada. 
|Nombre|Descripción| 
|---|---|
|Id|Número de identificación del empleado(Númerico)|
|S1,S2,S3,S4,S5,S6|Los sueldos de los seis meses| 

#### Datos intermedios.
    En este caso no los habrian ya que se puede pasar de los datos iniciales a los finales con un proceso sencillo, pero viendolo desde otro modo, los datos intermedios y los finales podrian coincidir en este caso. 

#### Datos de salida.
|Nombre|Descripción|
|---|---|
|$I_T$|Ingerso total en los seis meses|
|P|Promedio de ingresos mensual|

### Pseudocódigo
Inicio   
Leer Id, S1, S2, S3, S4, S5, S6     
$I_T$ = S1 + S2 + S3 + S4 + S5 + S6       
P = $I_T$ / 6             
Mostrar Id, $I_T$, P          
Fin  

### Diagrama de flujo. 

![](Diagramas/Diagrama1.png)


# Ejercicios 3.


#### 1. Un acuario necesita determinar cuántos litros o galones (eso lo decide el usuario) de agua caben en un acuario, pero solo dispone de una cinta métrica (en centímetros). Diseña un algoritmo para solucionar el problema. 

#### Datos de entrada. 

|Datos|Descripción|
|---|---|  
|Largo|Largo del tanque en cm|
|Ancho|Ancho del tanque en cm|
|Alto|Alto del tanque en cm|
|Unidad|Litros o galones| 

#### Datos Intermedios.
|Dato|Descripción|
|---|---|
|$Volumen_{cm^3}$|La multiplicación de Largo, Ancho,Alto|

#### Datos de salida. 
|Datos|Descripción|
|---|---|
|$Volumen_L$|Volumen en litros|
|$Volumen_{gal}$|Volumen en galones|

### Pseudocódigo
 
Inicio    
Mostrar "Ingresa las medidas del tanque en cm"    
Leer Largo Ancho Alto    
Mostrar  "Selecciona Litros o Galones"      
Leer Unidad
$Volumen_{cm^3}$ = Largo * Ancho * Alto    

Si Unidad = Litros  

     Volumen_L = Volumen_cm^3 /1000
     Mostrar Volumen_L

Si no

    Volumen_gal = Volumen_cm^3 / 3785.45
    Mostrar Volumen_gal

Fin si   

Fin   

### Diagrama de flujo. 
![](Diagramas/Diagrama2.png)


2. Realice un algoritmo para determinar cuánto se debe pagar por equis cantidad de lápices considerando que si son 1000 o más el costo es de $85 cada uno; de lo contrario, el precio es de $90. Represéntelo con el pseudocódigo y el diagrama de flujo.

#### Dato de entrada. 
|Dato|Descripción|
|---|---|
|Lapices||Cantiad de lapices|

#### Dato intermedios.
|Dato|Descripcón|
|---|---|
|Precio|Precio de los lapices|

#### Dato de salida.
|Dato|Descripción|
|---|---|
|$Precio_T$|Precio de todos los lapices|

### Pseudocódigo

Inicio     
Leer Lapices

Si lapices < 1000   

    Precio = 90 


Si no    

    Precio = 85 

Fin si    
$Precio_T$ = Lapices * Precio     
Mostrar $Precio_T$   
Fin 

### Diagrama de flujo.
![](Diagramas/Diagrama3.png)


3. Un almacén de ropa tiene una promoción: por compras superiores a $250 000 se les aplicará un descuento de 15%, de caso contrario, sólo se aplicará un 8% de descuento. Realice un algoritmo para determinar el precio final que debe pagar una persona por comprar en dicho almacén y de cuánto es el descuento que obtendrá. Represéntelo mediante el pseudocódigo y el diagrama de flujo.

#### Datos de entrada. 
|Datos|Descripción|
|---|---|
|V_compra|Valor de la compra|

#### Datos intermedios. 

    En este caso no hay Datos intermedios 

#### Datos de salida. 
|Datos|Descripción|
|---|---|
|Precio_T|Precio total de la compra| 
|Descuento|Descuento aplicado a la compra| 

### Pseudocodigo.
Inicio 
Leer V_compra 

Si  V_compra > $250 000 

    Descuento = 0.15
    Precio_T = V_compra - (V_compra * 0.15)

Si no 

    Descuento = 0.08
    Precio_T = V_compra - (V_compra * 0.08)

Fin si 

Mostrar Precio_T Descuento 

Fin

### Diagrama de flujo. 

![](Diagramas/Diagrama4.png)

4. El director de una escuela está organizando un viaje de estudios, y requiere determinar cuánto debe cobrar a cada alumno y cuánto debe pagar a la compañía de viajes por el servicio. La forma de cobrar es la siguiente: si son 100 alumnos o más, el costo por cada alumno es de $65.00; de 50 a 99 alumnos, el costo es de $70.00, de 30 a 49, de $95.00, y si son menos de 30, el costo de la renta del autobús es de $4000.00, sin importar el número de alumnos.

