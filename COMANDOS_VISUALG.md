# Cola: VisuALG (Portugol) — comandos essenciais

Resumo rápido: use VisuALG para escrever pseudocódigo claro antes de traduzir para C++/Arduino.

## Tipos básicos
- inteiro
- real
- caractere
- texto
- logico

## Declaração de variáveis
```
var
  n: inteiro
  media: real
  nome: texto
fimvar
```

## Entrada / Saída
```
leia(n)
escreva("Valor: ", n)
```

## Atribuição e expressões
```
n <- 10
media <- (a + b) / 2
```

## Condicionais
```
se x > 0 entao
  escreva("positivo")
senao
  escreva("não positivo")
fimse
```

## Repetições
```
para i de 1 ate n faca
  escreva(i)
fimpara

enquanto condicao faca
  ...
fimenquanto

faca
  ...
enquanto condicao
```

## Vetores (exemplo)
```
var
  v: inteiro[10]
fimvar
v[1] <- 5
```

## Procedimentos / Funções
```
procedimento soma(a, b)
  escreva(a + b)
fimprocedimento

funcao inteiro dobro(x)
  retorno x * 2
fimfuncao
```

## Comentários
```
// comentário de linha
/* comentário
   em várias linhas */
```

## Exemplo rápido (pseudocódigo)
```
algoritmo "media"
var
  a, b: real
fimvar
leia(a)
leia(b)
media <- (a + b) / 2
escreva("Média = ", media)
fimalgoritmo
```

-- Fim da cola VisuALG --
