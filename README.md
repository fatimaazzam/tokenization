# tokenization
## Asset Tokenization:
- In our project, we will build a simple asset tokenization for fungible tokens using solidity to write our smart contacts and also we will use the ERC20 open-zeppelin contracts. For local development we will use Truffle. Then we will deploy our smart contract using Infura.

Tokenization of assets, or simply put, asset tokenization is a process involving the transformation of assets on the blockchain. It includes physical as well as non-physical assets and applies to industries including finance, art, real estate, and health care. It is just the way of digitizing tangible and intangible assets and transforming them into tokens. However, a given acid is not necessarily equal to a single token as these are usually fragmented into smaller sections forming a whole token.

- There are two types of assets:

    - Fungible asset tokenization.Each unit of the tokenized asset has the same market value and validity, for example, Bitcoin: All units of 1 BTC are exactly the same. They hold the same market value, and are interchangeable. It doesn't matter from whom a BTC was purchased, since all BTC units have the same functionality and are part of the same network. You can swap one-fourth of a BTC for anyone else's one-fourth of a BTC, with confidence that your BTC’s one-fourth holds the same value, despite being one-fourth of different coins. A fungible cryptocurrency can be divided into as many decimal places which were configured during its issuance. Each unit will have the same value and validity.
    
    
   - Non-fungible asset tokenization. NFTs can't be replaced with tokens of the same type because each token represents a unique value. NFTs are not typically divisible, although F-NFTs do offer fractional ownership of NFTs, such as in the case of expensive fine art or commercial real-estate. Each token differs from another token of the same type and has unique information and attributes.
    


# Technologies:
- ## Solidity: 
    It is an object-oriented programming language created specifically by the Ethereum Network team for constructing and designing smart contracts on Blockchain platforms. It's used to create smart contracts that implement business logic and generate a chain of transaction records in the blockchain system.
    
- ## Truffle: 
    It is a Development Environment, Testing Framework and Asset pipeline for Ethereum Blokchains. Ganache : Ganache is a personal Ethereum Blockchain used to test smart contracts where you can deploy contracts, develop applications, run tests and perform other tasks without any cost.
    
- ## Infura:
    provides the tools and infrastructure that allow developers to easily take their blockchain application from testing to scaled deployment - with simple, reliable access to Ethereum and IPFS.
    
    We create new project in Infura:
    ![Infura](https://user-images.githubusercontent.com/27667600/174467988-278d2916-166c-4b6d-8b78-aedc45908e7d.PNG)

    
- ## OpenZeppelin Contracts:
     helps you minimize risk by using battle-tested libraries of smart contracts for Ethereum and other blockchains. It includes the most used implementations of ERC standards.
     
- ## Metamask:
      is a free web and mobile crypto wallet that allows users to store and swap cryptocurrencies, interact with the Ethereum blockchain ecosystem, and host a growing array of decentralized applications (dApps). It is one of the most widely used crypto applications in the world.
      
- ## React:
     Component-based front-end library responsible only for the view layer of the application.

# Project Digarmas:
- In our project we use ERC 20 smart contract which is imported from open-zeppelin contract. So the contract is function wise complete. Then this contract will be deployed on test-net through Infura. We will have some sort of UI which an HTML written in react and connected to MetaMask. Blockchain basically will be our database.

 ![Component_digram](https://user-images.githubusercontent.com/27667600/174467411-2ad32f2f-5b45-45e4-b037-1ffe0ce53a53.png)

- As shown in the figure above there are three main components:

   -  ERC 20 Token smart contract:
    As mentioned previously we used open-zeppelin contracts framework, so ERC 20 will be imported from zeppelin framework.
   - Initial Supply to Owner: 
    Full amount of tokens are minted and assigned to the owner.
   - Initial Crowd-sale contract:
    External people can buy tokens, then shift token from owner to the crowd- sale people and also they can sell these token to other peoples. 
    
 ![Activity_Diagram](https://user-images.githubusercontent.com/27667600/174467464-57ae83d8-0f9e-4fc8-96cd-95726b54e7d1.png)
 
 When the crowd-sale people sell a token they will send money to the crowd-sale contract by transaction and then they will get the token back. Since
this process is not easy in the production or the main network, we need to take care of the address that the crowd-sale people send money to, so we build Kyc mock contract to check the whitelist addresses.

# Application:
When the user click on buy token button then Metamask is opened directly, so the user can then click on confirm or reject the transaction as shown in the figure below:
![Metamask](https://user-images.githubusercontent.com/27667600/174467715-9510c895-06aa-4063-8018-18ee69e95a7f.PNG)

In case the user confirm the transaction from his wallet (Metamask) then the number of token will be incremented and a gase fees amount will be deducted from the user wallet. And also the user can view his transaction as shown in the figure below:

![transaction](https://user-images.githubusercontent.com/27667600/174467905-0b3a425b-1df3-4dee-b485-1ba5e6578261.PNG)



