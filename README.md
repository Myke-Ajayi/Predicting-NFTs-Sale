# Predicting_NFTs_sales
![nft2](https://user-images.githubusercontent.com/84211426/144865210-fcce9d11-eca6-4313-a137-785f061311a3.jpeg)

### Overview
What’s an NFT? An NFT is a unit of data stored on a blockchain that certifies a digital asset to be unique and therefore not interchangeable. The first popular example of NFTs is CryptoKitties, a collection of artistic images representing virtual cats that are used in a game on Ethereum that allows players to purchase, collect, breed, and sell them on Ethereum. In 2017, the market capitalisation of NFTs is $30 miillion and as at this writing December 2021 [according to business insider JP Morgan value NFT at $7 billion](https://markets.businessinsider.com/news/currencies/nft-market-worth-7-billion-legal-issues-could-hinder-growth-2021-11#:~:text=to%20BI%20Prime-,The%20NFT%20market%20is%20now%20worth%20more%20than%20%247%20billion,hinder%20its%20growth%2C%20JPMorgan%20says&text=A%20recent%20boom%20in%20NFT,%247%20billion%2C%20according%20to%20JPMorgan)

### Methodology

- The first step was the data gathering stage [Nft_data_gathering.ipynb](Nft_data_gathering.ipynb)
- The next step was analysing the data and checking the data gathered for hidden information. [NFT_analysis.ipynb](NFT_analysis.ipynb)
- Then this step was processing the data and building models. [Preprocessing.ipynb](Preprocessing.ipynb)

### Motivation

The data for this project was gathered from OpenSea. OpenSea is the largest marketplace for NFTs and, actually, acts as a 'marketplace for marketplaces'. Using their API, was able to gather about 44,000 data from 2018 to 2021. Then engineer the columns for the target class using the combination of the number of sales; sell orders and the lastsale.eventtype (all these are columns within the data). Since we trying to predict if an NFT wil sell or not, focusing on the sale attributes of the data is the best fit for building a model. 

The main challenges in the NFT space is increased supply and minting fees. When creating NFTs there is an average of about 70 to $600 of minting fees. And an additional charge for storing on the block chain. This adds up on the creator. Also, to add to it due to increased supply majority of these NFTs do not sell; causing an expense for the creators. Using this model, will be able to predict if an NFT will sell or not before spending money and time. 
##### Data Source: https://docs.opensea.io/reference/api-overview

### Results 

The best model is a Decision Tree model with an accuracy score of 95% and a precision score of 96%. The model as a type I error (prediciting the NFT will sell and not selling) of 103 values out of 14k tokens. And a type II error of 26 values out of 14k tokens i.e predicting it will not sell and actually selling which is a good thing to the seller.
![confusion matrix](https://user-images.githubusercontent.com/84211426/145226678-a04bd223-1f6e-4de6-8fb4-28d0f6db4e7b.png)

From the model, was able to extract the most important features to pay attention to. 
![feature importance](https://user-images.githubusercontent.com/84211426/145229052-8d2d0363-9f5d-495f-ad31-91fa1120bc61.png)


### Recommendation
The most important is to improve on older artworks, the older the NFT the more likely is to sell. Also, utilise social media to create fanbase cause the bigger the fanbase the more likely tokens are sold.

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
