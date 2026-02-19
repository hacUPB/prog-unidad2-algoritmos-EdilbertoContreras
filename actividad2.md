# Actividad 2
## 📤 Ejercicio 1.

Investiga cuáles son los símbolos que se utilizan para representar cada operación de un algoritmo con un diagrama de flujo. Asegúrate de que la fuente es confiable, discute lo que encontraste con tus compañeros y con el profe. Cuando estés seguro/a de tener los símbolos correctos, consigna la información en la bitácora.

![Imagen random](https://cdn.processon.io/admin/knowledge/article_content_img/67455ff187ba486a4c41157c.png)

## Ejercicio 2.

    Construye un algoritmo que, al recibir como datos el ID del empleado y los seis primeros sueldos del año, calcule el ingreso total semestral y el promedio mensual, e imprima el ID del empleado, el ingreso total y el promedio mensual.

    Inicio del algoritmo

        Algoritmo Sueldo Semestral

        Definir ID como entero
        Definir s1, s2, s3, s4, s5, s6 como real
        Definir total, promedio como real

        Escribir "Ingrese ID del empleado:"
        Leer ID

        Escribir "Ingrese los 6 sueldos del año:"
        Leer s1, s2, s3, s4, s5, s6

        total ← s1 + s2 + s3 + s4 + s5 + s6
        promedio = total / 6

        Escribir "ID del empleado: ", ID
        Escribir "Ingreso total semestral: ", total
        Escribir "Promedio mensual: ", promedio

    Fin del algoritmo

## Ejercicios 3. Un **acuario** necesita determinar cuántos litros o
    
    1. Un acuario necesita determinar cuántos litros o galones (eso lo decide el usuario) de agua caben en un acuario, pero solo dispone de una cinta métrica (en centímetros). Diseña un algoritmo para solucionar el problema. 

        Algoritmo Acuario

    Definir largo, ancho, alto, volumen, litros, galones
    Definir opcion Como Entero

    Escribir "Ingrese largo, ancho y alto en cm:"
    Leer largo, ancho, alto

    volumen = largo * ancho * alto

    Escribir "Litros"
    Escribir "Galones"
    Leer opcion

    Si opcion = Litros Entonces
        litros = volumen / 1000
        Escribir "Capacidad en litros: " litros
    Sino
        galones = volumen / 3785
        Escribir "Capacidad en galones: " galones
    Fin Si

FinAlgoritmo

![imagen](imagenes/acuario.drawio.png)
## ejercico 4. cuanto pagar por x cantidad 

    2. Realice un algoritmo para determinar cuánto se debe pagar por equis cantidad de lápices considerando que si son 1000 o más el costo es de $85 cada uno; de lo contrario, el precio es de $90. Represéntelo con el pseudocódigo y el diagrama de flujo.
        
|variable| inicio  | fin |
|--------|----|---|
|cantidad|  0 | N.lapices  |
|presio  |  0 | valor  |
| total  |  0 | total a pagar  |

        Algoritmo PagoLapices

        Definir cantidad, precio, total

        Escribir "Ingrese la cantidad de lapices:"
        Leer cantidad

        Si cantidad >= 1000 Entonces
            precio = 85
        Sino
            precio = 90
        FinSi

        total = cantidad * precio

        Escribir "Precio por lapiz:" precio
        Escribir "Total a pagar:" total

        FinAlgoritmo


![imagen](imagenes/lapices.drawio.png)

    3. Un almacén de ropa tiene una promoción: por compras superiores a $250 000 se les aplicará un descuento de 15%, de caso contrario, sólo se aplicará un 8% de descuento. Realice un algoritmo para determinar el precio final que debe pagar una persona por comprar en dicho almacén y de cuánto es el descuento que obtendrá. Represéntelo mediante el pseudocódigo y el diagrama de flujo.

|compra|compra > 250k|descuento|valor del descuento|presioT|
|---|---|---|---|---|
|200k| no  | 8%  | 16k  | 184k  |
|250k|  no | 8%  |  20k | 230k  |
|300k| si  | 15%  | 45k  | 255k  |

        Algoritmo DescuentoAlmacen

        Definir compra, descuento, precioFinal Como Real

        Escribir "Ingrese el valor de la compra"
        Leer compra

        Si compra > 250000 Entonces
            descuento = compra * 0.15
        Sino
            descuento = compra * 0.08
        FinSi

        precioFinal = compra - descuento

        Escribir "Descuento obtenido:" descuento
        Escribir "Precio final a pagar:" precioFinal

        FinAlgoritmo
![imagen](imagenes/descuento.drawio.png)

    4. El director de una escuela está organizando un viaje de estudios, y requiere determinar cuánto debe cobrar a cada alumno y cuánto debe pagar a la compañía de viajes por el servicio. La forma de cobrar es la siguiente: si son 100 alumnos o más, el costo por cada alumno es de $65.00; de 50 a 99 alumnos, el costo es de $70.00, de 30 a 49, de $95.00, y si son menos de 30, el costo de la renta del autobús es de $4000.00, sin importar el número de alumnos.
