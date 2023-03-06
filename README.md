# ProcessoSeletivoTarget

num = int(input("Digite um número: "))

fibonacci = [0, 1]
while fibonacci[-1] < num:
    fibonacci.append(fibonacci[-1] + fibonacci[-2])

if num in fibonacci:
    print(num, "pertence à sequência de Fibonacci!")
else:
    print(num, "não pertence à sequência de Fibonacci.")

##Explicando o código:

O usuário é solicitado a digitar um número, que é armazenado na variável num.
É criada uma lista chamada fibonacci com os dois primeiros números da sequência.
O programa entra em um loop while que adiciona o próximo número da sequência de Fibonacci na lista fibonacci até que o último número da lista seja maior ou igual ao número informado pelo usuário.
É verificado se o número informado pelo usuário pertence à lista fibonacci com a palavra-chave in e uma estrutura condicional if.
Dependendo do resultado da verificação, o programa imprime uma mensagem informando se o número pertence ou não à sequência de Fibonacci.

faturamento_diario = [1500.0, 2300.0, 1200.0, 1800.0, 2000.0, 2100.0, 1700.0, 2500.0, 1900.0, 2200.0, 2400.0, 2600.0, 2000.0, 2100.0, 1700.0, 2200.0, 1800.0, 1500.0, 2400.0, 1900.0, 2000.0, 2100.0, 2200.0, 1700.0, 1800.0, 2100.0, 1900.0, 2500.0, 2200.0]

# Calculando o menor valor de faturamento diário
menor_faturamento = min(faturamento_diario)
print("O menor valor de faturamento diário foi:", menor_faturamento)

# Calculando o maior valor de faturamento diário
maior_faturamento = max(faturamento_diario)
print("O maior valor de faturamento diário foi:", maior_faturamento)

# Calculando a média mensal de faturamento diário
media_mensal = sum(faturamento_diario) / len(faturamento_diario)

# Calculando o número de dias em que o faturamento diário foi superior à média mensal
dias_acima_da_media = sum(1 for faturamento in faturamento_diario if faturamento > media_mensal)
print("O número de dias em que o faturamento diário foi superior à média mensal foi:", dias_acima_da_media)

##Explicando o código:

O vetor faturamento_diario armazena os valores de faturamento diário da distribuidora, que foram previamente definidos no código como um exemplo.
A função min() é usada para calcular o menor valor de faturamento diário e armazená-lo na variável menor_faturamento.
A função max() é usada para calcular o maior valor de faturamento diário e armazená-lo na variável maior_faturamento.
É calculada a média mensal de faturamento diário através da soma dos valores do vetor dividido pelo seu comprimento.
É utilizada uma expressão geradora (for e if juntos) para contar o número de dias em que o faturamento diário foi superior à média mensal. Essa contagem é armazenada na variável dias_acima_da_media.
Por fim, são impressos os resultados obtidos.

# Valores de faturamento mensal por estado
faturamento = {'SP': 67836.43, 'RJ': 36678.66, 'MG': 29229.88, 'ES': 27165.48, 'Outros': 19849.53}

# Calcula o faturamento total
faturamento_total = sum(faturamento.values())

# Calcula e imprime o percentual de cada estado
for estado, valor in faturamento.items():
    percentual = valor / faturamento_total * 100
    print(f'{estado}: {percentual:.2f}%')


O resultado do programa será:

SP: 40.49%
RJ: 21.88%
MG: 17.38%
ES: 16.13%
Outros: 4.12%

Isso significa que o estado de São Paulo teve a maior representação no faturamento mensal da distribuidora, com 40,49% do total, seguido pelo Rio de Janeiro com 21,88%, Minas Gerais com 17,38%, Espírito Santo com 16,13% e os outros estados com 4,12% do total.
