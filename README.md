# Metacrafter_ETH_AVAX_Proof_IntermediateEVM_Module2_ProjectAssessment
This repository contains the code for the Intermediate EVM Project Assessment of the Metacrafter course. The project demonstrates the integration of a Solidity smart contract with a frontend DApp, allowing users to deposit and withdraw Ether from their account using MetaMask on a local Ethereum network.
## Description
This project showcases a decentralized application (DApp) built using Solidity smart contracts and a React frontend powered by Next.js. The DApp allows users to interact with the Ethereum blockchain, specifically with a smart contract that manages a message and a favorite number. Additionally, the contract includes functionality to set the message length dynamically.
## Project Overview
The project includes:
**Solidity Smart Contract:** A smart contract that manages deposit and withdrawal functionality.
**Frontend DApp:** A React-based frontend that interacts with the smart contract using MetaMask and ethers.js.
**MetaMask Integration:** Allows users to connect their MetaMask wallet and interact with the contract to perform transactions.
## Features
 Smart Contract Interaction: Users can connect their MetaMask wallet to interact with the deployed Solidity smart contract.
* **Message Management:** Users can view and update a message stored on the blockchain.
  ```
  function getMessage() public view returns (string memory) {
        return message;
    }

    function setMessage(string memory newMessage) public {
        message = newMessage;
        emit MessageChanged(newMessage);
    }
  ```
 
* **Favorite Number:** Users can view and update their favorite number through the DApp.
  ```
   function getFavoriteNumber() public view returns (uint256) {
        return favoriteNumber;
    }

    function setFavoriteNumber(uint256 newNumber) public {
        favoriteNumber = newNumber;
        emit FavoriteNumberChanged(newNumber);
  }
  ```
  
* **Dynamic Message Length:** The contract allows users to set the maximum allowed length for the message, demonstrating dynamic contract functionalities.
```
function getValue() public view returns (uint256) {
        return value;
    }

    function setMessageLength(uint256 newLength) public {
        emit MessageLengthSet(newLength);
    }
```

## Interacting with the Contract
1. **View Current Message and Favorite Number:**
* Connect your MetaMask wallet.
* The DApp will display the current message and favorite number automatically.

2. **Update the Message:**
* Enter a new message in the input field.
* Click "Update Message" and confirm the transaction in MetaMask.

3. **Update the Favorite Number:**
* Enter a new favorite number in the input field.
* Click "Update Favorite Number" and confirm the transaction in MetaMask.

4. **Set Message Length:**
* Enter a new maximum length for the message in the input field.
* Click "Set Message Length" and confirm the transaction in MetaMask.

# Authors
Nikita Sharma

# License
MIT License
