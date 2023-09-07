# Anotações Curso 03 - Tipos de Operadores em Python

----------------------------------------------------------------
### Operadores Aritméticos

**O que são?**
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
São operadores que servem para comparar dois valores.

*Igualdade (==)*
    saldo = 450
    saque = 200

    print(saldo == saque)
    >>> False

*Diferença (!=)*
    saldo = 450
    saque = 200

    print(saldo != saque)
    >>> True

*Maior/Maior Igual (>/>=):*
    saldo = 450
    saque = 200

    print(saldo > saque)
    >>> True
    print(saldo >= saque)
    >>> True

*Menor/Menor Igual (</<=):*
    saldo = 450
    saque = 200

    print(saldo < saque)
    >>> False
    print(saldo <= saque)
    >>> False

----------------------------------------------------------------
### Operadores de Atribuição

**O que são e para que servem?**
São operadores utilizados para definir o valor inicial ou sobrescrever o valor de um variáve.

*Atribuição Simples (=)*
    saldo = 500

    print(saldo)
    >>>500

*Atribuição com Adição (+=)*
    saldo = 500
    saldo += 200

    print(saldo)
    >>>700

*Atribuição com Subtração (-=)*
    saldo = 500
    saldo -= 100

    print(saldo)
    >>>600

*Atribuição com Multiplicação ( *= )*
    saldo = 500
    saldo *= 2

    print(saldo)
    >>>1000

*Atribuição com Divisão Float (/=)*
    saldo = 500
    saldo /= 5

    print(saldo)
    >>>100.0

*Atribuição com Divisão Inteiro (//=)*
    saldo = 500
    saldo //= 5

    print(saldo)
    >>>100

*Atribuição com Módulo (%=)*
    saldo = 500
    saldo %= 480

    print(saldo)
    >>>20

*Atribuição com Exponeciação ( Não deu para inserir o simbolo aqui )*
    saldo = 500
    saldo **= 2

    print(saldo)
    >>>6400

----------------------------------------------------------------
### Operadores Lógicos

----------------------------------------------------------------
### Operadores de Identidade

----------------------------------------------------------------
### Operadores de Associação