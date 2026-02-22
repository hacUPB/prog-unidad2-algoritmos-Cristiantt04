![](Images/Imagen%201.png)

# Ejercicio 1.1
¿Cuántos estados diferentes se pueden representar usando N bits?

#### R// 
- 1 bit → $2^1$ = 2 estados
- 2 bits → $2^2$ = 4 estados
- 3 bits → $2^3$ = 8 estados
- n bits → $2^n$ estados 


# Ejercicio 1.2 (Conversiones)

1. Convierte el número decimal 22 a binario.
2. ¿Cuál es el resultado en decimal del número binario 10110?

#### Solución 
    1. Decimal: 22
       Binario: 10110

     22 ÷ 2 = 11, residuo 0
     11 ÷ 2 = 5, residuo 1
     5 ÷ 2 = 2, residuo 1
     2 ÷ 2 = 1, residuo 0 
     1 ÷ 2 = 0, residuo 1

     [Residuos de abajo hacia arriba]

2.
 |1|0|1|1|0| 
 |---|---|---|---|---|
 |$2^4$|$2^3$|$2^2$|$2^1$|$2^0$|
 |16|8|4|2|1|

16 + 4 + 2 = 22 

$10110_{2}$ = $22_{10}$


# Tabla ASCII
![](Images/Imagen%203.jpg)
# Ejercicio 1.3
1. ¿Qué número binario representa el carácter 'C' en ASCII?

##### R// C = $67_{10}$ = $110001_2$

# Bits 
+----+----+----+----+----+----+----+-------+                 
| bite | bite | bite | bite | bite | bite |bite | bite |   
+-----------------------byte--------------------+

Un bit (binary digit) es la unidad más pequeña de información en una computadora. Solo puede tener dos valores: 0 o 1. Todo lo que hace un sistema digital (texto, imágenes, números, programas) se representa internamente usando combinaciones de bits.

Un byte está compuesto por 8 bits. Con 8 bits se pueden formar $2^8$ = 256 combinaciones distintas, lo que permite representar valores del 0 al 255. Por eso un byte es suficiente para almacenar, por ejemplo, un carácter en codificaciones básicas como ASCII.

Cuando se necesitan números más grandes o más información, simplemente se usan más bytes. Más bits implican más combinaciones posibles.

#### 🗃️ Unidades de almacenamiento
- 1 Byte (B) = 8 bits
- 1 Kilobyte (KB) = 1024 bytes
- 1 Megabyte (MB) = 1024 KB
- 1 Gigabyte (GB) = 1024 MB
- 1 Terabyte (TB) = 1024 GB

# Ejercicio 1.4

1. ¿Cuántos bytes se necesitan para almacenar la palabra “Hola” en ASCII?

2. ¿Cuántos bits hay en 5 KB?


#### Solución

1. Se necesitan 4 bytes para almacenar “Hola” en ASCII. Ya que cada caracter necesita un byte (8 bits).

2. En 5 KB hay 40 960 bits.    
5 * 1024 * 8 = 40 960 bits.



# Sistema Hexadecimal

El sistema hexadecimal es un sistema de numeración en base 16. Utiliza los siguientes símbolos:

0, 1, 2, 3, 4, 5, 6, 7, 8, 9, A, B, C, D, E, F

El sistema hexadecimal se utiliza ampliamente en informática porque permite representar números binarios de forma más compacta y legible.

Relación con el sistema binario

Cada dígito hexadecimal equivale exactamente a 4 bits (un nibble), ya que:

$2^4$ = 16

Esto significa que:

1 dígito hexadecimal = 4 bits

2 dígitos hexadecimales = 1 byte (8 bits)
#### Errores de Redondeo y Precisión
En los sistemas informáticos, los números decimales se almacenan generalmente utilizando el estándar de punto flotante (IEEE 754).

El problema surge porque no todos los números decimales pueden representarse exactamente en binario. Por ejemplo, valores como:
- 0.1
- 0.2

Producen representaciones binarias infinitas periódicas.

Debido a esto, el sistema debe truncar o redondear la representación, lo que genera pequeñas imprecisiones. Estas diferencias pueden acumularse en cálculos repetitivos o financieros si no se manejan correctamente.

![](Images/Imagen%204.png)

## Ejercicio 1.4

1. Convierte el número decimal 255 a hexadecimal.
2. ¿Cuál es el valor hexadecimal de la secuencia binaria 11010110?

#### Solución 
1.  $255_{10}$ = $FF_{16}$

2.
  |1|1|0|1|0|1|1|0| 
 |---|---|---|---|---|---|---|---|
 |$2^7$|$2^6$|$2^5$|$2^4$|$2^3$|$2^2$|$2^1$|$2^0$|
 |128|64|32|16|8|4|2|1|

 128 + 64 + 16 + 4 + 2 = $214_{10}$ = $D6_{16}$

 # Ejercicios Finales de Repaso


1. Explica, en tus propias palabras, por qué es necesario que las computadoras representen los datos en binario.
2. Convierte el número binario 10011011 a decimal y a hexadecimal.
3. Investiga y describe cómo se representa una imagen en formato PNG en el disco.
4. Analiza la siguiente situación: ¿Qué sucede si intentas almacenar un número mayor al que puede representar un byte (por ejemplo, 300)? ¿Cómo lo maneja Python?

#### Soluciones
1. Porque el hardware de los aparatos electronicos funciona mediante dos estados baasico, alto voltaje y bajo voltaje, los transistores los cuales son las bases de los circuitos electronicos solo pueden estar apagados o encendidos, por lo cual representar los datos en un sistema de dos posibilidades de entrada y salida es lo mas ideal. 

2. 
  |1|0|0|1|1|0|1|1| 
 |---|---|---|---|---|---|---|---|
 |$2^7$|$2^6$|$2^5$|$2^4$|$2^3$|$2^2$|$2^1$|$2^0$|
 |128|64|32|16|8|4|2|1|

 128 + 16 + 8 + 2 + 1 = $115_{10}$ 


$115_{10}$ = $9B_{16}$
![](Images/Imagen%205.jpeg)

3. Una imagen PNG no se guarda como “una foto” sino como un archivo binario estructurado. Empieza con una firma que identifica el formato y después se organiza en bloques llamados chunks. Hay un bloque principal que define el ancho, alto y tipo de color, otros que contienen los datos reales de los píxeles comprimidos (usando un método sin pérdida llamado DEFLATE) y uno final que marca el cierre del archivo. Los píxeles normalmente se almacenan como combinaciones de RGB o RGBA, y antes de guardarse se aplican filtros para mejorar la compresión. Todo está diseñado para que la imagen ocupe menos espacio sin perder calidad.

4. Un byte solo puede representar 256 valores distintos, es decir, números del 0 al 255 si es sin signo. Si intentas guardar 300 en un solo byte en un lenguaje como C o Java, ocurre un desbordamiento: el número “se envuelve” y solo se conservan los 8 bits menos significativos, lo que cambia el valor almacenado. En cambio, Python no tiene este problema porque sus enteros no tienen un tamaño fijo de 8 o 32 bits. Python usa enteros de tamaño dinámico, así que puede representar 300 (o números muchísimo más grandes) sin overflow, limitado únicamente por la memoria disponible.