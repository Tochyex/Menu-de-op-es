num1 = int(input('Primeiro valor: '))
num2 = int(input('Segundo valor: '))
opcao = 0
maior = 0
menor = 0
while opcao != 5:
    print('\033[1;31m-='*15, '\033[m')
    print('''\033[1;33m    [1] Soma
    [2] Multiplicação
    [3] Maior
    [4] Novos valores
    [5] Sair do programa\033[m''')
    opcao = int(input('Selecione uma das opções acima: '))
    multi = num1 * num2
    if opcao == 1:
        soma = num1 + num2
        print('Somando os valores {} e {} o resultado é {} '.format(num1, num2, soma))
    elif opcao == 2:
        multi = num1 * num2
        print('Multiplicando os valores {} e {} o resultado é {} '.format(num1, num2, multi))
    elif opcao == 3:
        if num1 > num2:
            maior = num1
        else:
            maior = num2
        print('Entre os valores {} e {} o maior é {} '.format(num1, num2, maior))
    elif opcao == 4:
        print('Digite novamente os valores.')
        num1 = int(input('Primeiro valor: '))
        num2 = int(input('Segundo valor: '))
    elif opcao == 5:
        print('Fim do programa.')
    else:
        print('Opção invalida, digite outra opção.')
    print('\033[1;31m-='*15, '\033[m')
print('Programa finalizado com sucesso, Obrigado!')
        
