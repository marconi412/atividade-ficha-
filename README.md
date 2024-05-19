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

atvd 11 
#Temperaturas
temperaturas = []
for temp in range(5):
    temperatura = float(input(f"Digite a {temp+1}ª temperatura: "))
    temperaturas.append(temperatura)

maior_temp = max(temperaturas)
menor_temp = min(temperaturas)
media_temp = sum(temperaturas) / len(temperaturas)

print(f"Maior temperatura: {maior_temp}")
print(f"Menor temperatura: {menor_temp}")
print(f"Média das temperaturas: {media_temp}")

atvd 12
# Crédito especial
saldo_medio = float(input("saldo médio do último ano: "))

if saldo_medio <= 200:
    credito = 0
elif 201 <= saldo_medio <= 400:
    credito = saldo_medio * 0.2
elif 401 <= saldo_medio <= 600:
    credito = saldo_medio * 0.3
else:
    credito = saldo_medio * 0.4

print(f"Saldo médio: {saldo_medio}")
print(f"Valor do crédito: {credito}")

atvd 13
from datetime import datetime

# Obtendo informações do usuário
nome = input("Digite seu nome: ")
idade = int(input("Digite sua idade: "))

# Calculando o ano de aposentadoria
ano_atual = datetime.now().year
idade_aposentadoria = 65
ano_aposentadoria = ano_atual + (idade_aposentadoria - idade)

# Criando a mensagem de aposentadoria
mensagem_aposentadoria = f"Olá, {nome}! Com base na sua idade, você poderá se aposentar no ano de {ano_aposentadoria}."

# Exibindo a mensagem
print(mensagem_aposentadoria)

atvd 14 
# Obtendo informações do usuário
valor_hora = float(input("Digite o valor da sua hora de trabalho: "))
horas_trabalhadas = float(input("Digite a quantidade de horas trabalhadas no mês: "))

# Calculando o salário bruto
salario_bruto = valor_hora * horas_trabalhadas

# Calculando o desconto do Imposto de Renda
if salario_bruto <= 2112:
    desconto_ir = 0
elif salario_bruto <= 2826.65:
    desconto_ir = salario_bruto * 0.075
elif salario_bruto <= 3751.05:
    desconto_ir = salario_bruto * 0.15
elif salario_bruto <= 4664.68:
    desconto_ir = salario_bruto * 0.225
else:
    desconto_ir = salario_bruto * 0.275

# Calculando o desconto do Sindicato
desconto_sindicato = salario_bruto * 0.03

# Calculando o FGTS
fgts = salario_bruto * 0.11

# Calculando o salário líquido
salario_liquido = salario_bruto - desconto_ir - desconto_sindicato

# Exibindo os resultados
print(f"Salário Bruto: R$ {salario_bruto:.2f}")
print(f"(-) Desconto do Imposto de Renda: R$ {desconto_ir:.2f}")
print(f"(-) Desconto do Sindicato: R$ {desconto_sindicato:.2f}")
print(f"FGTS (não descontado): R$ {fgts:.2f}")
print(f"Salário Líquido: R$ {salario_liquido:.2f}")
