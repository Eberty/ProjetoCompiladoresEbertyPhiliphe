# Lexical analyzer in compiler project for Portugol language

## Portugol 
Portugol is a pseudolanguage that allows 
the reader to develop algorithms structured in Portuguese in a simple and intuitive way, regardless of programming language.
[See in Wikipedia(PT)](https://pt.wikipedia.org/wiki/Portugol)
## Grammar
Programa → **inicio** Declarações Comandos **fim** <br>
Declarações → Declaração Declarações | ε<br>
Declaração → Tipo **:** Identificadores **;**<br>
Tipo → **int** | **dec**<br>
Identificadores → Identificador **,** Identificadores | Identificador<br>
Comandos → Comando Comandos | ε<br>
Comando → CMD-Se | CMD-Para | CMD-Obtenha | CMD-Mostre | CMD-Atrib<br>
CMD-Se → **se** Expr **entao** Comandos **senao** Comandos **fim_se** | **se** Expr **entao** Comandos **fim_se**<br>
CMD-Para → **para** Identificador **de** Expr **ate** Expr **passo** Expr Comandos **fim_para** | **para** Identificador **de** Expr **ate** Expr Comandos **fim_para**<br>
CMD-Obtenha → **leia** **(** Identificador **)** **;**<br>
CMD-Mostre → **imprima** **(** Identificador **)** **;** | **imprima** ( Número )**;** | **imprima** ( Cadeia ) **;**<br>
CMD-Atrib → Identificador **<-** Expr **;**<br>
Expr → Expr OpBinario Expr | OpUnario Expr | Número<br>
OpBinario → **+** | **-** |  **\***  | **/** | **e** | **ou** | **=** | **<>** | **>** | **>=** | **<** | **<=**<br>
OpUnario → **-** | **++** | **--** | **nao**<br>
Número → Inteiro | Decimal<br>
## Automato
![alt text](https://github.com/Eberty/ProjetoCompiladoresEbertyPhiliphe/tree/master/Automato/automato.jpg "Automato")
## Transition Table
![alt text](https://github.com/Eberty/ProjetoCompiladoresEbertyPhiliphe/tree/master/Automato/transitionTable.png "Transitions")

## Input and output
https://github.com/pharkrum/Compiler-Project-to-Portugol/blob/master/Arquivos/Portugol-Relatorio.pdf
