Passo 1
    - Encontrar todas as póssiveis combinações de 4 números(entre 1 e 16) cuja soma resulta em 34. (No total existem 86 combinações).
    - Essas combinações de números deverão ser salvas em uma tabela. 
    - A tabela 86x4 deve ser preenchida dos números maiores aos menores. (16,15,2,1) (16,14,3,1) (16,13,4,1)...
    - Uma segunda tabela será criada a partir desta, indicando em quais linhas cada númeral pode ser encontrado. (Ex. 16 -> 1,2,3,4...) (Para melhor localização dos números             menores.)
    
Passo 2
    - Começando na pósição (1,1) do quadrado mágico será adicionado o primeiro valor da tabela 86x4. (16)
    - Das casas adjacentes a (1,1) serão colocados as possiveis combinações de 16 começando pelas maiores. (Somente para as pósições que contabilizam 34).
        - O valor da soma de todas as linhas e colunas, bem como das diagonais deve ser contabilizado, reduzindo de 34 o valor das areas preenchidas.
        - Se não for possivel zerar com os números não utilizados uma outra iteração deve ser iniciada. 
        - EX.: Linha 1 = (16,15,2,1). Coluna 1 = (16,14,3,1). Não é possivel sendo que o 1 já está presente em outro local.
     - Completado as casas adjacentes a (1,1) passamos para a próxima casa (1,2) que teria valor (15) e repetimos o processo.
     - O mesmo será feito para as casas (1,3), (1,4), (2,1) e assim por diante, até que um quadrado mágico perfeito seja concluido, ou até uma impossibilidade acontecer.
     
Passo 3
    - Após a iteração com 16 como valor inicial o mesmo deve ser feito para os outros valores.
    
Passo 4
    - Terminada todas as iterações com a pósição (1,1) como ponto inicial o processo deve ser repetido tomando as outras pósições como inicio. (1,2), (1,3), (1,4), (2,1)...

Passo 5
    - Para cada quadrado mágico completo e correto, deve ser encontrado todos os seus variantes.
    - Rotacionando o quadrado em 90°, 180° e 270°. 
    - Espelhando o quadrado horizontamente, verticalmente, e em ambas as diagonais.
    - E aplicando multiplas manipulações ao mesmo tempo.
 





