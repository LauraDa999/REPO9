# REPO9
#  1. De los retos anteriores selecciona 3 funciones y escribelas en forma de lambdas.
a. Diseñe una función que calcule la cantidad de carne de aves en kilos si se tienen N gallinas, M gallos y K pollitos cada uno pesando 6 kilos, 7 kilos y 1 kilo respectivamente en LAMBDA
```
calcular_cantidad_carne = lambda N, M, K: (N * 6) + (M * 7) + (K * 1)

# Ejemplo de uso de la función lambda
N = 10  # Número de gallinas
M = 5   # Número de gallos
K = 20  # Número de pollitos

total_carne = calcular_cantidad_carne(N, M, K)
print(f"La cantidad total de carne de aves es {total_carne} kilos.")
```
b. Funcion para elevar al cuadrado, en LAMBDA:
```
elevar_cuadrado_lambda = lambda x: x**2
```

c. Funcion para para sumar dos números en LAMBDA:
```
sumar_dos_numeros_lambda = lambda x, y: x + y
```
# 2. De los retos anteriores selecione 3 funciones y escribalas con argumentos no definidos (*args)
a. Imprimir un listado con los números del 1 al 100 cada uno con su respectivo cuadrado cCON ARGS:
```
def calcular_cuadrados(*args):
    for numero in args:
        cuadrado = numero ** 2
        print(f"Número: {numero}, Cuadrado: {cuadrado}")

# Llamar a la función con los números del 1 al 100
numeros = range(1, 101)
calcular_cuadrados(*numeros)
def calcular_cuadrados(*args):
    for numero in args:
        cuadrado = numero ** 2
        print(f"Número: {numero}, Cuadrado: {cuadrado}")

# Llamar a la función con los números del 1 al 100
numeros = range(1, 101)
calcular_cuadrados(*numeros)
```
b. Imprima un listado con los números iguales desde 1 hasta 999 y seguidamente otro listado con los números pares desde 2 hasta 1000, CON ARGS:
```
def imprimir_numeros(*args):
    for rango in args:
        print(f"Números {rango} desde {rango[0]} hasta {rango[1]}:")
        for numero in range(rango[0], rango[1] + 1, 2 if rango[0] % 2 == 0 else 1):
            print(numero)

# Para números impares
imprimir_numeros((1, 999))

# Para números pares
imprimir_numeros((2, 1000))

```
c. Imprimir el factorial de un número natural n dado CON ARGS:
```
def calcular_factorial(*args):
    for n in args:
        if n < 0:
            print(f"El factorial no está definido para números negativos ({n}).")
        elif n == 0:
            print(f"El factorial de 0 es 1.")
        else:
            factorial = 1
            for i in range(1, n + 1):
                factorial *= i
            print(f"El factorial de {n} es {factorial}.")

# Solicita los números naturales y calcula sus factoriales
numeros = [int(x) for x in input("Ingrese números naturales separados por espacios: ").split()]
calcular_factorial(*numeros)
```
#  Punto 3. Escriba una función recursiva para calcular la operación de la potencia
La función potenciatoma tiene dos argumentos, basey exponente.
Si el exponente es negativo y Si el exponente es positivo, la recursión continúa hasta que el exponente alcanza 0, momento en el cual se aplican los casos.
```
def potencia(base, exponente):
    if exponente == 0:
        return 1
    elif exponente < 0:
        return 1 / (base * potencia(base, -exponente - 1))
    else:
        return base * potencia(base, exponente - 1)
```

# Punto #4. 
Utilice la siguiente plantilla de code para contar el tiempo:
Se calcula la serie de Fibonacci de forma recursiva y mide el tiempo de ejecución de ese cálculo. Aquí está una explicación
```
import time
bandera = True
a : int = 1
while bandera == True:
  start_time = time.time()
  def fiboRecursivo(n : int )-> int:
    if n <=1:
      # caso base
      return 1
    else:
      # condicion
      return fiboRecursivo(n-1)+fiboRecursivo(n-2)  

  if __name__ == "__main__":
    num = a
    serieFibo = fiboRecursivo(num)
    end_time = time.time()
    timer = end_time - start_time

  if timer > 10.0:
    break
  else:
    a=a+1 
    #print("La serie de Fibonacci hasta " + str(num) + " es " + str(serieFibo))  
    #print("Su tiempo de ejecución fue de +str(timer)) Estos dos por si quires analizar cada tiempo
print("La serie de Fibonacci hasta " + str(num) + " es " + str(serieFibo))
print("A partir de aqui considerar tiempo considerable")
print("Su tiempo de ejecución fue de : " +str(timer))

```

# 5. Crear cuenta en stackoverflow y adjuntar imagen en el repo:

https://www.linkedin.com/in/laura-garcia-17056a232
![Imagen de WhatsApp 2023-10-16 a las 22 36 49_7d1b101e](https://github.com/LauraDa999/REPO9/assets/141860731/74ec70ef-57cd-4e34-b07d-fa760aa3ac33)


#  6. link de linkedin:
https://www.linkedin.com/in/laura-garcia-17056a232/


