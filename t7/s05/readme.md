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
|CSV<br />.csv|Texto organizado em registros e campos separados por um delimitador.|Exportação de uma tabela de vendas.|
|JSON<br />.json|Texto com objetos, listas e valores, permitindo estruturas aninhadas.|Troca de dados entre sistemas.|
|Excel<br />.xlsx|Pasta de trabalho com uma ou mais planilhas.|Relatório consultado por uma equipe.|

### Importar uma biblioteca em Python

Importar uma biblioteca em Python significa trazer para o seu programa um conjunto de recursos que já foram desenvolvidos, para que você possa utilizá-los sem precisar criar tudo do zero.

```
import openpyxl
```

"Quero usar os recursos da biblioteca openpyxl neste programa".

Podemos pensar em uma biblioteca como uma caixa de ferramentas. Sem importar uma biblioteca, você teria apenas as ferramentas básicas do Python. Ao importar uma biblioteca, você passa a ter acesso a novas informações específicas.

### Instalar uma biblioteca

Instalar uma biblioteca significa adicionar novos recursos ao ambiente Python para que eles possam ser usados nos seus programas.

```
pip install openpyxl
```

"Python, instale a biblioteca neste ambiente."

O Python já vem com várias bibliotecas prontas, como math, datetime e csv. Porém, outras bibliotecas precisam ser instaladas separadamente.

Instalar a biblioteca é como instalar o aplicativo. Importar é como abrir esse aplicativo quando você precisa utilizá-lo.

* Lendo e salvando arquivos CSV.
* Lendo e salvando arquivos JSON.
* Lendo e salvando arquivos XLSX.
* \[VS CODE]

### Módulo datetime

O módulo datetime faz parte da biblioteca padrão do Python, portanto não precisa ser instalado com pip. Ele fornece classes para representar e manipular datas, horários e intervalos de tempo. Entre as principais estão:  date, time, datetime e timedelta.

*datetime* é a caixa de ferramentas do Python para trabalhar com datas e horas

\[VS CODE]

https://docs.python.org/pt-br/3.12/library/datetime.html

### Expressões regulares básicas para limpeza de dados

As expressões regulares, também chamadas de Regex (Regular Expressions), são padrões utilizados para procurar, identificar, extrair, substituir ou remover partes de textos.

No Python, trabalhamos com expressões regulares principalmente por meio do módulo

```
import re
```

Regex é uma forma de dizer ao Python qual padrão de texto queremos encontrar.

## Funções e Modularização

|Módulo<br />arquivo Python<br />códigos reutilizáveis|Import<br />usa o módulo em outro arquivo|
|-|-|

### Por que utilizar módulos?

Com o crescimento do projeto, o arquivo começa a ficar grande.

Já utilizamos módulos várias vezes:

```
import re
```

```
import pandas
```

```
import datetime
```

Estamos utilizando o sistema de importação do Python para acessar funcionalidades disponibilizadas externamente ao nosso arquivo. A instrução import procura o módulo solicitado e associa esse módulo a um nome disponível no programa.

### if \_\_name\_\_ == "\_\_main\_\_":

O comando if \_\_name\_\_ == "\_\_main\_\_":  é uma estrutura condicional em Python  usada para garantir que um bloco de código seja executado apenas quando o arquivo for rodado diretamente, e não quando for importado como um módulo em outro script.

Esse recurso é muito útil para colocar testes ou exemplos dentro do próprio módulo.

```
if \_\_name\_\_ == "\_\_main\_\_":
```

### \*args e \*\*kwargs

\*args e \*\*kwargs:  argumentos especiais.

|       \*args||       \*\*kwargs||
|-|-|-|-|
|recebe|armazena|recebe|armazena|
|posicionais|tupla|nomeados|dicionário|

* \*args:  permite que uma função receba uma quantidade variável de argumentos posicionais.
* \*\*kwargs:  permite receber uma quantidade variável de argumentos nomeados.
