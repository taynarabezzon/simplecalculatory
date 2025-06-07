print("simplecalculatory")

listadestrings = ['SOMA:1', 'SUBTRAÇÃO:2', 'MULTIPLICAÇÃO:3', 'DIVISÃO:4']

for i in listadestrings:
    print(i)

operação = int(input('Escolha a operação (1 = Soma, 2 = Subtração, 3 = Multiplicação, 4 = Divisão): '))
num1 = float(input('Escolha o primeiro número: '))
num2 = float(input('Escolha o segundo número: '))

def resultado():
    if operação == 1:
        res = num1 + num2
        print(f'{num1} + {num2} = {res}')
    elif operação == 2:
        res = num1 - num2
        print(f'{num1} - {num2} = {res}')
    elif operação == 3:
        res = num1 * num2
        print(f'{num1} * {num2} = {res}')
    elif operação == 4:
        if num2 == 0:
            print('Esta operação não é possível: divisão por zero.')
        else:
            res = num1 / num2
            print(f'{num1} / {num2} = {res}')
    else:
        print('Operação inválida.')

resultado()


