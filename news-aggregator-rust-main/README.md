# Cryptocurrency News Aggregator

## Description

Cryptocurrency News Aggregator - is a Rust-based web application that fetches the latest cryptocurrency news and market data from multiple trusted sources. Users can search by cryptocurrency name to get real-time news articles with concise summaries, source info, and publication dates as well as market data such as price and capitalization of the provided currency.

## Key Features

 - Search for cryptocurrency market data

 - Get the latest news related to cryptocurrencies

 - Error handling for missing data or API issues

 - Clean and modern responsive UI

 - Suggests supported cryptocurrencies

# How It Works

1. User enters a cryptocurrency name (e.g., bitcoin) in the search bar.

2. App fetches:

    Market data like price and market cap.

    Latest news articles.

3. Fetched data is displayed on the same page and divided into two following columns:
    - <b> Market Data </b>, where you can find such info as price and market cap. of provided token, 

    - <b> Latest news </b>, where you can find list of related articles and the link to the original source by following <b> Read more </b> button.


# Demo

When you start the application, by default you will be greeted with the following screen:

![Image not available](https://github.com/Timirlon/news-aggregator-rust/blob/main/demo/default-screen.png)

Let's try to type the name of cryptocurrency that we are interested in right in the search bar. We will start with bitcoin:

![Image not available](https://github.com/Timirlon/news-aggregator-rust/blob/main/demo/bitcoin-search.png)

We could also try to type other cryptocurrency names. For example, we provide the meme crypto of Doge Coin, and get the following data:

![Image not available](https://github.com/Timirlon/news-aggregator-rust/blob/main/demo/doge-search.png)

The application also supports the error handling. For instance, if we enter the name of fake or non-existent crypto currency, the application won't be able to fetch any market data due to that and will inform us about that. However, it might still return some news article, because the search of article is conducted based on key words that were provided by user.

![Image not available](https://github.com/Timirlon/news-aggregator-rust/blob/main/demo/search-not-found.png)

## Technologies Used
- Backend: 
  - Rust - programming language

- Frontend: 
  - HTML/CSS + Bootstrap - layout and design
  - JS - scripting


- APIs
  - CoinGecko API
  
    Used to fetch real-time cryptocurrency data such as current price, market capitalization, and token details.

  - GNews API

    Used to fetch recent news articles related to selected cryptocurrencies. Also includes basic date formatting and sentiment tagging.

## Installation

To run this project locally, ensure that you have Rust installed. You can follow the instructions to install Rust [here](https://www.rust-lang.org/learn/get-started).

Additionally, you need "GNEWS_API_KEY" API key variable  placed in your .env file

### Steps to run:

1. Clone the repository:
    ```bash
    git clone https://github.com/XoxoLbel/news-agregator-rust
    cd news-aggregator-rust
    ```

2. Install dependencies:
    ```bash
    cargo build
    ```

3. Run the server:
    ```bash
    cargo run
    ```


## Development Team

- Abdykhalyk Dias SE-2322

## License

This project is designed for academic purposes only and is not intended for commercial use. Licensed under MIT License.
