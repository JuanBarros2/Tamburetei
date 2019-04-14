# Primeiro estágio

## 2012.2

1. Diferencie token, lexema e padrão
*R. Token é um par consistindo em um nome e um valor de atributo opcional; Lexema é uma sequência de caracteres no programa fonte que casa com o padrão para um token; Padrão é uma descrição da forma que os lexemas de um token podem assumir;*


2. Na etapa de análise léxica, um identificador também pode ser combinado como uma palavra chave. Cite dois modos que fazem com que o analisador léxico não dê conflito para o caso acima.
*R. Criar diagramas de transição separados para cada palavra reservada; Cadastrar palavras reservadas na tabela de símbolos e realizar consultas subseqüentes.*

3. Escreva as definições regulares para as seguintes linguagens:
    1. Todas as cadeias de letras que contenham as cinco vogais ordenadas. **alfabeto = [a-z]**
    *R. consoantes = {bcdfghjklmnpqrstvwxyz}*
    * *
    2. Todas as cadeias de letras nas quais as letras estão em ordem lexicográfica ascendente.
    *R. palavra = a * b * c * d * e * f * g * h * i * j * k * l * m * n * o * p * q * r * s * t * u * v * w * x * y * z*
    3. Comentários consistindo em uma cadeia envolvida por /* e */ sem o */ intervenientes a menos que figurem entre aspas.
    *R. *
    4. Todas as cadeias de zero e uns com um número par de zeros e ímpar de uns.


4. Contrua um autômato finito não-determinístico para as seguintes expressões regulares. Mostre a sequência de movimentos feita por cada uma no processamento da cadeia de entrada *ababbab*.
    1. (a|b)*
    2. (a*|b*)*
    3. ((ε|a)b*)*
    4. (a|b)* abb(a|b)*


5. Descreva as linguagens denotadas pelas seguintes expressões regulares
    1. a(a|b)*a
    2. ((ε|a)b*)*
    3. (a|b)*a(a|b)(a|b)
    4. a*ba*ba*ba*
    5. (aa|bb)((ab|ba)(aa|bb)*(ab|ba)(aa|bb)*)*


6. Faça diagramas de transição para reconhecer as mesmas linguagens como cada uma das seguintes expressões regulares:
    1. a(a|b)*a
    2. ((ε|a)b*)*
    3. (a|b)* abb(a|b)*
4. Suponha que tenhamos os seguintes tokens: (1) a palavra chave while; a palavra-chave when; e identificadores consistindo em sequencias de letras e dígitos, começando com uma letra. Mostre:
    1. O NFA para esses tokens;
    2. O DFA para esses tokens;