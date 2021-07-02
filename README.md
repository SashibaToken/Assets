# Sishiba Governance V1: Listing a new asset

This repository facilitates the last step of the process of listing a new asset to the Aave protocol, that is creating the on-chain proposal to the Aave Governance.


## Requirements 

- You must have agreed with the Aave Genesis team on risk parameters for your token during an ARC on the governance forum.
- You must have deployed the AToken, VariableDebtToken, StableDebtToken, InterestStrategy overlying contracts for your token.
- You must have created the associated AIP ([here](https://github.com/aave/aip))
- You must have enough Proposition Power.

## Set the environment variables.

Copy the `.default.env` file, rename it to `.env` and update it to match with your tokens addresses and your risk parameters.

Example for the Curve Token listing: 

```

FORKING_BLOCK=11538355
```
# Node
## Install

`$ npm i`

## Run the test

`$ npm run test`
## Run the deployment script

`$ npm run propose-new-asset:kovan` for kovan

`$ npm run propose-new-asset:main` for mainnet

# docker-compose

In one terminal tab: `docker-compose up`

Enter the container in new tab: `docker-compose exec contracts-env bash`

In the container run: 

`$ npm run test`

`$ npm run propose-new-asset:kovan` for kovan

`$ npm run propose-new-asset:main` for mainnet


