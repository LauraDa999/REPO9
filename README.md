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
