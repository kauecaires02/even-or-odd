# even-or-odd

    from random import randint
     
    print('Par ou Impar?')
    print('Digite um numero entre 1 e 10')
     
    vcNumero = int(input())
     
    print('Voce escolhe (P)ar ou (I)mpar?')
    vcEscolha = input()
     
    cpNumero = randint(1,10)
    soma = vcNumero + cpNumero
    resultado = ""
     
    if soma % 2 == 0:
        if vcEscolha.lower() == 'p':
            resultado = "Deu PAR - WIN"
        else:
            resultado = "Deu PAR - LOSS"
    else:
        if vcEscolha.lower() == 'i':
            resultado = "Deu IMPAR - WIN"
        else:
            resultado = "Deu IMPAR - LOSS"
        
    print("Voce digitou",vcNumero," e escolheu", vcEscolha)
    print("Computador digitou",cpNumero)
    print(resultado)
