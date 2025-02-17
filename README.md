# Blockchain-Based-Property-Registration

<a href="LICENSE"><img src="https://img.shields.io/static/v1?label=license&message=MIT&color=green"></a>
<img src="https://img.shields.io/badge/Ethereum-20232A?style=for-the-badge&logo=ethereum&logoColor=white">
<img src="https://img.shields.io/badge/Flutter-%2302569B.svg?style=for-the-badge&logo=Flutter&logoColor=white">
## Land Registration using Blockchain
## Problem it Solves:
1. The elimination of middlemen: The elimination of middlemen or brokers makes the process of land registration less expensive. Brokers who try to defraud uninformed people will be unable to do so any longer. Brokers frequently take a long time to finish procedures, thus our project will help people save time.
3. A distributed tamper-proof ledger that prohibits ownership fraud.
4. IPFS is used to store important property registration papers in a secure manner.

## Technology Stack:
1. Ethereum Blockchain
2. Polygon/Matic
3. Web3Dart
4. IPFS
5. Flutter
6. Metamask

#### Check new Smart contract At Polygon Testnet: [here](https://mumbai.polygonscan.com/address/0xbc6d9e15255533C19f1589A7e9fbB60440a539e0)

#### Check Smart contract At (discontinued) Ropsten Ethereum Testnet: [here](https://ropsten.etherscan.io/address/0x702058ba021cd4e4f847b40f32b58aa5be3a4661)

## To Run Application Locally
1. Clone the github repository and cd to the folder
2. Install the flutter 3.0.2, nodejs
3. Install ganache and truffle as shown below:
```
npm install -g truffle
```
4. Open Ganache and keep it running in the Background
5. Install the Metamask chrome extension, choose the local network and import the accounts
6. Compile and run our migrations from the command line as shown below:
```
truffle compile
truffle migrate
```
7. Copy contract address as seen in the image below and paste in variable `contractAddress` located in the file `./lib/constant/constant.dart`
<pre>
2_deploy_migration.js
=====================

   Replacing 'Land'
   ----------------
   > transaction hash:    0x427b2b402f767ac6a90334ab3c687b086b274de747fe10d6e194743b15057d78
   > Blocks: 0            Seconds: 0
   <b>>contract address:    0xed690C24C60A48F8A9819c9A15AD75B70CFBEa5a</b>
   > block number:        3
   > block timestamp:     1650602828
   > account:             0x33e94e4619f0AecDf81e9676Eb82c109FBa53356
   > balance:             99.9154895
   > gas used:            3996227
   > gas price:           20 gwei
   > value sent:          0 ETH
   > total cost:          0.07992454 ETH
</pre>
8. In `constant.dart` file, change the value of the variable `chainId` to `'1337'` and change the value of the variable `rpcUrl` to `"http://127.0.0.1:7545"`
9. Run the flutter web app
```
flutter pub get

flutter run -d web-server --web-port 5555
```
10. Open the browser and the dapp will be running in http://localhost:5555/
11. Create mapbox api key from https://www.mapbox.com/ and Replace it with `mapBoxApiKey`in `constant.dart` file


