# 😎 Smart Agent. AI image generator app - using Galadriel - the first Layer 1 
![SmartAgent-coverImage](https://github.com/Bild96/Smart-Agent/assets/52472445/8e63a80a-c9d1-4a94-af80-bc754b3e44fb)

<img src="https://img.shields.io/badge/Open%20Source-Yes-cyan?style=flat-square">
<img src="https://img.shields.io/badge/Version-0.1-green?style=for-the-badge"><img src="https://img.shields.io/github/license/bild96/smart-agent?style=for-the-badge&color=blue">


## 🏁 Quickstart
This quickstart covers two things:
* Deploying an AI app to the Galadriel devnet
* Calling your deployed AI app and viewing the results

## 🔥 Prerequisites
 A Galadriel devnet [account](https://docs.galadriel.com/setting-up-a-wallet). We recommend creating a new EVM account for development purposes.
    Some [devnet tokens](https://docs.galadriel.com/faucet) on the account you are using.
    node and npm installed on your machine.

## Deploying a contract on Galadriel devnet:
1. devnet tokens
Get yourself some devnet tokens from the [faucet](https://docs.galadriel.com/faucet).
2. Clone repository
Clone the repo that contains Galadriel example contracts and the oracle implementation.
```
git clone https://github.com/bild96/smart-agent.git
cd smart-agent/contracts
```
3. Setup environment
Use the ||template.env|| file to create a ||.env|| file:
```
# Starting in repo root
cp template.env .env
```
Then, modify the ||.env|| file:
- Set ||PRIVATE_KEY_GALADRIEL|| to the private key of the account you want to use for deploying the contracts to Galadriel devnet.
- Set ||ORACLE_ADDRESS|| to the [current devnet oracle address](https://docs.galadriel.com/oracle-address) provided by Galadriel team: 0x4168668812C94a3167FCd41D12014c5498D74d7e.

4. Install dependencies
   Install the dependencies using npm:
```
   # In repo root -> /contracts
   npm install
 ```
5. Deploy contract to devnet
   The [quickstart contract](https://github.com/galadriel-ai/contracts/blob/main/contracts/contracts/Quickstart.sol) can be deployed with a [simple script](https://github.com/galadriel-ai/contracts/blob/main/contracts/scripts/deployQuickstart.ts):
  ```
npm run deployQuickstart
```
The output of the script will show the deployed contract address. Store this and export it in terminal to call the contract later:
```
# Replace with your own contract address
export QUICKSTART_CONTRACT_ADDRESS=0x...
```

## 💡 Calling your contract
Prerequisites:
- You’ve deployed the quickstart contract in the previous step, and stored the contract address.
  Execute the following command to run a [script](https://github.com/galadriel-ai/contracts/blob/main/contracts/scripts/deployQuickstart.ts) that calls the deployed contract:

   ```
  npm run callQuickstart
  ```

The script will interactively ask for the input (DALL-E prompt: what image should be generated) and then call the contract with the input. The output, when ready, will be printed to the console.
If this step fails, make sure you have set the ||QUICKSTART_CONTRACT_ADDRESS|| environment variable to the address of your deployed contract.

🎉 You’re done! You’ve successfully created and called your own on-chain AI app.

## 🤳 Screenshots <a name = "screenshots"></a>
[galadriel Image URL](https://storage.googleapis.com/galadriel-assets/7c749d04-737b-40c2-b0f4-3a9b266eb9c3.png)

![7c749d04-737b-40c2-b0f4-3a9b266eb9c3](https://github.com/Bild96/Smart-Agent/assets/52472445/f48f53e4-0470-47c0-861f-8c26bfb4eec0)

## ⛏️ Built With <a name = "tech_stack"></a>
<img alt="python" src="https://img.shields.io/badge/python-%231572B6.svg?&style=for-the-badge&logo=python&logoColor=yellow"/><img alt="Typescript" src="https://img.shields.io/badge/typescript-%23563D7C.svg?&style=for-the-badge&logo=typescript&logoColor=white"/>

## ✍️ Authors <a name = "authors"></a>

 🧑‍💻 [Bild96](https://x.com/bild96)


## 🎉 Acknowledgments <a name = "acknowledgments"></a>
 🏗️ [ETHGlobal HackFS © 2024](https://ethglobal.com)
  <h1 align="left">
  <a href="https://discord.gg/ethglobal"><img src="static/Join-Discord.png" width="380" alt="Join Discord"></a>
 </h1>
 
#### 🪙 Want to show support? Just spread the word and smash the ⭐ star button
###### Donate ETH: ***0xfd7a470001364d707c81074142b6aC9248B0b0cc***
  

  



 

   









