## Porsche Sales Intelligence

Dashboard interativo desenvolvido em HTML, CSS e JavaScript para explorar uma base de vendas de veículos Porsche. O projeto permite analisar as entregas concluídas, comparar modelos e cidades, acompanhar os anos-modelo e visualizar as formas de pagamento.

Este é um projeto independente de portfólio, sem vínculo oficial com a Porsche. Os dados utilizados são destinados ao exercício e não representam necessariamente informações oficiais da fabricante.

## Dashboard

A interface foi desenvolvida com uma proposta visual inspirada no segmento automotivo premium, utilizando tons escuros, detalhes em vermelho, imagens de veículos e indicadores para facilitar a análise dos dados.

As imagens abaixo são referências visuais utilizadas durante o desenvolvimento do layout.



## Filtros e indicadores

<img width="1024" height="768" alt="image" src="https://github.com/user-attachments/assets/3c63e7f5-6c54-487d-9d5d-0b289bdb36a5" />


## Gráficos e insights

<img width="1280" height="720" alt="Grafico_insights" src="https://github.com/user-attachments/assets/436fd395-63d7-4891-918f-86c48eb36009" />


## Links do projeto

Dashboard publicada: https://evellyrodrigues6-hash.github.io/but_santander_excel_ia_claud_dash_porshe/

Código-fonte HTML: https://github.com/evellyrodrigues6-hash/but_santander_excel_ia_claud_dash_porshe/blob/main/index.html

Repositório: https://github.com/evellyrodrigues6-hash/but_santander_excel_ia_claud_dash_porshe


## Objetivo da análise

O objetivo foi transformar uma planilha em uma interface que facilitasse a exploração dos dados e a identificação de padrões nas vendas registradas.

## As principais perguntas analisadas foram:

Quantas unidades possuem status de entrega concluída?

Quais cidades apresentam maior volume de entregas?

Quais modelos aparecem com maior frequência entre as entregas?

Qual ano-modelo possui maior representatividade?

Qual é a proporção de registros cancelados?

Quais formas de pagamento aparecem com maior frequência?

Como os modelos se distribuem entre as principais cidades?

As análises foram limitadas aos campos disponíveis na planilha. Como a base não contém informações suficientes sobre custos, margens ou metas, o projeto não busca avaliar lucratividade ou desempenho em relação a objetivos comerciais.

## Funcionalidades

Filtros combináveis por modelo Porsche, Model Year, cidade, forma de pagamento e período da venda.

Indicadores que se atualizam conforme os filtros selecionados.

Comparação de entregas por cidade e modelo.

Distribuição dos registros por ano-modelo e forma de pagamento.

Matriz de modelos por cidade.

Insights calculados com base nos dados filtrados.

Tabela paginada para consulta dos registros.

Exportação dos dados filtrados para CSV.

## Base de dados e tratamento

A fonte utilizada foi uma planilha Excel fornecida para o projeto, na aba Sanitized.

Na verificação inicial, foram identificados os seguintes dados:

100 registros e 12 colunas.

100 valores distintos na coluna sale_id.

40 modelos de veículos.

79 cidades.

9 formas de pagamento.

Nenhuma linha completamente duplicada identificada.

Nenhum valor ausente nas colunas analisadas.

24 datas com o valor INVALID no campo SaleDateSanitized.

## Regras de negócio

Cada registro foi considerado uma venda ou unidade registrada, pois a base possui um sale_id distinto por linha e não apresenta uma coluna específica de quantidade. Essa é uma premissa adotada para a análise.

O status Delivered foi considerado entrega concluída, enquanto Cancelled representa registros cancelados. Os demais status foram mantidos como etapas operacionais distintas.

As datas inválidas foram desconsideradas nas análises que dependem do período da venda. Esses registros ainda podem ser utilizados em análises que não dependem da data.

O campo Model Year representa o ano-modelo do veículo e não deve ser confundido com o ano em que a venda ocorreu.

Como a moeda dos valores não foi identificada na base, não foi atribuído um símbolo monetário. Também não foram calculadas métricas de custo, margem ou data efetiva de entrega, pois essas informações não estão disponíveis.

Antes da publicação, foram retirados da versão HTML os campos com nomes de clientes e vendedores. A planilha original não deve ser disponibilizada publicamente sem a verificação das permissões de uso e da presença de informações pessoais.

## Desenvolvimento do projeto

O desenvolvimento foi realizado em etapas. Primeiro, foram analisadas a estrutura da planilha, a qualidade dos dados e as regras dos indicadores. Em seguida, foram implementados os filtros, os KPIs, os gráficos e a tabela de consulta.

Na etapa visual, foram ajustadas a paleta de cores, a hierarquia dos indicadores, as imagens automotivas e a área de resumo executivo. O objetivo foi tornar a navegação mais clara e facilitar a interpretação dos resultados.

O ChatGPT foi utilizado como apoio na elaboração e revisão do HTML, CSS e JavaScript, na organização visual e na definição das regras de análise. As decisões sobre os indicadores e o tratamento dos dados foram ajustadas de acordo com as características da planilha.

## Tecnologias utilizadas

HTML5: estrutura da página.

CSS3: estilos, layout e responsividade.

JavaScript: filtros, indicadores, gráficos e interações.

Excel: fonte dos dados.

ChatGPT: apoio durante o desenvolvimento.

## Próximas melhorias

Validar todas as interações na versão publicada.

Adicionar testes para os filtros e indicadores.

Melhorar a apresentação dos resultados em telas menores.

Documentar eventuais limitações identificadas durante os testes.

Projeto de portfólio desenvolvido para praticar análise de dados, definição de regras de negócio e criação de dashboards interativos.
