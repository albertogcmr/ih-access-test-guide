


```python
# 1º crear una lista del 1 al 10

​

lst=[1,2,3,4,5,6,7,8,9,10]      # version newbie

print (lst)

​

lst=[i for i in range(1, 11)]   # version pro

print (lst)

# 2º crear una nueva lista desde la primera de los numeros pares o impares

​

# pares 

lst2=[]

for e in lst:                   # version newbie

	if e%2==0: lst2.append(e)

print (lst2)

​

​

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

​```