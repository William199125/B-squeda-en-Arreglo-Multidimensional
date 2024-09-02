# B-squeda-en-Arreglo-Multidimensional
Búsqueda en Arreglo Multidimensional
def bubble_sort(fila):
    n = len(fila)
    for i in range(n):
        for j in range(0, n-i-1):
            if fila[j] > fila[j+1]:
                fila[j], fila[j+1] = fila[j+1], fila[j]

def ordenar_fila(matriz, fila_a_ordenar):
    # Mostramos la matriz original
    print("Matriz original:")
    for fila in matriz:
        print(fila)

    # Ordenamos la fila específica utilizando bubble sort
    bubble_sort(matriz[fila_a_ordenar])

    # Mostramos la matriz con la fila ordenada
    print("\nMatriz con la fila", fila_a_ordenar, "ordenada:")
    for fila in matriz:
        print(fila)

# Definimos una matriz 3x3 con valores numéricos
matriz = [
    [9, 8, 7],
    [3, 2, 1],
    [6, 5, 4]
]

# Fila que queremos ordenar (índice empieza en 0)
fila_a_ordenar = 1

# Llamamos a la función para ordenar la fila específica
ordenar_fila(matriz, fila_a_ordenar)
