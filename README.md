TAREFA 1
lista = [x for x in range(300)]
x = input("Digite um numero:")
if x < 300:
    print x,"numero desejado"
if x > 300:
    print x,"Fora dos padroes"
	
	

TAREFA 2
import random
lista1 = [random.randint(0,5000000) for x in range(500)]
print (lista1)

lista2 = [random.randint(0,5000000) for x in range(5000)]
print (lista2)

lista3 = [i for i, j in zip(lista1,lista2) if i == j]
print (lista3)


TAREFA 3
x = int(input("Digite um numero:"))
numero = 2
c = 1
p = 0
while numero < x:
    i = numero - 1
    while i > 1:
            if numero % i ==0 : break
            i -= 1
            c += 1
    else:
        print numero,
        p += 1
        numero += 1

print "\n\nForam encontrados %d números primos." %p
