#### 1. Introdução
O desafio tem como objetivo ampliar a inteligência de negócios da empresa Melhores Compras, por meio da coleta, organização e apresentação de dados. A proposta se divide em dois desafios principais:

- Modelagem dimensional de dados para análise de estoque.
- Estimativa de custos para armazenamento em nuvem.


#### 2. Primeiro Desafio: Data Mart Estoque

##### 2.1. Perguntas Executivas e Justificativas

- Tempo médio de reposição por categoria de produto: Auxilia no planejamento de compras e evita rupturas no estoque.
- Produtos abaixo do estoque mínimo: Identifica itens frequentemente escassos para otimização da gestão de estoque.
- Taxa de rotatividade do estoque: Permite ajustar o estoque conforme a demanda em diferentes centros de distribuição.
- Valores do estoque nos centros de distribuição: Análise de valores armazenados para otimização e correlação com saídas de produtos.
- Impacto de promoções e eventos sazonais: Identifica padrões de demanda para planejamento eficiente de estoque e vendas.

##### 2.2. Dados Necessários

- Centro de distribuição: Nome, localização, capacidade.
- Produto: Nome, marca, cor, dimensões, SKU.
- Fornecedor: Nome, localização, tempo de entrega, confiabilidade.
- Categoria: Nome, descrição, segmento, subcategoria, prioridade de abastecimento.

##### 2.3. Modelo Dimensional

- Criar um modelo dimensional Star Schema que responda às perguntas executivas.
- Utilizar ferramentas como Oracle SQL Data Modeler (ou similar).
- Entregas esperadas:
    - Modelo dimensional físico em PDF.
    - Scripts DDL para criação e remoção do modelo (cria.sql e apaga.sql).
    - Dicionário de dados detalhado.

#### 3. Segundo Desafio: Calculadora de Preços em Cloud

##### 3.1. Contexto
A empresa deseja estimar o investimento mensal necessário para armazenar seus dados na nuvem. Para isso, será utilizada uma calculadora de preços de provedores cloud.

##### 3.2. Premissas

- Carga de trabalho:
    - 50.000 pedidos diários.
    - 70% dos pedidos têm 1 item; os demais têm 2 itens.

- Infraestrutura necessária:
    - 2 servidores Windows (4 núcleos, 32GB RAM).
    - 4 servidores Linux (4 núcleos, 32GB RAM).

- Dados a serem armazenados:
    - 5TB estruturados (e-commerce, ERP, sistemas legados).
    - 2TB não estruturados (imagens, vídeos, áudio), sendo:
    - 20% em "cold storage".
    - 80% em "hot storage".
    - Crescimento de 30% ao ano.

##### 3.3. Entregas Esperadas
- Selecionar dois provedores de cloud e comparar os custos.
- Planilha Excel com cálculos detalhados (calculo.xls).
- PDF com orçamentos gerados pelas ferramentas dos provedores (orcamentos.pdf).
- Justificativa da escolha do melhor orçamento.

#### 4. Entregas Finais
O material deve ser entregue em um pacote compactado (.zip) contendo:

- Modelo dimensional:
    - modelo-dimensional-fisico.pdf
    - cria.sql
    - apaga.sql
    - dicionario-de-dados.pdf

- Cálculo de cloud:
    - calculo.xls
    - orcamentos.pdf

- Componentes do grupo:
    - componentes.txt (nomes, RMs e integrantes em ordem alfabética).

#### 5. Recomendações Finais

- Testar os scripts DDL antes da entrega.
- Conferir se todos os arquivos estão no pacote para evitar penalização.
- Garantir que os cálculos e modelos estão corretos e bem estruturados.

