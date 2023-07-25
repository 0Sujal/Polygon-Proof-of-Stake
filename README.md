###Polygon Proof of Stake 
This is the first project in Polygon-Advance, in this project, I was tasked to deploy an NFT collection on the Ethereum blockchain, Map the collection to Polygon, and Transfer assets over via the Polygon Bridge.

in this project, an NFT collection is to be deployed on the goerli network, Map the collection to Polygon, and Transfer assets to mumbai network using Polygon Bridge.

#MY NFT
https://gateway.pinata.cloud/ipfs/QmUrT85Ut7W38GVuJHbxni9FhAwVoQqNYwZoWVHn1AcqCU/
![image](https://github.com/0Sujal/Polygon-Proof-of-Stake/assets/90201074/beb50cce-dd5c-4102-a132-38abde197265)

#Steps involved in program

npm install
Compile the contracts using: npx hardhat compile
Perform test using command : npx hardhat test
Create an environment file .env In this file add PRIVATE_KEY="your wallet private key", GOERLI_URL and MUMBAI_URL
To Deploy ERC721 contract to the Goerli Ethereum Testnet, Execute command: npx hardhat run scripts/deploy.js --network goerli An the address will be generate. Paste this address into contarctAddress.js(in metadata folder) and also in batchMint.js(in scripts folder)
Batch Mint NFTs Run the following command to batch-mint NFTs: npx hardhat run scripts/batchMint.js --network goerli The script will mint the specified number of NFTs and assign them to your address.
Approve and Deposit NFTs to Polygon Mumbai Run the following commands to approve and deposit the minted NFTs from Ethereum to the Polygon Mumbai network using the FxPortal Bridge: npx hardhat run scripts/approveDeposit.js --network goerli
After installing the dependencies, run the test file by using the following command:

npx hardhat test
Deploying the ERC721 Contract
Before deploying, make sure to rename ".env.example" to ".env" and provide your wallet private key where required i.e. "PRIVATE_KEY= 'your wallet private key'". 

#Run the following command to deploy the ERC721 contract to the Goerli Ethereum Testnet:

Batch Mint NFTs
Run the following command to batch-mint NFTs using the deployed ERC721 contract:

npx hardhat run scripts/batchMint.js --network goerli
The script will mint the specified number of NFTs and assign them to your address.

Approve and Deposit NFTs to Polygon Mumbai
Run the following commands to approve and deposit the minted NFTs from Ethereum to the Polygon Mumbai network using the FxPortal Bridge:

npx hardhat run scripts/approveDeposit.js --network goerli

![image](https://github.com/0Sujal/Polygon-Proof-of-Stake/assets/90201074/ccc19d36-015f-440e-b30c-6db6ed50d26b)


after this you can check  your transaction in https://goerli.etherscan.io/

![image](https://github.com/0Sujal/Polygon-Proof-of-Stake/assets/90201074/e10c5c41-1248-45aa-9f2a-68ca518efb58)


Authors Sujal Dua 21BCS5327@cuchd.in

License This project is licensed under the Sujal Dua License - see the LICENSE.md file for details
