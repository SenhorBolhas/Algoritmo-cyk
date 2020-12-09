# Algoritmo-cyk
Algoritmo CYK executado para gramáticas na forma normal de Chomsky 
Feito em: Jupyter Notebook - Python

1. É necessário um arquivo (gramatica.txt) contendo a gramatica
- A gramática deverá estar na forma normal de Chomsky

2. A leitura do arquivo é feita pela primeira célula

3. As células 3, 4 e 5 registram as funções que serão usadas no CYK e a própria função CYK

4. A celula final serve para executar o algoritmo de fato -> cyk(testarPalavra)
- Teremos uma variável com a palavra sendo passada como parâmetro - nesse caso testarPalavra com "aaaaabbbbb"
- Cada linha de derivação corresponde a uma lista, essas listas são contidas numa lista que é retornada por esse método.

-Casos:
- Aparição do símbolo inicial na ultima linha -> palavra válida na gramática
- Aparição de um símbolo não-inicial OU linha vazia -> palavra inválida na gramática
- Símbolo inválido na palavra -> exceção KeyError levantada

- Para alterar a gramática utilizada, alterar o segundo parâmetro no cyk 
-Ex: cyk(palavra, gramatica=g2)
