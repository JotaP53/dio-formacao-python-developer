# Anotações Curso 04 - Estruturas Condicionais e de Repetição em Python

----------------------------------------------------------------
### Identação e Blocos

**Identação**<br/>
Itentar código é uma forma de manter o código mais legível e manutenível.<br/>
Mas em Python, ela também exerce um outro pape: o interpretatador consegue determinar onde um bloco de comando inicia e onde ele termina.<br/>

**Bloco de Comando**<br/>
As linguagens de programação costumam utilizar caracteres ou palavras reservadas para terminar o início e  fim do bloco. Em Java e C, por exemplo, utilizam chaves.<br/>

**Utilizando Espaços**<br/>
Existe uma convenção em python que define as boas práticas para escrita de código na linaguem. Nesse documento é indicado utilizar 4 espaços em branco por nível de identação, ou seja, a cada novo bloco adicionamos 4 novos espaços em branco.<br/>

----------------------------------------------------------------
### Estruturas Condicionais

**if / if-else / elif**<br>

A estrutura condicional permite o desvio de fluxo de controle, quando determinadas expressões lógicas são atendidas.<br>

Ex: carteira de motorista. SE o candidato puder tirar, os sistema permite, SE NÃO, não permite.<br>

*if*<br>

Para criar uma estrutura condicional simples, composta por um único desvio, podemos utilizar a palavra reservada *if*. O comando irá testar a expressão lógica, e em caso de retorno verdadeiro as ações presentes no bloco de código do if serão executadas.<br>

    saldo = 2000.0
    saque = float(input("Informe o valor: "))

    if saldo >= saque
        print("Realizando saque!")

    if saldo < saque
        print("Saldo insuficiente!")

*if/else*<br>

Para criar uma estrutura condicional com dois desvios, podemos utilizar as palavras reservadas *if* e *else*. como sabemos, se a expressão lógica testada no if for verdadeira, então o bloco de código do if será executado. Caso contrário o bloco de código do else será executado.<br>

    saldo = 2000.0
    saque = float(input("Informe o valor: "))

    if saldo >= saque
        print("Realizando saque!")

    else:
        print("Saldo insuficiente!")

*elif*<br>

Em alguns cenários queremos mais de dois desvios, para isso podemos utilizar a palavra reservada *elif*. O elif é composto por uma nova expressão lógica, que será testada e caso retorne verdadeiro o bloco de código do elif será executado. Não existe um número máximo de elifs que podemos utilizar, **porém evite criar grandes estruturas condicionais, pois elas aumentam a complexidade do código**.<br>

    opcao = int(input("Informe uma opção: [1] Sacar \n[2] Extrato: "))

    if opcao == 1:
        valor = float(input("Informe a quantia para o saque: "))
        # ...
    elif opcao == 2:
        print("Exibindo o extrato ... ")
    else:
        sys.exit("Opção inválida")

**if aninhado**<br>



**if ternário**<br>

----------------------------------------------------------------
### Estruturas de Repetição