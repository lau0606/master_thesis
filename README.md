# Early Wallet Behavior and Transparency in Meme Coin Markets

This repository contains the full code and data used for the Master's thesis titled *"Early Wallet Behavior and Transparency in Meme Coin Markets"*, submitted in June 2025 at Aalborg University, MSc in Business Data Science.

*Authors*: Magdalena Baran, Laura Kéri, Ilija Koturić  
*Supervisor*: Primoz Konda

## Project Overview

Our thesis investigates  wallet behavior and transparency in the meme coin system with focus on three politically branded tokens on the Solana blockchain: *$TRUMP*, *$MELANIA*, and *$LIBRA*.

We combine:
- *On-chain transaction analysis*: to detect suspicious activity patterns
- *Reddit-based sentiment & topic modeling*: to understand psychological dynamics

A custom suspicion score and behavioral clustering help reveal wallet patterns like sniper activity, wash trading, and market manipulation. Simultaneously, Reddit discussions provide qualitative insights into hype, FOMO, and emotional investment behavior.

## Repository Structure

- requirements.txt: List of Python packages required to run the code
- FOMO_HYPE/: Contains code for detecting FOMO and hype in Reddit discussions
- Reddit_Data/: Includes scraped Reddit threads mentioning $TRUMP, $MELANIA, and $LIBRA, notebooks for downloading and preparing data, merged and cleaned datasets
- topic_modelling/: Topic modelling notebooks for each coin and a summary file of extracted topics
- sentiment_analysis/: Contains sentiment analysis notebooks using VADER and TextBlob
- OnChain_Analysis/: Includes code for building wallet maps and analyzing on-chain behavior (profit, suspicion, and scam detection)

## Methodology Summary

- *Suspicion Score*: Evaluates wallets based on 5 risk indicators (e.g., early entry, high profit, wash trading).
- *Clustering*: KMeans applied to profit and activity metrics to detect trading pattern groups.
- - *Visual Tools*: Interactive Bokeh wallet map color-coded by suspicion, profit, cluster, or scam type.
- *Reddit NLP*:
  - Topic modeling: Using BERTopic for $TRUMP, $MELANIA, and $LIBRA
  - Sentiment analysis: Using VADER and TextBlob
  - FOMO/Hype detection: Based on regex dictionary

## Data Sources

- Solana transaction data from [Pinax via Snowflake](https://app.snowflake.com/marketplace/listing/GZTSZ33VCBM/pinax-solana-raw-blockchain-data)
- Reddit posts and comments from multiple cryptocurrency and finance subreddits
- Token prices retrieved manually from [CoinMarketCap](https://coinmarketcap.com)

## Results

- *Wallet Behavior*: Over 50% of analyzed wallets showed suspicious patterns; few wallets earned the majority of profits.
- *Reddit Analysis*: Topic clusters revealed political cynicism, scam awareness, and FOMO herding behavior.
- *FOMO Trends*: Persisted even after dump phases, indicating strong emotional investment.
- *Transparency Insight*: Despite public data, real-time analysis is practically inaccessible for average investors.


## Thesis

The full thesis is included in the repository or available [here](https://github.com/lau0606/master_thesis/blob/main/EarlyWalletBehaviorandTransparencyinMemeCoinMarkets.pdf).

