# Exercício para a terça-feira:

- Anote suas dificuldades e dúvidas para que possamos conversar na próxima aula!

- Caso não consiga fazer algum dos exercícios, não desista :) pule para o próximo.

- de preferência, anote e me diga no início da aula quanto tempo vocês levaram para fazer esses exercícios.

## Parte 1 - Instalação do R e RStudio

No dia-a-dia é interessante que vocês consigam usar o R e o RStudio no **computador pessoal (ou de trabalho) de vocês**.

Portanto, a parte 1 da tarefa é realizar a instalação do R e do RStudio no computador pessoal, para que consigam usar depois do curso.

### Instalar o R:

Primeiro é necessário instalar o R:

- O link de instalação pode ser encontrado aqui: https://cran.fiocruz.br/

- Caso você use Linux, ele pode pedir que você instale utilizando comandos no terminal, e isso pode ser um pouco assustador. Caso você não tenha costume de usar o terminal, posso ajudar compartilhando a tela no horário antes da aula!

Este outro link pode ajudar também: https://livro.curso-r.com/1-1-instalacao-do-r.html

## Instalar o RStudio: 

Depois de instalar o R, podemos instalar o RStudio:

- O link de instalação pode ser encontrado aqui: https://www.rstudio.com/products/rstudio/download/#download


Este outro link pode ajudar também:
https://livro.curso-r.com/1-2-instalacao-do-rstudio.html

ATENÇÃO: Caso tenha problemas com a instalação, peça ajuda no horário pré-aula (18h30-19h00).


## Parte 2 - teórica:

As etapas a seguir são opcionais, mas caso você não esteja confortável com alguns conceitos, será importante para entender os exercícios que utilizaremos códigos. Conceitos mais importantes: média, mediana, desvio padrão.


- Leitura: Análise com estatística descritiva para leigos: https://escoladedados.org/tutoriais/analise-com-estatistica-descritiva-para-leigos/

- Esse vídeo fala sobre o cálculo de variância e desvio padrão: https://youtu.be/A-N-eEB1owQ - até 21:23


## Parte 3 - Exercitando conceitos

### Exercícios do script da aula 1

Faça os exercícios da [aula 1](https://github.com/beatrizmilz/2024-08-cebrap-lab-intro-R/blob/main/scripts/1-r-base.qmd) (caso algum tenha ficado por fazer).


### Preparando o exercício

1 - Crie um arquivo qmd (para relatórios), e salve o mesmo com o nome `tarefa-1.qmd`.

2 - Nos metadados do arquivo (primeiras linhas), preencha seu nome, a data, e dê o título como `Tarefa 1 - Introdução ao R`.

3 - Aperte knit e veja o que acontece!

### Pausa para uma lista de funções que pode ajudar nos exercícios

Nos exercícios a seguir, precisamos usar algumas funcões para calcular alguns valores. Algumas funções ainda não foram tratadas, mas segue aqui uma lista que pode ser útil:

nome_do_vetor <- c(valor, valor, valor) # - cria um objeto que armazena um conjunto de valores. chamamos isso de VETOR!

class(nome_do_vetor) # - verificar a classe de um vetor

lenght(nome_do_vetor) # - verificar quantos elementos tem em um vetor

mean(nome_do_vetor) # - para vetores numéricos. essa função calcula a média dos valores em um vetor.

median(nome_do_vetor) # - para vetores numéricos. essa função calcula a mediana dos valores em um vetor.

var(nome_do_vetor) # - para vetores numéricos. essa função calcula a variância dos valores em um vetor.

sd(nome_do_vetor) # - para vetores numéricos. essa função calcula o desvio padrão dos valores em um vetor.

min(nome_do_vetor) # - para vetores numéricos. essa função retorna o menor valor encontrado em um vetor.

max(nome_do_vetor) # - para vetores numéricos. essa função retorna o maior valor encontrado em um vetor.

round(nome_do_vetor, numero_de_casas_decimais) # - para vetores numéricos. essa função retorna os valores do vetor arredondados. O segundo argumento define o número de casas decimais para ser usado no arredondamento.

### Respondendo perguntas com código

4 - O vetor abaixo apresenta a esperança de vida por UF no Brasil em 2010:

esp_vida_2010 <- c(71.63, 70.32, 73.8, 73.3, 71.97, 72.6, 77.35, 75.1, 74.6, 70.4, 
74.25, 74.96, 75.3, 72.36, 72, 74.8, 72.32, 71.62, 75.1, 72.52, 
75.38, 72.97, 73.51, 76.61, 75.69, 71.84, 72.56)

Crie um campo de código (chunk), cole o código acima no seu script, para ter disponível o vetor como um objeto. Execute o código e veja se o objeto foi criado no seu environment.

Obs: Lembre-se de que códigos em R devem ser executados dentro de campos de código. Os textos deverão estar fora dos campos de código, ou precedidos por # (hashtag indica comentário). 


5 - Usando o vetor criado anteriormente, cole as perguntas abaixo no seu arquivo de relatório e responda utilizando funções do R. Lembre-se de colocar as respostas dentro de campos de código!

5a - Qual é a classe desse vetor?

5b - Quantos estados estão presentes neste vetor?

5c - Calcule a média, mediana, variância e desvio padrão desse vetor.

5d - Encontre o valor mínimo e máximo deste vetor.

5e - Calcule a amplitude dos valores deste vetor (valor maximo - valor mínimo).

5f - Experimente a função quantile() com o vetor criado. Ex: quantile(nome_do_vetor) . Compare com os outros valores retornados. O que você interpreta do resultado? O que significa os valores em 0%, 25%, 50%, 75%, 100%?

5g - Arredonde os valores deste vetor para apenas 1 casa decimal.

6 - Aperte knit novamente, e veja o resultado. Cada pergunta tem a sua resposta apresentada com códigos?
