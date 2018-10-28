# Introducción

Antes de comenzar a introducir los conceptos de análisi de imágenes, es buena idea dar un pequeño *tour* sobre el lenguaje de programación **Python**

**Python** es un lenguaje de programación interpretado y fuertemente tipado, lo que significa que nuestros programas serán procesados línea por línea mediante un intérprete, el cual realizará todas las operaciones y tareas solicitadas en tiempo real. *Fuertemente tipado* significa que no es necesario establecer el tipo de dato de una variable ya que lo interpreta de manera automática.

### Hola mundo

```python
print "Hola mundo"
```
La función de este código solamente es mostrarnos un texto en la terminal, el cual es *Hola mundo*

### Variables, operaciones y estructuras de control soportadas por Python

* __Variable:__ Una variable es aquella que nos permite almacenar datos en la memoria temporal, de tal forma que podamos utilizarlos después para realizar operaciones. Las variables se caracterizan por no llevar espacio y tener un formato muy parecido a este:

	* `miVariable`
	* `variable`
	* `mi_Variable`

Entre otros estilos

* **Operaciones:** Son las operaciones aritméticas que se pueden realizar, dichas operaciones con su signo correspondiente son las siguientes.
	
	* `Suma: + (en cadenas de texto funciona como concatenación)` 
	* `Resta: -`
	* `Multiplicación: *`
	* `División: /`
	* `Resta: -`
	* `Asignación: =`
	* `Mayor que/Mayor o igual que: > / >=`
	* `Menor que/Menor o igual que: < / <=`
	* `Igual que: ==`
	* `Desigual que: !=`
	* `O: or`
	* `Y: and`
	* `No: not`
	* `O a nv de bits: |`
	* `Y a nv de bits: &`
	* `No a nv de bits: ~`
	* `Corrimiento de bits: <</>>`

	**Ejemplo:**

	```python
	a = 5  #Este es un claro ejemplo de asignación
	b = 8

	print "Suma: ", a + b 				#La pantlla nos muestra el resultado, el cual es 13
	print "Resta: ", a - b 				#La pantlla nos muestra el resultado, el cual es -3
	print "Multiplicación: ", a * b 	#La pantlla nos muestra el resultado, el cual es 40
	print "División: ", a / b 			#La pantlla nos muestra el resultado, el cual es 0.625
	```
* **Estructuras de control:** También llamadas estructuras de control de flujo, son aquellas que nos permiten establecer reglas para la ejecución del código dependiendo de una condicion dada se cumpla o no, incluso si el código se deba de repetir cierto número de veces o de manera indeterminada, dichas estructuras son.

	* `if-else: Condicional if`
	* `for: Ciclo`
	* `while: Ciclo`

**Ejemplo**

```python
a = 10
b = 7

if a > b:
	print "a es mayor que b"
else:
	print "a no es mayor que b"

#La estructura de control if se compone de la siguiente sintaxis

if <variable|valor> <Operador de comparación, puede ser <, >, <=, etc> <variable|valor>
	<Bloque|Acción a realizar al cumplir la condición>
else<En caso contrario>
	<Bloque|Acción a realizar al no cumplir la condición>

for i in range(0, 11, 2):
	print i

#Este código ejemplifica el ciclo for, el cual imprime los números pares del 1 al 10, funciona con la siguiente sintaxis

for <variable> in range(<inicio>, <final>, <paso>), donde paso es el salto que realizará entre los números por iteración

while(a == 10):
	a = a + 1
#Este código ejemplifica el ciclo while, el cual incrementa la variable a hasta que llegue al número 10, funciona muy parecido al if

```

### Funciones, módulos, colecciones e hilos

* **Funciones:** Una funcíón es un bloque de código que realiza una tarea el cual regresa un valor mediante parámetros dados, aunque estas dos condiciones no son obligatorias, una función se define de la siguiente manera

```python
def <nombre de la funcion>(<parámetro1 = valor por default>, <parámetro2 = valor por default>, ..., <parámetroN>):
	<bloque>

	return <valor a regresar>
```

Ejemplo: Definamos una función que realice una suma de la siguiente manera
```python
def sumar(a, b):
	return a + b

print sumar(5, 7) #Imprime el valor 12
```