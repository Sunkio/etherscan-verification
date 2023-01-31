# Etherscan Verification 
A simple test project to verify smart contracts on Etherscan or Polygonscan

## How to interact with the deployed testnet app
The contract has been deployed to Polygon Mumbai for testing purposes. You can find out more about it [here](). You need test funds to interact with the app. There are several faucets you can use to get Mumbai for free. Here’s one example that has worked well for me in the past: https://mumbaifaucet.com/ 
If you’re brand new to web3: To get started, you first need a wallet such as Metamask to receive testnet funds and start interacting with the app.

## Installing / Getting started with the project
To install this project, you will need to install the necessary dependencies. Once all of the dependencies are installed and you're done editing, you can deploy the smart contract to the (test) net of your choice.

1.) Fork and clone this repository to your local machine
Fork this repo, then clone it to your local machine:
```
git clone https://github.com/YOUR-USERNAME/etherscan-verification
```
2.) Blockchain Part
Run the following commands in your CLI:
```
cd etherscan-verification
npm init --yes
npm install --save-dev hardhat
npx hardhat
npm install dotenv
```
Create an endpoint on QuickNode, or any other provider of your choice, and copy the HTTP-URL. Create a .env file and follow the structure of the .env-example file to add your QuickNode URL, your private key, and your token from a matching blockchain explorer (e.g. Polygonscan or Etherscan). DO NOT upload this file to Git Hub! It is already included in .gitignore but better double-check. slightly_smiling_face

Once you’re done editing, run:
```
npx hardhat compile 
npx hardhat run scripts/deploy.js --network mumbai 
```
## How to Contribute
Contributions are always welcome! Please check the Code of Conduct .

## License
This project is licensed under the MIT License.

## Support
If you have any questions or need help getting started, please open an issue in the repository or contact me on Twitter: @tanja_codes
