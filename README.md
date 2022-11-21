# Copa do Mundo de Futebol

Você foi convocado para fazer parte da equipe de desenvolvimento da FIFA! O objetivo é criar um sistema que permita a
gestão de uma Copa do Mundo de Futebol.

## Primeira Etapa

A primeira etapa consiste em criar um sistema que realizará o sorteio dos grupos da Copa do Mundo. Para isso, você deve
criar um programa que:

1. Leia o nome de todos os países participantes da Copa do Mundo;
2. Realize o sorteio dos grupos;
3. Imprima na tela o resultado do sorteio.

O sorteio possui as seguintes regras:

1. Cada grupo deve conter 4 países;
2. Seleções do mesmo continente não podem ficar no mesmo grupo, com exceção da Europa, que pode ter até 2 seleções no
mesmo grupo;
3. As seleções cabeças de chave não podem ficar no mesmo grupo;

### Dicas

1. Utilize a biblioteca [random](https://docs.python.org/3/library/random.html) para realizar o sorteio;
```
import random
grupoA = {}
grupoB = {}
grupoC = {}
grupoD = {}
grupoE = {}
grupoF = {}
grupoG ={}
grupoH = {}
times_euro = ['Holanda', 'Inglaterra', 'Gales', 'Polônia', 'França', 'Espanha', 'Alemanha', 'Bélgica', 'Croácia', 'Sérvia', 'Suíça', 'Portugal']
times_america = ['Equador','EUA','Argentina','México', 'CostaRica','Canadá','Brasil','Uruguai', 'Dinamarca']
times_asia = ['Qatar','Irã','ArábiaSaudita','Tunísia','Japão','Coreia']
times_africa = ['Marrocos','Senegal','Camarões','Gana',]
times_oceania = ['Austrália']
times = times_euro + times_america + times_asia + times_africa + times_oceania
n = 4
sorteioA = random.sample(times, n)
times = list(set(times) - set(sorteioA))
sorteioB = random.sample(times, n)
times = list(set(times)- set (sorteioB))
sorteioC = random.sample(times, n)
times = list(set(times)- set (sorteioC))
sorteioD = random.sample(times, n)
times = list(set(times)- set (sorteioD))
sorteioE = random.sample(times, n)
times = list(set(times)- set (sorteioE))
sorteioF = random.sample(times, n)
times = list(set(times)- set (sorteioF))
sorteioG = random.sample(times,n)
times = list(set(times) - set(sorteioG))
sorteioH = random.sample(times,n)
times = list(set(times) - set(sorteioH))
grupoA = sorteioA
grupoB = sorteioB
grupoC = sorteioC
grupoD = sorteioD
grupoE = sorteioE
grupoF = sorteioF
grupoG = sorteioG
grupoH = sorteioH
```
## Segunda Etapa

A segunda etapa consiste em gerar os jogos da primeira fase da Copa do Mundo. Para isso, você deve criar um programa que:

1. Leia os grupos gerados na primeira etapa;
2. Gere os jogos da primeira fase;
3. Imprima na tela os jogos da primeira fase.

```
n = 2
print('Jogos do Grupo A:')
jogoA1 = random.sample(grupoA, n)
grupoA = list(set(grupoA) - set(jogoA1))
jogoA2 = random.sample(grupoA, n)
jogoA3 = [jogoA1[0], jogoA2[0]]
jogoA4 = [jogoA1[1], jogoA2[1]]
jogoA5 = [jogoA1[0], jogoA4[1]]
jogoA6 = [jogoA3[1], jogoA4[1]]
print(jogoA1)
print(jogoA2)
print(jogoA3)
print(jogoA4)
print(jogoA5)
print(jogoA6)
```

## Terceira Etapa

A terceira etapa consiste em criar um sistema que construa a pontuação dos grupos da Copa do Mundo. Para isso, você deve
criar um programa que:

1. Leia os jogos gerados na segunda etapa;
2. Leia os resultados dos jogos de cada grupo;
3. Imprima na tela a pontuação de cada grupo.

## Quarta Etapa

A quarta etapa consiste em criar um sistema que gere os confrontos da fase final da Copa do Mundo. Para isso, você
deve criar um programa que:

1. Leia o resultado dos grupos gerados na terceira etapa;
2. Gere os confrontos da fase final;
3. Imprima na tela os confrontos da fase final.
4. Leia o resultado de cada jogo das fases finais até chegar na grande final;
5. Imprima na tela o resultado da grande final.
