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

if valor1 < valor2 and valor1 < valor3:
    print("o primeiro produto é o mais barato.")
elif valor2 < valor1 and valor2 < valor3:
    print("o segundo produto é o mais barato")
else:
    print("o terceiro produto é o mais barato.")
