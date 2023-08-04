# Stock on You: A Network Analysis of the Top 50 S&P Stocks | Exploring Relationships and Sector Dominance in the Stock Market Landscape

## Author

- [Ma. Lair A. Balogal](https://github.com/lairbally)

## Overview
Stock on You is a data analysis project that explores the relationships and sector dominance among the top 50 S&P stocks with the highest daily returns during the 5-year period from 2013 to 2018. The goal of this project is to gain insights into the complex interconnections between these high-performing stocks and to identify dominant sectors in the stock market landscape.

## Features
- Network analysis of the top 50 S&P stocks with the highest daily returns from 2013 to 2018 to uncover underlying connections.
- Exploration of relationships between individual stocks to reveal patterns and dependencies.
- Identification of dominant sectors within the stock market.

## Data Source
The dataset used in this project contains historical stock prices for all companies currently listed on the S&P 500 index, spanning the 5-year period from 2013 to 2018. The data was sourced from Cam Nugent’s GitHub repository [here](https://github.com/CNuge/kaggle-code).

Each file in the dataset includes the following columns:

- Date: in the format yy-mm-dd
- Open: stock price at market open (all in USD, as this is NYSE data)
- High: highest price reached during the day
- Low: lowest price reached during the day
- Close: closing price
- Volume: number of shares traded
- Name: the stock’s ticker name

For the purpose of exploratory data analysis and to enhance the dataset, sector classification for each S&P company based on The Global Industry Classification Standard (GICS®) was obtained. You can find more information about GICS® [here](https://www.msci.com/our-solutions/indexes/gics).

## Dependencies
To run this project, you will need the following libraries and packages:

- pandas
- numpy
- wordcloud
- matplotlib
- plotly
- Pillow (PIL)
- statsmodels
- tqdm
- networkx
- sklearn
- joblib
- seaborn
- scipy

You can install these dependencies using pip:

```
pip install pandas numpy wordcloud matplotlib plotly Pillow statsmodels tqdm networkx scikit-learn joblib seaborn scipy
```

Please note that some of the dependencies, such as `Pillow` and `scikit-learn`, are sub-packages of the larger libraries `PIL` and `sklearn`, respectively.

In addition to the dependencies, make sure to include the warning filters at the beginning of your Python script or Jupyter Notebook to suppress certain warnings:

```python
import warnings
warnings.filterwarnings("ignore", category=Warning)
warnings.simplefilter(action='ignore', category=FutureWarning)
```

## Usage
To analyze the stock market landscape and explore the relationships among the top 50 S&P stocks with the highest daily returns, follow these steps:

1. Download the dataset from the provided link and extract the `data.rar` file. The dataset should contain the stock data in CSV format and the sector data in XLSX format.
2. Open the `stock_on_you_network_and_gc_analysis.ipynb` Jupyter Notebook.
3. Run the notebook cells sequentially to execute the entire analysis.

## Results and Visualizations
The `stock_on_you_network_and_gc_analysis.ipynb` notebook includes creative visualizations, such as:
- Word Clouds depicting commonly occurring stock names using the `upvote.png` image.
- GIF visualizations for interactive exploration of dynamic stock sector performance plots.

The notebook also presents the results of the analysis, including network graphs showing the relationships between the top 50 S&P stocks, sector-wise stock distribution and dominance visualizations, and various centrality measures.

## Contribution Guidelines
We welcome contributions to this project! If you have any ideas for improvement or new features to add, please feel free to open an issue or submit a pull request. 

## License
This project is licensed under the [MIT License](LICENSE).
