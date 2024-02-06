# Desafio_Cientista_de_Dados

O desafio proposto envolveu a participação em um processo seletivo, no qual de maneira ficticia tive que integrar um time dedicado à criação de uma plataforma de aluguéis temporários em Nova York. Com a finalidade de fundamentar a estratégia de precificação para o cliente, alocaram-me na tarefa específica de realizar uma análise exploratória dos dados referentes ao maior concorrente da plataforma. Além disso, a responsabilidade incluiu a execução de um teste de validação para um modelo preditivo.


## 🚀 Começo

Estas instruções permitirão que você acesse um ambiente virtual do projeto no google colab para fins de execução do funcionamento do modelo e visualização da análise exploratória dos dados (EDA) .

### 📋 Pré requisitos

Antes de começar, você precisará ter acesso as seguintes ferramentas:
- [Git](https://git-scm.com).
- [GoogleColab](https://www.python.org/).

### 🎲 Passo a passo para executar o projeto:

```bash
# Clone o repositorio
$ git clone https://github.com/ArthurSilva707/Desafio_Cientista_de_Dados.git
```

#### Após clonar o repósitorio acesse o seguinte link:

1. [Desafio Cientista de Dados](https://colab.research.google.com/drive/10Zm2IH0ngJV8cxaeB-PAc177nc40krAy?usp=sharing)
    - Atente-se que o link está em modo leitor
2.  Adicione a base de dados ao ambiente
    - Acesse a pasta onde o repósitorio foi clonado encontre o arquivo chamado 'teste_indicium_precificacao.csv' e importe para os arquivos do Google Colab 
    - ![Adicionar arquivos](https://i.imgur.com/gLx2clt.png)
    - Aguarde a base dados carregar inteira para seguir os próximos passos
3. Execute todos os códigos
    - Ambiente de Execução > Executar tudo
    - ![Executar tudo](https://i.imgur.com/VVD723w.png)
4. Após todos os códigos serem executados com sucesso esse deve ser o resultado da aba de arquivos do seu Colab
   - ![Resultado final](https://i.imgur.com/X4Hxm3a.png)


## O presente projeto teve como propósito responder às seguintes questões: 


1. Supondo que uma pessoa esteja pensando em investir em um apartamento para alugar na plataforma, onde seria mais indicada a compra?

- R: levando em considerações o quanto a pessoa estiver disposto a pagar, os alugueis possuem uma média de $ 152.72. tem uma tendência de preços mais altos quando se passa a analizar apartamentos localizados em Manhattan e no Brooklyn e preços mais baixos quando se trata do Queens, Staten Island e Bronx. 
. 

2. O número mínimo de noites e a disponibilidade ao longo do ano interferem no preço?

- R: Chegam a variar em torno de $ 10-20, assim como também têm a influência do local em que o apartamento se encontra 


3. Existe algum padrão no texto do nome do local para lugares de mais alto valor?

- R: Sim, tem uma tendência de preços mais altos quando se passa a analizar apartamentos localizados em Manhattan e no Brooklyn e também para o tipo de espaço de cada anúncio(room_type).


4. Explique como você faria a previsão do preço a partir dos dados. Quais variáveis e/ou suas transformações você utilizou e por quê? Qual tipo de problema estamos resolvendo (regressão, classificação)? Qual modelo melhor se aproxima dos dados e quais seus prós e contras? Qual medida de performance do modelo foi escolhida e por quê?

- R: 
Para a previsão do preço a partir dos dados, aqui estão os passos que eu segui:
 - Tratamento dos dados: identifiquei tipos dos dados, correlações, outliers, exclui valores faltantes/nulos
 - Seleção de Variáveis: considerei variáveis que intuitivamente têm uma relação com o preço, como 'minimo_noites', 'numero_de_reviews', 'reviews_por_mes' e 'disponibilidade_365'.
 - Tipo de Problema: regressão, pois queremos prever um valor contínuo (o preço) com base em variáveis de entrada.
 - Escolha do Modelo: utilizei modelos de regressão linear, como o Linear Regression, para estabelecer uma linha base.
 - Métrica de Avaliação: Erro Médio Quadrático (MSE) é uma métrica comum, que mede a média dos quadrados dos erros entre os valores previstos e os reais. também foi o tipo de métrica que utilizei por mais tempo na faculdade e essa proximidade influênciou na minha escolha.

5. Supondo um apartamento com as seguintes características:
   
    ```bash
    {
    'id': 2595,
    'nome': 'Skylit Midtown Castle',
    'host_id': 2845,
    'host_name': 'Jennifer',
    'bairro_group': 'Manhattan',
    'bairro': 'Midtown',
    'latitude': 40.75362,
    'longitude': -73.98377,
    'room_type': 'Entire home/apt',
    'price': 225,
    'minimo_noites': 1,
    'numero_de_reviews': 45,
    'ultima_review': '2019-05-21',
    'reviews_por_mes': 0.38,
    'calculado_host_listings_count': 2,
    'disponibilidade_365': 355
    }
    ```

    Qual seria a sua sugestão de preço?

- R: baseado no meu modélo minha sugestão seria $175.65, apesar do valor desse apartamento estar por $225 de acordo com a base de dados, valores acima de $175 são minórias e isso foi considerado no modelo.


## 🛠️ built with
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" width="40" height="40" /> 
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/google/google-original.svg" width="40" height="40" />
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/git/git-original.svg" width="40" height="40" />
          
