# •	Análise de Viagens de Bicicleta para a Conversão de Clientes

## Nota importante:

Dentro do Jupyter Notebook disponível nesse projeto pode ser encontrado todo o meu código, além de caixas de texto. Nessas caixas de texto há explicações sobre cada etapa do processo de análise. Meu objetivo foi fazer com que essas explicações pudessem ser entendidas por qualquer pessoa, mesmo que não seja da área de dados. Portanto, caso você não possua conhecimento em programação e/ou análise de dados, ainda pode ler o jupyter notebook e acompanhar todo o meu raciocínio.

## Descrição do projeto:

Esse é o projeto final do curso “Google Data Analytics Certificate” promovido pelo Coursera em Parceria com o Google. Seu objetivo é aplicar os conhecimentos em Análise de Dados promovidos pelo curso e trabalhar em um projeto desde a confecção do problema de negócio até a apresentação dos resultados para os tomadores de decisão.
Nossa fonte de dados principal é o registro de todas as viagens de bicicletas feitas pelos nossos clientes em um período de 12 meses, iniciando no dia 1 de julho de 2021 e terminando no dia 30 de junho de 2022. 

## Problema de negócio:
Nesse projeto, vamos supor que trabalhamos para uma empresa de aluguel de bicicletas em Chicago, que tem um modelo de negócio muito parecido com as “bicicletas do Itaú”. No nosso caso, a empresa tem dois tipos de assinatura: a casual, em que o cliente paga para utilizar a bicicleta por uma viagem ou por um dia completo, e a anual, em que o cliente assina o serviço por um ano, podendo utilizar as bicicletas sempre que quiser. 
Um dos diretores acredita que a saúde financeira da empresa depende da maximização do número de clientes que assinam o plano anual. Como se sabe, muitas empresas que prestam serviços estão adotando um modelo de negócio por assinatura ao invés de vender um serviço uma única vez, já que isso gera uma receita constante e mais previsível, reduzindo riscos. Por esse motivo, ***o objetivo desse projeto é converter os usuários casuais em usuários anuais, assegurando uma maior consistência nas receitas da empresa.***

***A parte do nosso trabalho como o analista de dados do time é compreender as diferenças de comportamento entre os usuários casuais e anuais.*** O nosso gerente nos avisou que os resultados das nossas análises serão utilizados para orientar as campanhas de marketing, já que se conhecermos melhor o comportamento de nossos clientes, podemos fazer uma campanha mais personalizada e eficaz. Nosso gerente pediu-nos também para ficarmos atentos à outras informações presentes nos dados que possam ser interessantes para a nossa campanha de marketing.

## Resultados

Fomos capazes de chegar a algumas conclusões importantes para a resolução do nosso problema de negócio:

1- A tese do gerente de marketing pode ser fundamentada nos dados disponíveis, pela seguinte razão: durante o inverno o número de viagens de bicicleta cai drasticamente. Isso significa que os clientes que não assinam o plano anual param de gerar receita para a empresa. Se conseguirmos converter esses clientes casuais para clientes anuais, teremos uma maior receita nos meses frios e uma receita mais constante ao longo do ano.

2- Os clientes casuais e anuais de fato apresentam um comportamento diferente. Diversas relações encontradas, como a diferença da quantidade do tipo de cliente por dia da semana, por hora de uso e pelo tempo que cada bicicleta é utilizada fortalece a hipótese de que ***os membros anuais utilizam mais as bicicletas como um meio de transporte, enquanto os membros casuais utilizam mais as bicicletas como um meio de lazer.***

3- A vasta maioria das viagens se concentram nas regiões denominadas "Central" e "North Side". Além do fato dessas regiões serem densamente povoadas, o que justifica um maior número de viagens, chama a atenção o fato dessas também serem ***as duas regiões mais ricas da cidade de Chicago.*** Isso poderia significar que nossos clientes tem menor sensibilidade ao preço. Essa é apenas uma hipótese, já que ela ***não pode ser sustentada com os dados que temos disponíveis***.

## Ressalva: confiabilidade dos dados
Durante a análise ficou claro que os dados apresentam inconsistências. É importante notar a diferença entre dados impróprios para a realização de uma análise específica, e dados intrinsicamente inconsistentes. No primeiro caso, é trabalho do analista tratar os dados para que fiquem adequados para a análise, o que não é um problema. Todavia, no segundo caso é válido questionar se aqueles dados foram coletados de forma correta. Caso eles estejam incorretos, todo o projeto será comprometido. Alguns dos problemas que tivemos foram: 1- mais de um milhão de registros com dados de geolocalização prejudicados; 2- inconsistência no número de ID de estações e nome das respectivas estações); 3- tempos de viagens negativos (o fim da viagem acontecendo antes do seu próprio início); 4- viagens extremamente longas (a mais longa nos registros teria durado 34 dias), dentre outros problemas menores.
Ainda com todas essas ressalvas, o trabalho de análise foi feito, os problemas foram detectados e tenho confiança de que se fosse um trabalho real, as conclusões apontariam na direção correta. Todavia, parece haver alguma dificuldade na forma com que a empresa gera e/ou gerencia os seus dados, e seria muito produtivo caso o time de dados, junto com a área de negócios, criassem soluções para atacar esses problemas.
