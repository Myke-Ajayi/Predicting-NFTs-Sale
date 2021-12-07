# Predicting_Nfts_sales
![nft2](https://user-images.githubusercontent.com/84211426/144865210-fcce9d11-eca6-4313-a137-785f061311a3.jpeg)

### Overview
What’s an NFT? An NFT is a unit of data stored on a blockchain that certifies a digital asset to be unique and therefore not interchangeable. The first popular example of NFTs is CryptoKitties, a collection of artistic images representing virtual cats that are used in a game on Ethereum that allows players to purchase, collect, breed, and sell them on Ethereum. In 2017, the market capitalisation of NFTs is $30 miillion and as at this writing December 2021 [according to business insider JP Morgan value NFT at $7 billion](https://markets.businessinsider.com/news/currencies/nft-market-worth-7-billion-legal-issues-could-hinder-growth-2021-11#:~:text=to%20BI%20Prime-,The%20NFT%20market%20is%20now%20worth%20more%20than%20%247%20billion,hinder%20its%20growth%2C%20JPMorgan%20says&text=A%20recent%20boom%20in%20NFT,%247%20billion%2C%20according%20to%20JPMorgan)

### Methodology

- The first step was the data gathering stage [Nft_data_gathering.ipynb](Nft_data_gathering.ipynb)
- The next step was analysing the data and checking the data gathered for hidden information. [NFT_analysis.ipynb](NFT_analysis.ipynb)
- Then this step was processing the data and building models. [Preprocessing.ipynb](Preprocessing.ipynb)

### Motivation

The data for this project was gathered from OpenSea. OpenSea is the largest marketplace for NFTs and, actually, acts as a 'marketplace for marketplaces'. Using their API, was able to gather about 44,000 data from 2018 to 2021. Then engineer the columns for the target class using the combination of the number of sales; sell orders and the lastsale.eventtype (all these are columns within the data). Since we trying to predict if an NFT wil sell or not, focusing on the sale attributes of the data is the best fit for building a model. 
After evaluating the test data, the best model hs an accuracy score of 95% and has a type I (prediciting the NFT will sell and not sellin) error of 21 values out of 14k values 
##### Data Source: https://docs.opensea.io/reference/api-overview


### Structure

```
├── csv-files                           <- Data gathered and used for the project
├── models                              <- The pickled models for deployment.
├── notebooks
│   ├── NFT_analysis                    <- Analysis of the data
│   ├── Nft_data_gathering.ipynb        <- Intermediate data that has been transformed.
│   ├── Preprocessing.ipynb             <- The final processing of data sets and modeling.
│   
├── README.md                           <- Summary of the project
│
├── environment.yml                     <- List of all libraries used for building this project
├── models                              <- The pickled models for deployment.
├── nft_project.ipynb                   <- Overview of all information about the project
├── presentation                        <- The presentation to the stakeholers.
```

### Author
Michael Boluro-Ajayi
