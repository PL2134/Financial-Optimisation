## Summary of Findings

1. Why do people invest in the housing market above other forms of investment? Another question that the group found of interest was why do people invest in the housing market above other forms of investments? 

   Through research into the benefits of investing in the real estate market above other types of investments, we found that everyday investors wanted a steady cash flow and - unlike typical stock dividends- real estate provides a monthly contribution to total income. It protects against inflation - when prices of goods go up, so do rents. Real estate also presents a profitable investment that appreciates over time. However, typical investors are also frightened of the lack of liquidity compared to other financial assets, such as stocks. For this reason, people invest in the housing market above other forms of investment.

   

2. What assets best represent typical investment portfolios?

   When starting our research, we wanted to ensure that we found data that best symbolises what the average investor was investing in. 
   We found that the ordinary investor typically invested in the following:

    - Real estate (represented in our portfolio by the ETF Vanguard Real Estate Index Fund to be referred to as “VNQ”). 
    - Bonds (seen in our portfolio as the ETF, iShares Core US Aggregate Bond to be referred to as “AGG”) 
    - Commodity (depicted in our portfolio as “GLD” a financial asset that gives its investors access to the gold market). 
    - Shares within the stock exchange (in our project represented by the S&P 500 ETF, “SPY”). 

   Thus providing an asset that best represents the common investment portfolio in a satisfactory way. 



3. Is real estate a good asset against inflation?

   Our initial theory that Real Estate is a good asset against inflation is not true. 

   The code downloads the data of 4 portfolios - AGG (Treasury Bonds ETF), VNQ (Real Estate), GLD (Gold) and SPY (S&P 500) and performs thorough data analysis, after which, we found that S&P 500 is the best performing asset for investment for the risk-seeking investors with the highest Sharpe ratio followed by Gold.

   Our data analysis also concluded that Real Estate and Bonds are not good investment. Especially the bonds, as it could not even give us a return that could make up for the growth in the price of goods due to inflation.
   
   In addition, if an investor is considering both risk and return, we will recommend a diversified portfolio, which contains all four assets mentioned above, each weights 25%.

## Introduction

The code performs data analysis on 4 portfolios : US Aggregated Bonds ETF (AGG), Real Estate (VNQ), GOLD (GLD) and S&P 500 (SPY). 

The code performs the following data analysis..

 - Uses Alpaca API to download the last 6 years of data of all the above said portfolios in the form of CSV
 - Download the Risk Free Rate data in the form of CSV using Nasdaq API
 - Converts the CSVs into Dataframes using Pandas
 - Cleans up the dataframes and concatenates all the dataframes
 - Performs following data analysis to identify the best performing financial asset
	- Calculates daily returns
	- Generat 20,50 and 200 days Moving Averages
	- Calculate annulaized mean, annualized standard deviation
	- Calculate rolling variance and rolling covariance of all the portfolios against S&P 500
	- Calculate Sharpe Ratio
	- Generate Monte Carlo Simulation for next 10 years

## Development

This code is built in Jupyter notebook. The process must be pretty much same when executing from GitBash on WindowsPC. If you are using VSCode then the required extensions/modules can be installed from VSCode GUI. To ensure, a suitable environment is existing to execute this code, you will need to have python3 and pip3 installed already. The Python version used to write this code is 3.10.6, any verison older than version 3 might not work efficiently.

## Dependencies

Apart from python3 and pip3, you will need to have jupyterlab, conda, anaconda, pandas, numpy and matplotlib installed at the operating system level.
The code is heavily dependent on pandas, numpy,hvplot, alpaca_trade_api, nasdaq, python-dotenv and matplotlib modules.

Following modules must be already installed before running the code and conda environment must be activated as well. To execute the code, Jupyter notebook must be used. 

Below commands are Mac compatible to install required modules/tools.

As mentioned above ensure python3 and pip3 are already installed - preferrable version 3

	Install Jupyterlab

		pip3 install jupyterlab

	Install conda..

		pip3 install conda or brew install conda

	Install matplotlib..

		pip3 install matplotlib

	Install anaconda3..

		pip3 install anaconda3
	
	Install python-dotenv module..

		python3 -m pip3 install python-dotenv

	Install alpaca-trade-api.. 

		pip3 install alpaca_trade_api

	Install hvplot..

		conda install hvplot

	Install nasdaq-data-link

		pip3 install nasdaq-data-link

## Execution steps

To successfully execute the code...

conda environment must be created and activated.

	conda create -n cenv python=3.10.6
	conda activate cenv

To execute the code from Windows - you will need Visual Studio Code installed as well to look at the code.

The file 'project_one_final_05112022.ipynb' is the file to be opened from the 'Jupyter notebook' interface ONLY.

Clone the directory which contains all the .csv files and the .ipynb file to your system using the following commands

	git clone https://github.com/PL2134/group_3_project_1.git 

Once the clone completes.. 

	Go to the directory "group_3_project_1"

	cd group_3_project_1

Execute 'Jupyter notebook' command

In the Jupyter notebook interface, open the file 'project_one_final.ipynb'




