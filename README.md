

calculado

def prompt_menu():
    a = float(input("Escolha o primeiro número: "))
    b = float(input("Escolha o segundo número: "))
    print("""
Choose an operation from the list:
1. Adição
2. Subtração
3. Multiplicação
4. Potência
5. Divisão

    """)
    op = int(input("Enter the choice number: "))
    return a, b, op

def calculate():
    a, b, op = prompt_menu()
    if op == 1:
        print("adição: {} + {} = {}".format(a,b,a+b))
    elif op == 2:
        print("subtração: {} - {} = {}".format(a,b,a-b))
    elif op == 3:
        print("multiplicação: {} * {} = {}".format(a,b,a*b))
    elif op == 4:
        print("potência: {}^{} = {}".format(a,b,a**b))
    elif op == 5:
        try:
            print("divisão: {} / {} = {}".format(a,b,a/b))
        except:
            print("Divisão por 0 não é possível!")

    else:
        print("Não existe essa escolha!")
    loop()


