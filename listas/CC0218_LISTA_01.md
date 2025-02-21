## CC0218 - LISTA 01

#### Exercício: Dados Brutos
Os dados sobre o número de casas em quarteirões de uma cidade são:

2, 2, 2, 2, 3, 3, 3, 3, 5, 5, 5, 5, 10, 10, 10, 10, 10, 15, 15, 15, 15, 20, 20, 20, 20, 25, 25, 25, 25, 25, 30, 30, 30, 30, 30, 30, 30, 30, 30, 50, 50, 50, 50, 50, 50, 80, 80, 80, 80, 80.

<div>
a) Calcule a mediana.<br>
b) Construa uma tabela com frequências e proporções.
</div>

***Respostas***

a) Há 50 observações. Para dados ordenados, a mediana é a média do 25º e 26º elemento.  
Conforme indicado, os 25º valores correspondem a 20 e os 26º a 25, de modo que

$$\text{Mediana} = \frac{20 + 25}{2} = 22{,}5.$$

b) Primeiro, listamos os valores distintos com suas frequências:

| Valor | Frequência | Proporção  |
|:-----:|:----------:|:----------:|
| 2     | 4          | 4/50 = 0,08  |
| 3     | 4          | 4/50 = 0,08  |
| 5     | 4          | 4/50 = 0,08  |
| 10    | 5          | 5/50 = 0,10  |
| 15    | 4          | 4/50 = 0,08  |
| 20    | 4          | 4/50 = 0,08  |
| 25    | 5          | 5/50 = 0,10  |
| 30    | 9          | 9/50 = 0,18  |
| 50    | 6          | 6/50 = 0,12  |
| 80    | 5          | 5/50 = 0,10  |

Cada proporção é obtida dividindo a frequência do valor pelo total de 50 observações.

#### Exercício: Tabela de Frequência
Queremos estudar o número de erros de impressão de um livro. A tabela abaixo apresenta os dados coletados em uma amostra de 50 páginas:

| **Erros** | **Frequência** |
|-----------|----------------|
| 0         | 25             |
| 1         | 20             |
| 2         | 3              |
| 3         | 1              |
| 4         | 1              |

<div>
a) Qual o número médio de erros por página?<br>  
b) Qual o número mediano?<br>  
c) Qual é o desvio padrão?<br>  
d) Se o livro tem 500 páginas, qual é o número total de erros esperado no livro?
e) Construa um gráfico de barras para representar a distribuição de frequências de erros por página.<br>
</div>

***Respostas***

a) Calcule a média ponderada dos erros:
\[
\bar{x} = \frac{0\cdot25 + 1\cdot20 + 2\cdot3 + 3\cdot1 + 4\cdot1}{50} = \frac{0 + 20 + 6 + 3 + 4}{50} = \frac{33}{50} \approx 0,66.
\]

b) Com 50 observações, a mediana é a média dos valores da 25ª e 26ª posição.

- As 25 primeiras páginas (posição 1 a 25) têm 0 erros.
- A partir da 26ª página, temos 1 erro (pois as 20 ocorrências de 1 erro preenchem as posições 26 a 45).

Assim, a mediana é:
\[
\text{Mediana} = \frac{0 + 1}{2} = 0,5.
\]

c) Primeiro, calculamos o somatório dos quadrados das diferenças entre cada valor e a média, ponderado pela frequência:

1. Para \(x=0\):  
   Diferença: \(0 - 0,66 = -0,66\); quadrado: \(0,4356\).  
   Contribuição: \(25 \times 0,4356 = 10,89\).

2. Para \(x=1\):  
   Diferença: \(1 - 0,66 = 0,34\); quadrado: \(0,1156\).  
   Contribuição: \(20 \times 0,1156 = 2,312\).

3. Para \(x=2\):  
   Diferença: \(2 - 0,66 = 1,34\); quadrado: \(1,7956\).  
   Contribuição: \(3 \times 1,7956 = 5,3868\).

4. Para \(x=3\):  
   Diferença: \(3 - 0,66 = 2,34\); quadrado: \(5,4756\).  
   Contribuição: \(1 \times 5,4756 = 5,4756\).

5. Para \(x=4\):  
   Diferença: \(4 - 0,66 = 3,34\); quadrado: \(11,1556\).  
   Contribuição: \(1 \times 11,1556 = 11,1556\).

Somando as contribuições:
\[
S = 10,89 + 2,312 + 5,3868 + 5,4756 + 11,1556 \approx 35,22.
\]

A variância é:
\[
\sigma^2 = \frac{35,22}{50} \approx 0,7044.
\]

O desvio padrão é:
\[
\sigma \approx \sqrt{0,7044} \approx 0,84.
\]

d)Se a média de erros por página é aproximadamente 0,66, o total esperado de erros em 500 páginas é:
\[
\text{Total} = 0,66 \times 500 \approx 330 \text{ erros}.
\]

#### Exercício: Tabelas de Frequência 2
A tabela abaixo resume o número de filhos de 100 famílias:

| **Número de Filhos** | **Frequência de Famílias** |
|-----------------------|----------------------------|
| 0                    | 10                         |
| 1                    | 27                         |
| 2                    | 28                         |
| 3                    | 19                         |
| 4                    | 9                          |
| 5                    | 4                          |
| Mais que 5           | 3                          |

a) Qual é a moda do número de filhos?  
b) Que dificuldades você enfrentaria para calcular a média exata do número de filhos?

***Respostas:***
a) A moda é 2, pois é o número de filhos que ocorre com maior frequência (28 famílias).

b) O desafio para calcular a média exata é a categoria "Mais que 5", que não especifica quantos filhos, exatamente, estão incluídos. Sem saber o valor exato para essas 3 famílias, não é possível determinar com precisão o total de filhos, o que impede o cálculo exato da média.

#### Exercício: Comparação entre Média e Mediana
Com respeito às medidas de centralidade, 
<div>
a) A média e a mediana sempre coincidem?<br>  
b) Dê um exemplo prático em que a mediana seja uma medida mais adequada do que a média para descrever um conjunto de dados. Justifique sua escolha.<br>
c) Em qual tipo de distribuição os valores da média e mediana são sempre iguais?
</div>

***Respostas:***
a) Não, a média e a mediana não coincidem sempre. Elas são iguais apenas quando os dados estão distribuídos de maneira perfeitamente simétrica.

b) Um exemplo prático é a distribuição de renda em uma cidade. Geralmente, a renda tem uma distribuição assimétrica à direita, em que alguns poucos indivíduos possuem rendas muito altas que elevam a média. Nesse caso, a mediana — que indica o valor central dos dados — fornece uma medida mais representativa da "renda típica", pois não é afetada por esses valores extremos.

c) Em distribuições simétricas, como na distribuição normal, os valores da média e da mediana são sempre iguais.

#### Exercício: Tabela de Classes
A tabela abaixo apresenta a distribuição de frequência da massa corporal ($m$) de um grupo de pessoas. Podemos ter certeza que a **massa corporal média** desse grupo é superior a 70 kg? Justifique sua resposta.

| **Massa Corporal ($m$ em kg)** | **Frequências** |
|----------------------------------|-----------------|
| $40 \leq m < 45$                 | 5               |
| $45 \leq m < 60$                 | 15              |
| $60 \leq m < 70$                 | 25              |
| $70 \leq m < 90$                 | 50              |
| $90 \leq m < 100$                | 5               |
| **Total**                        | 100             |

***Respostas:***
Como não temos certeza das massas de cada indivíduo, vamos considerar o caso extremo (mas possível) em que todos tem o menor peso de suas classes. Assim, utilizando os valores mínimos de cada classe, temos:

- Para \(40 \le m < 45\): \(m = 40\) kg, frequência 5  
- Para \(45 \le m < 60\): \(m = 45\) kg, frequência 15  
- Para \(60 \le m < 70\): \(m = 60\) kg, frequência 25  
- Para \(70 \le m < 90\): \(m = 70\) kg, frequência 50  
- Para \(90 \le m < 100\): \(m = 90\) kg, frequência 5  

Neste caso, a média ponderada será
\[
\mu = (5(40) + 15(45) + 25(60) + 50(70) + 5(90)) / 100 = 63{,}25.
\]

Portanto, ao utilizar os valores mínimos, a massa corporal média estimada será de aproximadamente 63,25 kg que é inferior a 70 kg.

#### **Exercício 8: Medidas de Dispersão**
Quais dessas medidas são **medidas de dispersão**?

I – média;  
II – mediana;  
III – variância;  
IV – desvio padrão;  
V – amplitude interquartil.

***Respostas:***
III, IV e V.

#### Exercício: Transformação nos Dados
Nosso laboratório realizou 150 medições da altura de cactos e obtivemos média igual a $1.7 \, \text{m}$ e variância de $0.25 \, \text{m}^2$, mas descobrimos que nosso instrumento de medição estava com defeito, marcando sempre $25 \, \text{cm}$ acima do valor real. 

<div>
a) Será que podemos corrigir o erro na média e variância ou devemos repetir todas as medições?<br>
b) O que aconteceria com a média, mediana, moda e variância se os dados fossem multiplicados por 2?
</div>

#### Exercício: Boxplot
Construa o **boxplot** das informações do exercício "Dados Brutos" e, com base apenas nele, responda:  
a) Existe alguma simetria na distribuição?  
b) Existem valores discrepantes (outliers)?  
c) O que pode ser concluído sobre a dispersão dos dados?

#### Exercício: Histograma
Construa um **histograma de densidade de frequência** dos dados apresentados no exercício **Tabela de Classes**.

#### Exercício: Coeficiente de Variação e Comparação de Unidades
Considere os seguintes conjuntos de dados:

**Conjunto A:** Alturas de jogadores de basquete (em centímetros)  
198, 202, 195, 200, 197, 203, 199, 201

**Conjunto B:** Salários mensais de executivos (em milhares de reais)  
15, 22, 18, 25, 19, 23, 20, 24

a) Calcule o coeficiente de variação (CV) para ambos os conjuntos.  
b) Qual conjunto apresenta maior variabilidade relativa? Justifique por que o CV é mais adequado para esta comparação do que o desvio padrão.  
c) Em quais situações práticas o uso do CV seria mais apropriado do que o desvio padrão?

#### Exercício: Correlação entre variáveis quantitativas
Determine se $Y$ ou $Z$ estão mais correlacionadas com a variável $X$. Justifique sua resposta.

| $X$    | $Y$    | $Z$    |
|--------|--------|--------|
| 41     | 52     | 60     |
| 73     | 95     | 35     |
| 67     | 72     | 60     |
| 37     | 52     | 80     |
| 58     | 96     | 50     |

#### Exercício: Correlação entre variáveis qualitativas
Considerando os dados da tabela abaixo, podemos dizer que há correlação entre o sexo e a frequência de atividades físicas? Justifique sua resposta.

| **Frequência de Atividades** | **H**  | **M**  | **Total** |
|------------------------------|--------|--------|-----------|
| **Ativo**                    | 149    | 148    | 297       |
| **Sedentário**               | 13     | 51     | 64        |
| **Eventual**                 | 31     | 10     | 41        |
| **Total**                    | 193    | 209    | 402       |


#### Exercício: Correlação entre variáveis qualitativas e quantitativas

Uma empresa deseja analisar se há uma relação entre o setor de atuação dos funcionários (Administrativo, Financeiro, Operacional) e o salário mensal recebido. Para isso, foram coletados dados de uma amostra de funcionários, conforme a tabela abaixo:

| **Nome**        | **Setor**      | **Salário Mensal (R$)** |
|-----------------|----------------|-------------------------|
| Ana Silva       | Administrativo | 3.500                   |
| Maria Oliveira  | Administrativo | 3.600                   |
| João Santos     | Administrativo | 3.800                   |
| Julia Lima      | Financeiro     | 4.300                   |
| Pedro Costa     | Financeiro     | 4.200                   |
| Lucas Pereira   | Financeiro     | 4.500                   |
| Paula Martins   | Operacional    | 2.900                   |
| Rita Santos     | Operacional    | 2.700                   |
| Bruno Ferreira  | Operacional    | 3.000                   |
| Carlos Souza    | Operacional    | 2.800                   |


#### Exercício: Z-score
A média e a variância das notas dos alunos de Cálculo da turma $A$ foram iguais a 4. Na turma $B$, a média das notas em Cálculo foi de 7 e o desvio padrão foi 1. João é um aluno da turma $A$, Flávio é um aluno da turma $B$ e ambos tiraram 8. Você acha que Flávio se saiu melhor que João quando comparado aos demais alunos de suas respectivas turmas? Justifique sua resposta.
