Antes de fazer uma comparação com o algoritmo apresentado em https://kyriosdata.github.io/desafio4x4
eu irei apresentar um algoritmo que acredito ser mais correto.

### **Algoritmo**

**Passo1.** Gerar todas as possíveis combinações de 4 números distintos, entre 1 e 16, cuja soma é 34. Obtendo 86 combinações. 

**Passo2.** Preencher a adiagonal principal com uma das 86 combinações, e eme seguida, preencher a diagonal secundária com qualquer das combinações possiveis restantes.
Isso será feito de forma que todos os conjuntos de 2 combinações sejam utilizados.

>Nota: Uma combinação utilizada na diagonal principal não será utilizada na diagonal secundária em qualquer instância. Para prevenir espelhos verticais.
