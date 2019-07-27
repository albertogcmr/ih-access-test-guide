# Manual de la prueba de acceso para el Bootcamp de Data Analytics de Ironhack


## Propósito de este documento

Con este documento pretendemos darte una ayuda para que pases la prueba técnica de acceso al bootcamp de Ironhack en análisis de datos y sepas a lo que te vas a enfrentar. Consistirá principalmente en resolver un problema básico de programación en Python. Los conceptos estadísticos necesarios serán mínimos.

Contiene tres secciones: 
* **Programación online**: para que practiques los ejemplos. 
* **Conocimientos de Python**: para que sepas los conocimientos mínimos con ejemplos. 
* **Ejemplo de prueba de acceso**: para que veas qué puedes encontrarte. 


## Programación online

Para que puedas programar sin tener que instalarte ningún software, hazte una cuenta en la siguiente plataforma. Podrás practicar todo lo que quieras en muchos lenguajes de programación además de Python. Intenta probar a programar todo lo que se muestra en ete documento. 

https://repl.it/repls

## Conocimientos de Python

Para pasar la prueba deberás tener unos conocimientos mínimos


```python
# 1º crear una lista del 1 al 10​

lst=[1,2,3,4,5,6,7,8,9,10]      # version newbie
print (lst)

​lst=[i for i in range(1, 11)]   # version pro
print (lst)

# 2º crear una nueva lista desde la primera de los numeros pares o impares
# pares 

lst2=[]

for e in lst:                   # version newbie

	if e%2==0: lst2.append(e)

print (lst2)


lst2=[e for e in lst if e%2==0] # version pro

print (lst2)

​

# impares

lst2=[]

for e in lst:                  # version newbie

	if e%2==1: lst2.append(e)

print (lst2)

​

​

lst2=[e for e in lst if e%2==1] # version pro

print (lst2)

​

​

# 3º cambiar pares/impares por 0-1

​

# pares==0, impares==1

​

lst3=[]

for e in lst:                   # version newbie

	if e%2==0: lst3.append(0)

	else: lst3.append(1)

print (lst3)

​

​

lst3=[0 if e%2==0 else 1 for e in lst]  # version pro

print (lst3)

​

​

# pares==1, impares==0

​

lst3=[]

for e in lst:                     # version newbie

	if e%2==0: lst3.append(1)

	else: lst3.append(0)

print (lst3)

​

​

lst3=[1 if e%2==0 else 0 for e in lst]  # version pro

print (lst3)

​

​

​

​

# 4º sumar todos los elementos de la primera lista (dos versiones)

​

suma=0           # version 1

for e in lst:

	suma+=e

print (suma)

​

​

suma=sum(lst)    # version 2

print (suma)



```

## Ejemplo de prueba de acceso

A continuación hay una muestra de la antígua prueba de nivel. Ya no se pide esto pero te puede dar una idea de lo que se te preguntará. Recomendamos que intentes resolver este problema antes de presentarte a la prueba. 

Dada una lista de números enteros: 
1. Muestra por pantalla los números de esta lista que son mayores que 5.

```python
numeros = [1, 7, 6, 5, 4, 3, 2, 3, 4, 5, 6, 7, 6, 5, 4, 3, 2, 3, 4, 5, 6, 7]

for numero in numeros: 
	if numero > 5: 
		print(numero)
```

Obtendremos a la salida lo siguiente: 

```python
7 
6 
6 
7 
6 
6 
7
```

2. Indica cuántos números de la lista son mayores que 5.

```python
numeros = [1, 7, 6, 5, 4, 3, 2, 3, 4, 5, 6, 7, 6, 5, 4, 3, 2, 3, 4, 5, 6, 7]

mayores = 0
for numero in numeros: 
	if numero > 5: 
		mayores = mayores + 1

print(mayores)
```

Obtendremos a la salida lo siguiente: 

```python
7
```

3. Muestra por pantalla una nueva lista que traduzca los elementos de la lista original:
	* Los menores o iguales que 5 serán 0,
	* Los mayores que 5 serán 1.
```python
numeros = [1, 7, 6, 5, 4, 3, 2, 3, 4, 5, 6, 7, 6, 5, 4, 3, 2, 3, 4, 5, 6, 7]
solucion = []

for numero in numeros: 
	if numero > 5: 
		solucion.append(1)
	else: 
		solucion.append(0)

print(solucion)
```

Obtendremos a la salida lo siguiente: 

```python
[0, 1, 1, 0, 0, 0, 0, 0, 0, 0, 1, 1, 1, 0, 0, 0, 0, 0, 0, 0, 1, 1]
```
