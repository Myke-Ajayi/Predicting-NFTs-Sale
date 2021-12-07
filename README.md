# Predicting_Nfts_sales
![nft2](https://user-images.githubusercontent.com/84211426/144865210-fcce9d11-eca6-4313-a137-785f061311a3.jpeg)

### Overview
What’s an NFT? An NFT is a unit of data stored on a blockchain that certifies a digital asset to be unique and therefore not interchangeable. The first popular example of NFTs is CryptoKitties, a collection of artistic images representing virtual cats that are used in a game on Ethereum that allows players to purchase, collect, breed, and sell them on Ethereum.

OpenSea is the largest marketplace for NFTs and, actually, acts as a 'marketplace for marketplaces'. Using their API, was able to gather about 44,000 data from 2018 to 2021. Then engineer the columns for the target class using the combination of the number of sales; sell orders and the lastsale.eventtype (all these are columns within the data). 
Using this, we want to be able to predict if the model sells or not 
##### Data Source: https://docs.opensea.io/reference/api-overview

### Methodology

- The first step was the data gathering stage [Nft_data_gathering.ipynb](Nft_data_gathering.ipynb)
- The next step was analysing the data and checking the data gathered for hidden information. [NFT_analysis.ipynb](NFT_analysis.ipynb)
- Then this step was processing the data and building models. [Preprocessing.ipynb](Preprocessing.ipynb)

### Structure

├── csv-files                           <- Data gathered and used for the project
├── models                              <- The pickled models for deployment.
├── notebooks
│   ├── NFT_analysis                    <- Analysis of the data
│   ├── Nft_data_gathering.ipynb        <- Intermediate data that has been transformed.
│   ├── Preprocessing.ipynb             <- The final, canonical data sets for modeling.
│   
├── README.md                           <- Summary of the project
│
├── environment.yml                     <- List of all libraries used for building this project
├── models                              <- The pickled models for deployment.
├── nft_project.ipynb                   <- Overview of all information about the project
├── presentation                        <- The prestation to the stakeholers.


### Author
Michael Boluro-Ajayi
