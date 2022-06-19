# s06_tokenization
AssetTokenization
# Technologies:
- Solidity: 
    It is an object-oriented programming language created specifically by the Ethereum Network team for constructing and designing smart contracts on Blockchain platforms. It's used to create smart contracts that implement business logic and generate a chain of transaction records in the blockchain system.
    
- Truffle: 
    It is a Development Environment, Testing Framework and Asset pipeline for Ethereum Blokchains. Ganache : Ganache is a personal Ethereum Blockchain used to test smart contracts where you can deploy contracts, develop applications, run tests and perform other tasks without any cost.
    
- Infura:
    provides the tools and infrastructure that allow developers to easily take their blockchain application from testing to scaled deployment - with simple, reliable access to Ethereum and IPFS.
    
- OpenZeppelin Contracts:
     helps you minimize risk by using battle-tested libraries of smart contracts for Ethereum and other blockchains. It includes the most used implementations of ERC standards.
     
- metamask:
      is a free web and mobile crypto wallet that allows users to store and swap cryptocurrencies, interact with the Ethereum blockchain ecosystem, and host a growing array of decentralized applications (dApps). It is one of the most widely used crypto applications in the world.
      
- React:
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
