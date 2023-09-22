# Ethereum Crowdfunding Platform

An Ethereum-based crowdfunding platform. This project allows users to fund with ETH, ensuring that they meet a minimum threshold in USD equivalent.

## Features:

- **Crowdfunding with ETH**: Users can send ETH to the platform.
- **USD Threshold**: The platform uses the Chainlink price feed to verify if the ETH sent by the user is equivalent to or more than a set minimum in USD.
- **Withdraw Funds**: Only the owner of the contract can withdraw the accumulated funds.

## Smart Contracts:

1. **FundMe.sol**: 
   - Main contract for crowdfunding.
   - Uses the `PriceConverter` library to ensure that the ETH sent by the user meets the minimum USD threshold.
   - Provides functionality for the owner to withdraw funds.
2. **PriceConverter.sol**: 
   - A library that provides utility functions to convert ETH amounts to their USD equivalent using the Chainlink price feed.
   - Fetches the latest ETH/USD price and calculates the USD equivalent of a given amount of ETH.

## Dependencies:

- **Chainlink**: Used for fetching the latest ETH to USD conversion rate.

## License:

MIT

