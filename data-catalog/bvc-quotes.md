---
datapackage:
  title: Historical stock price data from Bolsa de Valores de Cabo Verde
  description: Historical quotes from the Bolsa de Valores de Cabo Verde (BVC).  
  created: 2022-03-15
  updated: 2024-07-10
  sources:
  - path: https://bvc.cv/pagina/historico-cotacoes-bvc-62
    title: Link to data source
  licenses:
  - path: http://opendatacommons.org/licenses/pddl/
    title: Open Data Commons Public Domain Dedication and License v1.0
  resources:
  - name: bvc_quotes_history
    title: Bolsa de Valores de Cabo Verde stock prices
    description: Historical quotes from the Bolsa de Valores de Cabo Verde (BVC).
    lastModified: 2024-07-11
    path: ./data/bvc_quotes_history.csv

---

## Banco Comercial do Atlântico (BCA) stock price overtime

<PlotlyLineChart
  data={{
    url: 'https://raw.githubusercontent.com/AlvaroLima/bvc-quotes/main/data/bca_quotes_history.csv'
  }}
  title="BCA Stock Price x Year"
  xAxis="dates"
  yAxis="preco_fecho"
/>

## Caixa Económica de Cabo Verde (CAIXA) stock price overtime

<PlotlyLineChart
  data={{
    url: 'https://raw.githubusercontent.com/AlvaroLima/bvc-quotes/main/data/caixa_quotes_history.csv'
  }}
  title="CAIXA Stock Price x Year"
  xAxis="dates"
  yAxis="preco_fecho"
/>

## Enacol (ENA) stock price overtime

<PlotlyLineChart
  data={{
    url: 'https://raw.githubusercontent.com/AlvaroLima/bvc-quotes/main/data/ena_quotes_history.csv'
  }}
  title="ENA Stock Price x Year"
  xAxis="dates"
  yAxis="preco_fecho"
/>

## Sociedade Cabo-verdiana de Tabacos (SCT)

<PlotlyLineChart
  data={{
    url: 'https://raw.githubusercontent.com/AlvaroLima/bvc-quotes/main/data/sct_quotes_history.csv'
  }}
  title="SCT Stock Price x Year"
  xAxis="dates"
  yAxis="preco_fecho"
/>