# Análise de Dados sobre Obesidade
O presente projeto destina-se na construção de um modelo de aprendizado de máquinas, utilizando uma base de dados sobre obesidade.

## Coleta de Dados
 A base de dados foi retirada do site <https://www.kaggle.com> e econtra-se disponível para download no presente repositório.
 Os dados foram divididos em 7 classificações diferentes, sendo estes:
 - Idade
 - Gênero
 - Altura (cm)
 - Peso (Kg)
 - IMC (Índice de Massa Corporal)
 - Nível de Atividade Física
 - Categoria de Obesidade
   
Como os dados não apresentaram nenhum dado nulo, foi preciso somente realizar o tratamento para os dados categóricos nominais de Gênero, já que os dados de **Categoria de Obesidade** serão utilizados como **variável resposta**. Foi utilizado o método One Hot Encoding para tratamento dos dados nominais.

## Modelagem
A modelagem escolhida foi o modelo de **árvore de decisão** com dados de treino(2/3). Sendo que a árvore treinada apresentou um total de **4 folhas**, como ilustrado abaixo.
![Árvore de decisão](https://github.com/Fhamadaa/Projeto_Obesidade/assets/143123795/90805d2c-2584-44f2-820f-c75c629100e0)

A avaliação foi realizada através da **matriz confusão**, conforme ilustrado na sequência.
![Matriz confusão](https://github.com/Fhamadaa/Projeto_Obesidade/assets/143123795/fc7dec74-8270-4126-b314-6a282ae8adbc)

## Conclusão
Com os dados já treinados, foi possível realizar o cálculo da **acurácia**. Com um total de 1000 linhas de dados, 750 destas foram treinadas e 250 foram utilizadas para teste. Dos valores para teste, 249 foram acertivos. Totalizando assim, uma acurácia de **99,6%** do modelo.
