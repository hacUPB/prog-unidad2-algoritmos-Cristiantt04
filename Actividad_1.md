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

