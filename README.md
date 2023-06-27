## Consulta das ações que compõem o índice IBRX50

O código desde programa em Python visa obter as ações que compõem o índice IBRX50 de acordo com determinado período de análise desejado.
O índice IBRX50 representa o retorno de uma carteira com as 50 ações mais negociadas no Ibovespa de acordo com critérios específicos que podem ser analisados em maior
detalhe no link da B3: 

https://www.b3.com.br/pt_br/market-data-e-indices/indices/indices-amplos/indice-brasil-50-ibrx-50.htm

### Objetivo e tratamento das informações

O programa utiliza uma automação de Web Scraper (raspagem de tela) que é capaz de obter as informações do site da B3 para compor o índice atual.

É definido um período para consulta dos preços das ações, tanto o preço de fechamento como o ajustado.

Com os dados tabelados, é possível plotar gráficos para ações específicas e analisar a diferença entre os preços e a distribuição de dividendos.

### Tratamento
Com os dados salvos em uma tabela os mesmo são tratadas de modo a preencher valores nulos com uma métodologia específica para que não haja tanto viés no seu preenchimento.
   - O método utilizado é o interpolate da biblioteca pandas e está melhor descrito no código.
### Consulta dos preços
A busca dos preços é feita pela plataforma Yahoo Finance, através da biblioteca yfinance.
### Visualização das informações
São plotados 2 gráficos:
- um das séries temporais com as curvas do preço de fechamento e outro com o preço ajustado
- outro com os valores de dividendos distribuídos por ação para a ação em análise

Por fim, podese-se fazer algumas análises e conclusões sobre a ação em análise para o período escolhido.
