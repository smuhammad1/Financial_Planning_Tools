# Financial_Planning_Tools

<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#installation-and-technologies">Installation and Technologies</a></li>
         <li><a href="#prerequisites">Prerequisites</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
	<!-- <li><a href="#license">License</a></li> -->
    <li><a href="#contact">Contact</a></li>
    <li><a href="#license">License</a></li>
  </ol>
</details>

<!-- ABOUT THE PROJECT -->
## About The Project
This is a financial tool to help clients plan for emergencies and for retirement. First, it helps them visualize their current savings to determine if they have enough for an emergency fund. Then, it uses forecast tools to estimate the performance of their portfolios in 10-30 years.

<!-- GETTING STARTED -->
## Getting Started

### Installation
<!-- This is an example of how you may give instructions on setting up your project locally. To get a local copy up and running follow these simple example steps. -->

This project uses Jupyter Notebook (within [JupyterLab](https://jupyterlab.readthedocs.io/en/stable/)) and the standard Python 3.8 libraries. In addition, this project requires the following libraries and/or dependencies:

* [Pandas](https://pandas.pydata.org/) - a software library designed for open source data analysis and manipulation

* [matplotlib](https://matplotlib.org/) - a cross-platform, data visualization and graphical plotting library for Python and its numerical extension NumPy

* [os](https://docs.python.org/3/library/os.html) - provides a portable way of using operating system dependent functionality 

* [requests](https://docs.python-requests.org/en/latest/) - allows you to send HTTP/1.1 requests extremely easily. There’s no need to manually add query strings to your URLs, or to form-encode your POST data. Keep-alive and HTTP connection pooling are 100% automatic

* [json](https://docs.python.org/3/library/json.html) - stands for JavaScript Object Notation. JSON is a lightweight data format used for data interchange between multiple different languages. It is easy to read for humans and easily parsed by machines

* [dotenv](https://pypi.org/project/python-dotenv/) - reads key-value pairs from a .env file and can set them as environment variables

* [alpaca_trade_api](https://pythonrepo.com/repo/alpacahq-alpaca-trade-api-python-python-third-party-apis-wrappers) - a python library for the Alpaca Commission Free Trading API. It allows rapid trading algo development easily, with support for both REST and streaming data interfaces

* MCForecastTools - the document named "MCForecastTools.py" contains the code functions needed to run the Monte Carlo Simulations (MCSimulation) used in this project

* All stock and bond data was pulled in using Alpaca API calls to the Alpaca SDK. The ETH and BTC data were pulled in using the Requests library from the following links: [btc_url]("https://api.alternative.me/v2/ticker/Bitcoin/?convert=USD"), [eth_url]("https://api.alternative.me/v2/ticker/Ethereum/?convert=USD")

### Prerequisites
```
import os
import requests
import json
import pandas as pd
from dotenv import load_dotenv
import alpaca_trade_api as tradeapi
from MCForecastTools import MCSimulation
%matplotlib inline
```
---

## Usage

To run this application, create a clone on the local desktop. Then, initiate your conda environment and 
open ```jupyter lab --ContentsManager.allow=hidden=True```. Now, you can run the notebook in jupyter lab and 
read hidden file with alpaca keys.

Steps for running application:

1st. Create a Financial Planner for Emergencies

    * Evaluate Crypto assets via Requests
    * Evaluate Stocks/Bonds portfolio using Alpaca SDK
    * Evaluate Emergency Fund


2nd. Create a Financial Planner for Retirement

    * Create Monte Carlo Simulation
    * Analyze Retirement Portfolio Forecasts

3rd. Review 30 year and 10 year Monte Carlo Simulations for stock and bonds porfolio: 
    
    * evaluate how the stocks/bonds porfolio values react relative to time and diversification.
    

The images below illustrates the results of the 30 year Monte Carlo simulations results:

<img width="467" alt="Screen Shot 2022-02-06 at 10 00 17 AM" src="https://user-images.githubusercontent.com/93550651/152694609-3ca905d7-e52b-4215-835d-b6f89bd38ba3.png">

<img width="515" alt="Screen Shot 2022-02-06 at 10 00 40 AM" src="https://user-images.githubusercontent.com/93550651/152694621-6b343815-9cc7-45bb-8ae2-7012080c1a3c.png">


<!-- CONTACT -->
## Contact

Sumayyah Muhammad - [@somayaann][linkedin-url] - sumayyahmuhammadts@gmail.com

Project Link: [https://github.com/smuhammad1/Financial_Planning_Tools]

<!-- LISCENSE -->
## License

MIT



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/smuhammad1/loan_qualifier_application.svg?style=for-the-badge
[contributors-url]: https://github.com/smuhammad1/loan_qualifier_application/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/smuhammad1/loan_qualifier_application.svg?style=for-the-badge
[forks-url]: https://github.com/smuhammad1/loan_qualifier_application/network/members
[stars-shield]: https://img.shields.io/github/stars/smuhammad1/loan_qualifier_application.svg?style=for-the-badge
[stars-url]: https://github.com/smuhammad1/loan_qualifier_application/stargazers
[issues-shield]: https://img.shields.io/github/issues/smuhammad1/loan_qualifier_application/network/members?style=for-the-badge
[issues-url]: https://github.com/smuhammad1/loan_qualifier_application/issues
<!-- [license-shield]: 
[license-url]:  -->
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/sumayyahmuhammadofficial/