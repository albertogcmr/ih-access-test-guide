# Casos de Uso

## Nóminas (listas)

Las nóminas de nuestros empleados están en esta lista de números. 
```python
nominas = [1900, 2000, 1800, 2400, 1700, 1950, 2000, 1806, 2400, 1700]
```
1. ¿Cuánto gasta la empresa en nóminas mensuálmente? ¿Y de forma anual?
2. ¿Cuál es la nómina más alta? ¿y la más baja?
3. ¿Cuál es la media de las nóminas en la empresa?
4. Si las nóminas estuvieran en dólares y las quisiéramos en euros cuál sería la nueva lista de nóminas? **1 EUR = 1.09 DOL**

## Fechas (strings)

```python
fecha = "10/03/2016"
```
1. Obtén el día, mes y año de esta fecha
2. Dada una fecha en formato `dd/mm/yy` calcula el número de días que tiene ese mes. Puedes ignorar si es bisiesto o no. 
3. Ahora pide la fecha al usuario mediante la función `input()` e imprime `día, mes y año` por consola. 

## Netflix (diccionarios)

Como ejemplo: 
```python
item = {"name": "", "year": 0, "genre": ""}
```
Ahora muchas: 
```python
padrino = {"name": "El padrino", "year": 1972, "genre": "Drama"}
lista = {"name": "La lista de Schindler", "year": 1993, "genre": "Drama"}
doce = {"name": "12 hombres sin piedad", "year": 1957, "genre": "Drama"}
vida = {"name": "La vida es bella", "year": 1997, "genre": "Comedy"}
bueno = {"name": "El bueno, el feo y el malo", "year": 1966, "genre": " Western"}
cadena = {"name": "Cadena perpetua", "year": 1994, "genre": "Drama"}
siete = {"name": "Los siete samuráis", "year": 1954, "genre": " Adventure"}

netflix = [padrino, lista, doce, vida, bueno, cadena, siete]
```
1. Dime el año de estreno de "el padrino" y su género. 
2. ¿Cuántas películas hay en nuestra playlist de Netflix?
3. ¿Cuántas películas de `Drama` hay en nuestra playlist de Netflix?
4. ¿Cuántas películas de `Drama` anteriores a `1990` hay en nuestra playlist de Netflix?

