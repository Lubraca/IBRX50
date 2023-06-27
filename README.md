## Query of the stocks that make up the IBRX50 index

The code of this Python program aims to obtain the stocks that make up the IBRX50 index according to a desired analysis period.
The IBRX50 index represents the return of a portfolio consisting of the 50 most traded stocks in the Ibovespa according to specific criteria that can be further analyzed in detail at the B3 link:

https://www.b3.com.br/pt_br/market-data-e-indices/indices/indices-amplos/indice-brasil-50-ibrx-50.htm

### Objective and information handling
The program uses a Web Scraper automation, which is capable of extracting information from the B3 website to compose the current index.

A period is defined to query the stock prices, both the closing price and the adjusted price.

With the tabulated data, it is possible to plot graphs for specific stocks and analyze the price differences and dividend distributions.

### Data Treatment
After saving the data in a table, it is processed to fill in null values using a specific methodology to minimize bias in the filling process.

The method used is the "interpolate" function from the pandas library, and it is further described in the code.

### Obtaining the prices

The price data is retrieved from the Yahoo Finance platform using the yfinance library.

### Information visualization
Two graphs are plotted:

- One shows the time series with the curves of the closing price
- Other shows the adjusted price

Finally, some analysis and conclusions can be drawn regarding the analyzed stock for the chosen period.
