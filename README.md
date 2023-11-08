def insertionSort(vetor):
    for i in range(1, len(vetor)):
        chave = vetor[i]
        j = i - 1
        while j >= 0 and vetor[j] > chave:
            vetor[j + 1] = vetor[j]
            j = j - 1
        vetor[j + 1] = chave

# Tamanho do vetor
tamanho = 30

# Criar vetor com números ímpares
vetor = [2 * i + 1 for i in range(tamanho)]

# Desordenar o vetor
import random
random.shuffle(vetor)

# Aplicar o insertion sort
insertionSort(vetor)

# Exibir o vetor ordenado
print("Vetor ordenado:", vetor)# cd-9
