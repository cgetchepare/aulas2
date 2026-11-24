# Diário de Bordo

24/11/2026

Notas de aula de Carlos G.F.E.

## Análise de Dados com Python - T7

## Manipulação Básica de Dados

### O que significa ler e escrever arquivos?

|**Operação**|**Significado**|**Exemplo**|
|-|-|-|
|Leitura<br />Arquivo -> Programa|Recuperar dados de um arquivo para utilizá-los no programa.|Carregar uma planilha de produtos.|
|Escrita<br />Programa -> Arquivo|Gravar dados do programa em um arquivo.|Salvar um relatório de estoque.|

https://docs.python.org/pt-br/3/library

### Conhecendo os três formatos

|**Formato**|**Como organiza os dados**|**Exemplo de uso**|
|-|-|-|
|CSV<br />(.csv)|Texto organizado em registros e campos separados por um delimitador.|Exportação de uma tabela de vendas.|
|JSON<br />(.json)|Texto com objetos, listas e valores, permitindo estruturas aninhadas.|Troca de dados entre sistemas.|
|Excel<br />(.xlsx)|Pasta de trabalho com uma ou mais planilhas.|Relatório consultado por uma equipe.|

### Importar uma biblioteca em Python

Importar uma biblioteca em Python significa trazer para o seu programa um conjunto de recursos que já foram desenvolvidos, para que você possa utilizá-los sem precisar criar tudo do zero.

```
import openpyxl
```

"Quero usar os recursos da biblioteca openpyxl neste programa".

Podemos pensar em uma biblioteca como uma caixa de ferramentas. Sem importar uma biblioteca, você teria apenas as ferramentas básicas do Python. Ao importar uma biblioteca, você passa a ter acesso a novas informações específicas.

