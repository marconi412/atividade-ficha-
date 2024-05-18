atvd 1
# Ver se a letra é vogal ou consoante
letra = input("Digite uma letra: ").lower()
if letra in 'aeiou'or 'AEIOU':
    print("A letra {letra} é uma vogal.")
else:
    print("A letra {letra} é uma consoante.")

atvd 2
# Encontrar o produto mais barato
valor1 = float(input("Digite o preço do primeiro produto: "))
valor2 = float(input("Digite o preço do segundo produto: "))
valor3 = float(input("Digite o preço do terceiro produto: "))

atvd3
if valor1 < valor2 and valor1 < valor3:
    print("o primeiro produto é o mais barato.")
elif valor2 < valor1 and valor2 < valor3:
    print("o segundo produto é o mais barato")
else:
    print("o terceiro produto é o mais barato.")

atvd 4
# Turno de estudo
turno = input("turno (M-matutino, V-Vespertino, N-Noturno): ").upper()
if turno == 'M':
    print("Bom Dia!")
elif turno == 'V':
    print("Boa Tarde!")
elif turno == 'N':
    print("Boa Noite!")
else:

    print("Valor Inválido!")

atvd 5
# Dia da semana
dia = int(input("Dia da semana de acordo com um numero (1-7): "))
dias = {
    1: "Domingo",
    2: "Segunda-feira",
    3: "Terça-feira",
    4: "Quarta-feira",
    5: "Quinta-feira",
    6: "Sexta-feira",
    7: "sabado", 
}
else:
     print("Valor inválido!")

atvd 6
# Média e conceito de notas
nota1 = float(input("Digite a primeira nota: "))
nota2 = float(input("Digite a segunda nota: "))

media = (nota1 + nota2) / 2

if 9 <= media <= 10:
    conceito = 'A'
elif 7.5 <= media < 9:
    conceito = 'B'
elif 6 <= media < 7.5:
    conceito = 'C'
elif 4 <= media < 6:
    conceito = 'D'
else:
    conceito = 'E'

print(f"Notas: {nota1}, {nota2}")
print(f"Média: {media}")
print(f"Conceito: {conceito}")
if conceito in 'ABC':
    print("APROVADO")
else:
    print("REPROVADO")

atvd 7
# Ano bissexto
ano = int(input("Digite um ano: "))

if (ano % 4 == 0 and ano % 100 != 0) or (ano % 400 == 0):
    print(f"O ano {ano} é bissexto.")
else:
    print(f"O ano {ano} não é bissexto.")

atvd 8
# Verificar idade
idade = int(input("Digite a sua idade: "))
if 0 <= idade <= 150:
    print(f"Sua idade é {idade}")
else:
    print("Valor inválido!")

atvd 9
# Soma e média de 5 números
numeros = []
for i in range(5):
    numero = float(input(f"Digite o {i+1}º número: "))
    numeros.append(numero)

soma = sum(numeros)
media = soma / 5

print(f"Soma: {soma}")
print(f"Média: {media}")

atvd 10
# Verificar se um número é primo
numero = int(input("Digite um número inteiro: "))
if numero > 1:
    for i in range(2, numero):
        if numero % i == 0:
            print(f"O número {numero} não é primo.")
            break
    else:
        print(f"O número {numero} é primo.")
else:
    print(f"O número {numero} não é primo.")
