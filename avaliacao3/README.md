Antes de fazer uma comparação com o algoritmo apresentado em https://kyriosdata.github.io/desafio4x4
eu irei apresentar um algoritmo que acredito ser mais correto.

### **Algoritmo**

**Passo1.** Gerar todas as possíveis combinações de 4 números distintos, entre 1 e 16, cuja soma é 34. Obtendo 86 combinações. 

**Passo2.** Preencher a adiagonal principal com uma das 86 combinações, e eme seguida, preencher a diagonal secundária com qualquer das combinações possiveis restantes.
Isso será feito de forma que todos os conjuntos de 2 combinações sejam utilizados.

>Nota: Uma combinação utilizada na diagonal principal não será utilizada na diagonal secundária em qualquer instância. Para prevenir espelhos verticais.
>
>![Image](https://github.com/Dener-arx/software-design-2021/blob/main/avaliacao3/Images/EspelhoVertical.png)

**Passo3.** Para cada linha será apresentado um número representando quanto falta para a soma ser 34. E dos 8 números restantes serão encontradas combinações de 2 números que resultam nesses valores, começando da primeira linha e testando todas as possibilidades. 

>Nota1: Combinações do tipo [0,1] e [1,0] serão tratadas de forma distintas.

>Nota2: No exemplo utilizado anteriormente não é possível encontrar uma combinação de dois números cujo resultado seja 31 ou 3, portanto ocorreu uma falha e esse quadrado mágico é invalido.
>
>![Image](https://github.com/Dener-arx/software-design-2021/blob/main/avaliacao3/Images/NumerosIncompativeis.png)

Caso todas as linhas tenham sido preenchidas corretamente, será feita a soma das colunas, somente sendo considerado um quadrado mágico válido caso todos os resultados sejam 34.

**Passo4.** Para cada conjunto da diagonal principal e secundária, também devem ser empregadas as possíveis permutações de suas combinações. 
>Nota: Cada combinação de 4 elementos possui 24 possíveis permutações, entretanto dentre essas 24, 12 permutações são consideradas espelhos(Ex.: 1,6,11,16 e 16,11,6,1), que são desnecessários, pois darão origem a um resultado espelho diagonal.
>
>![Image](https://github.com/Dener-arx/software-design-2021/blob/main/avaliacao3/Images/EspelhoDiagonal.png)

Portanto para cada conjunto de 2 combinações, teremos 12*12 = 124 possibilidades, que devem ser executadas de acordo com o passo 3.




