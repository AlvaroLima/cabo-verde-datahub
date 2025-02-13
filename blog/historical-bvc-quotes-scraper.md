# Historical BVC Quotes Scraper

This is my web scraper designed to extract historical quotes from the Bolsa de Valores de Cabo Verde (BVC) website. The scraper is implemented in a Jupyter Notebook using BeautifulSoup4, requests to gather data and pandas for data manipulation and analysis.

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/AlvaroLima/bvc-quotes.git 
    cd historical-bvc-quotes-scraper
    ```

2. Create a virtual environment and activate it:

    ```bash
    python3 -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. Install the required packages:

    ```bash
    pip install -r requirements.txt
    ```

## Usage

To run the scraper, open the Jupyter Notebook [bvc_scraper.ipynb](https://github.com/AlvaroLima/bvc-quotes/blob/main/main.ipynb) and execute the cells. The notebook will scrape the historical quotes data, clean it, and perform some basic exploratory data analysis.


## Data Storage
The cleaned data is saved to a CSV file in the data folder for future analysis.

## Download Dataset
You can download the entire dataset [here](https://r2.datahub.io/clyf18epi0000mc0dblub9man/main/raw/data-catalog/data/bvc_quotes_history.csv)

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

## License
This project is licensed under the MIT License. See the LICENSE file for details.

## Unlocking Cape Verde Stock Market Insights with Python and Tableau: An Ongoing Journey

Since January 2022, I've been leveraging Python and Tableau to scrape and analyze almost 20 years of data from the Cape Verdean stock market. This ongoing project has been updated weekly to ensure the most current insights, helping to visualize trends and make informed investment decisions.

Using Python's BeautifulSoup library, I was able to efficiently and ethically scrape and parse the data from  [www.bvc.cv](http://www.bvc.cv/), converting it into manageable DataFrames with the Pandas library. This included key columns such as entity names, closing prices, and dates. Here's a glimpse of the DataFrame structure:

```\
<class 'pandas.core.frame.DataFrame'>\
RangeIndex: 816 entries, 0 to 815\
Data columns (total 3 columns):\
#  Column      Non-Null Count Dtype\
--- ------      -------------- -----\
0  entidade    816 non-null   object\
1  preco_fecho 816 non-null   float64\
2  dates       816 non-null   datetime64[ns]\
dtypes: datetime64 , float64(1), object(1)\
memory usage: 19.2+ KB\
```

This data, which includes the closing prices of various stocks over time, was saved to a .csv file for further analysis.

The next step was importing the .csv file to Tableau and designing a dashboard to provide a comprehensive visualization of the stock market's evolution since 2005 up to today. This interactive dashboard helps identify trends and patterns, allows users to focus their analysis on a certain date range, chose which entities to display and overall empowers users to make smarter investment decisions.

Stay tuned for Part Two, where I will discuss how is used this information to make informed decisions and the insights gained from this analysis.

Feel free to check out the dashboard and explore the insights it offers and I I'll be happy to answer any questions you may have in the comments.

View the [dashboard here](https://public.tableau.com/app/profile/.lvaro.lima/viz/HistricodeCotaesBVC/Dashboard1)

Check out my design portfolio here [alvaro-lima.com](https://alvaro-lima.com/) .

![Histórico de Cotações BVC por Álvaro Lima](https://media.licdn.com/dms/image/D4E22AQGjscz-2NbnqQ/feedshare-shrink_2048_1536/0/1719231187944?e=1724889600&v=beta&t=3O1Wwjl4XazKmkQZmyzcKmozv_kEtVWbfQH7iAd0kYg)

** Disclaimer: ** This post is not intended to offer financial advice. It is for informational purposes only, focusing on the technologies used in the project.


