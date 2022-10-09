# lottery-smart-contract
A simple ethereum smart contract that models a lottery.

How it works:
  - to take part in the lottery every user needs to send some amount of money (which cannot be less than 0.01 ETH for each user).
  - after some people have entered the contract a "third-party"(manager of the contract) will ask the contract to pick a winner,
    beware that he does not pick the winner itself the contract does that.
  - after it picks the winner the contract sends him the full amount and resets the contract to the initial state. 
  
  How to setup:
  * You can use ```node deploy.js``` to deploy it using Infura API in the Ethereum network.
  * You need to set the 12-word secret recovery phrase of your account in order to be able to deploy it.
  * The contract is thoroughly tested using Mocha testing framework on the Ganache network.
