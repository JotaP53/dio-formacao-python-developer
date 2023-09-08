# Anotações Curso 03 - Tipos de Operadores em Python

----------------------------------------------------------------
### Operadores Aritméticos

**O que são e para que servem?**
<br/>
Operadores que executam operações matemáticas como adição, subtração, multiplicação e divisão.
* Adição: +
* Subtração: -
* Multiplicação: *
* Divisão Float: / (Nesse tipo de divisão sempre retorna o número em float)
* Divisão Inteira: // (Nesse tipo de divisão o resultado é sempre inteiro)
* Móduo (Resto da Divisão): %
* Exponeciação: ** (Exemplo: 2 ** 3 = 8)

**Precedência dos operadores**
Regra que marca qual operação deve ser feita primeira que a outra.

Ordem em que a precedência acontece:
1. Paêntesis
2. Expoêntes
3. Multiplicações e Divisões (da esquerda pra direita)
4. Somas e subtrações (da esquerda pra direita)

----------------------------------------------------------------
### Operadores de Comparação

**O que são e para que servem?**
<br/>
São operadores que servem para comparar dois valores.

*Igualdade (==)*
    <br/>
    saldo = 450
    saque = 200

    print(saldo == saque)
    >>> False

*Diferença (!=)*
    <br/>
    saldo = 450
    saque = 200

    print(saldo != saque)
    >>> True

*Maior/Maior Igual (>/>=):*
    <br/>
    saldo = 450
    saque = 200

    print(saldo > saque)
    >>> True
    print(saldo >= saque)
    >>> True

*Menor/Menor Igual (</<=):* 
    <br/>
    saldo = 450
    saque = 200

    print(saldo < saque)
    >>> False
    print(saldo <= saque)
    >>> False

----------------------------------------------------------------
### Operadores de Atribuição

**O que são e para que servem?**
<br/>
São operadores utilizados para definir o valor inicial ou sobrescrever o valor de uma variável.

*Atribuição Simples (=)*
    <br/>
    saldo = 500

    print(saldo)
    >>>500

*Atribuição com Adição (+=)*
    <br/>
    saldo = 500
    saldo += 200

    print(saldo)
    >>>700

*Atribuição com Subtração (-=)*
    <br/>
    saldo = 500
    saldo -= 100

    print(saldo)
    >>>600

*Atribuição com Multiplicação (Não deu para inserir o simbolo aqui)*
    <br/>
    saldo = 500
    saldo *= 2

    print(saldo)
    >>>1000

*Atribuição com Divisão Float (/=)*
    <br/>
    saldo = 500
    saldo /= 5

    print(saldo)
    >>>100.0

*Atribuição com Divisão Inteiro (//=)*
    <br/>
    saldo = 500
    saldo //= 5

    print(saldo)
    >>>100

*Atribuição com Módulo (%=)*
    <br/>
    saldo = 500
    saldo %= 480

    print(saldo)
    >>>20

*Atribuição com Exponeciação (Não deu para inserir o simbolo aqui)*
    <br/>
    saldo = 500
    saldo **= 2

    print(saldo)
    >>>6400

----------------------------------------------------------------
### Operadores Lógicos

**O que são e para que servem?**
<br/>
São operadores utilizados em conjunto com os operados de comparação para montar uma operação lógica. Quando um operador de comparação é utilizado, o resultado é um booleano, dessa forma podemos combinar operadores de comparação com os operadores lógios, exemplo:<br/>

*op_comparacao + op_logico + op_comparacao...N...*

Exemplos:
<br/>
    saldo = 1000
    saque = 200
    limite = 100
    
    saldo >= saque
    >>> True

    saque <= limite
    >>> False

*Operador E (and)*
<br/>
    saldo = 1000
    saque = 200
    limite = 100

    saldo >= saque and saque <= limite
    >>> False

*Operador OU (or)*
<br/>
    saldo = 1000
    saque = 200
    limite = 100

    saldo >= saque or saque <= limite
    >>> True

Para que AND retorne TRUE, todas as expressões precisam ser VERDADEIRAS
Para que OR retorne TRUE, apenas uma das expressões precisa ser VERDADEIRA

*Operador Negação (not)*
<br/>
    contatos_emergencia = []

    not 1000 > 1500
    >>> True

    not contatos_emergencia
    >>> True

    not "saque 1500;"
    >>> False

    not ""
    >>> True

*Operador Parênteses*
<br/>

Lembrar que Parênteses tem uma função de determinar a precedência, aqui ele cumpre a mesma função.
<br/>
    saldo = 1000
    saque = 250
    limite = 200
    conta_especial = True

    saldo >= saque and saque <= limite or conta_especial and saldo >= saque
    >>> True

    (saldo >= saque and saque <= limite) or (conta_especial and saldo >= saque)
    >>> True

----------------------------------------------------------------
### Operadores de Identidade

**O que são e para que servem?**
<br/>
São operadores utilizados para comparar se os dois objetos testados ocupam a mesma posição na memória.<br/>

Exemplo:
<br/>

    curso = "Curso de Python"
    nome_curso = curso
    saldo, limite = 200, 200

    curso is nome_curso
    >>> True

    curso is not nome_curso
    >>> False

    saldo is limite
    >>> True

----------------------------------------------------------------
### Operadores de Associação

**O que são e para que servem?**
<br/>
São operadores utilizados para verificar se um objeto está presente em uma sequência.<br/>

Exemplo:
<br/>

    curso = "Curso de Python"
    frutas = ["laranja", "uva", "limão"]
    saques = [1500, 100]

    "Python" in curso
    >>> True

    "maçã" not in frutas
    >>> True

    200 in saques
    >>> False