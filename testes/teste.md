# CÓDIGO DE ELIMINAÇÃO DE NÚMERO REPETIDOS :computer:

numeros = []
numero = int(input())
while numero>= 0:
  numeros.append(numero)
  numero = int(input())
sem_repetidos = list((set(numeros)))
quantidade = []
for i in range(len(sem_repetidos)):
  soma = 0
  for j in range(len(numeros)):
    if sem_repetidos[i] == numeros[j]:
      soma = soma+1
  quantidade.append(soma)
for i in range(len(sem_repetidos)):
  print(sem_repetidos[i],'-',quantidade[i])