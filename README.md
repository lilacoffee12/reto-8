# reto-8
´´
## 1
### imprimir numeros del 1 al 100 con su cuadrado 
```
for i in range(1,101): #Teniendo en cuenta que tomna el intervalo abierto
    print(i, i**2)

```
## 2 
### imprimir lista con numeros pares e impares 
```
for i in range(1,1000,2) :
    print(i)
    

for a in range(2,1001,2):
    print(a)


print(i,a)

```
## 3 
### imprimir numeros pares en descendencia hasta 2 
```
n= int(input("Ingrese un numero entero: "))

if n%2==0:
    lista_mk = [i for i in range(2,n+1,2)] 

    lista_mk = sorted(lista_mk, reverse=True)
    for a in lista_mk:
        print(a)
    
else:
    listaa_ = [i for i in range(2,n,2)]
    listaa_ = sorted(listaa_,reverse=True)
    print(listaa_)
```
## 4
### imprimir numeros de 1 hasta un numero n 
```
x = int(input("Ingrese numero: "))

def numero_factorial(n : int ):
  i : int = 1
  factorial : int = 1
  while(i <= n):
    factorial *= i
    i += 1
  return factorial

for n in range(1,x+1):
  print(n, numero_factorial(n) )
```
## 5
### Valor de 2 elevado a potencia usando cilos for 
```
n = int(input("Ingrese un numero entero: "))
for i in range(1,n+1):
    a= 2**i
    print(a)
```
## 6
### leer numero natural y real 
```
x = float(input("Ingrese un numero natural: "))
n = int(input("Ingrese un numero real: "))
import math
a = math.pow(x,n)

for i in range(1,n+1):
    a
    
print(a)
```
## 7
### tablas de multiplicar de 1 a 9
```
m:int=1
for i in range(1,10):
    for m  in range(1,11):
        a= i*m
    
        print(a)
```
## 8
### funcion que calcule una aproximación de una funcion exponencial de 0 para cualquier valor real 
```
x = int(input("Ingrese numero: "))  #Defino la funcion que me da e factorial de un numero

def numero_factorial(x): #En el desarrollo de esta, inicializo 2 variables
  i : int = 1
  factorial : int = 1
  while(i <= x):  #Esto para tener el listado de numeros por los que multiplicaré
    factorial *= i
    i += 1 #De esta manera, le doy continuidad 
  return factorial

a= int(input("Ingrese un numero entero: "))  
n = int(input("Ingrese un numero entero: "))

def aproximacion_exp(a,n): #Funciona bien para valores grandes, entre más pequeños, más aumenta el error
  suma : float =0
  for x in range(0,n+1):
      q = (a**x)/numero_factorial(x)
      suma+= q
  return suma  
print (aproximacion_exp(a,n))  


import math
w = math.exp (a)
print(w)
```
## 9
### Funcion que calcule la aproximacion de la funcion seno alrededor de 0
```
def numero_factorial(x):
  i : int = 1
  factorial : int = 1
  while(i <= x):
    factorial *= i
    i += 1
  return factorial

a = float(input("Ingrese un numero real: "))
n = int(input("Ingrese un numero entero: "))

def funcion_9_punto (a,n): #Funciona bien para valores pequeños, entre más aumenta el valor de a y de n, más aumenta el error
  suma: int = 0
  for x in range(0,n+1):
    q= ((-1)**x)*((a**(2*x+1))/ numero_factorial((2*x)+1)) 
    suma+=q
  return suma

print (funcion_9_punto(a,n))    

import math
w= math.sin(a)
print(w)
```
## 10
### Funcion que calcule una aproximacion de la funcion arcotangente alrededor de 0 
```
x = float(input("Ingrese numero real: "))

def numero_factorial(x): #Se aproxima más entre más pequeño sea el numero 
  i : int = 1
  factorial : int = 1
  while(i <= x):
    factorial *= i
    i += 1
  return factorial

n = int(input("Ingrese un numero entero: "))
a = float(input("Ingrese un numero real: "))
def funcion_arctan(n,a):
    suma: int = 0
    for x in range(0,n+1):
       q=((-1)**x)*(a**(2*x+1))/(2*x+1)
       suma+=q
       return suma
print(funcion_arctan(n,a))   

import math
q= math.atan(a)
print(q)


  

    





    

