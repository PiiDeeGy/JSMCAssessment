---

# NFT Minting Project

## Overview
The NFT Minting Project is a simple implementation for creating and managing NFTs (Non-Fungible Tokens) using JavaScript. This project demonstrates the basic functionality of minting NFTs, listing their metadata, and retrieving the total supply of minted NFTs.

## Description
This project allows you to create NFTs by minting them with specific metadata, store these NFTs in an array, and display their details. The key functions include minting new NFTs, listing all NFTs with their metadata, and getting the total supply of NFTs.

## Getting Started

### Installing
To set up and run the NFT Minting Project, follow these steps:

1. Clone the repository:
   git clone https://github.com/yourusername/NFT-Minting-Project.git

2. Navigate to the project directory:
   cd NFT-Minting-Project

### Executing Program
To run the program, follow these steps:

1. Open the project in your preferred code editor (e.g., VS Code).
2. Ensure you have Node.js installed on your system.
3. Run the script:
   node nftMinting.js

The script includes the following key functions:

- **mintNFT**: This function takes in parameters for the NFT's metadata (name, eye color, shirt type, bling) and creates an NFT object. The object is then stored in an array.
  function mintNFT(_name, _eyeColor, _shirtType, _bling) {
      const NFT = {
          "name": _name,
          "eyeColor": _eyeColor,
          "shirtType": _shirtType,
          "bling": _bling
      }
      NFTs.push(NFT);
      console.log("\nMinted: " + _name);
  }

- **listNFTs**: This function iterates through the array of NFTs and prints their metadata to the console.
  function listNFTs() {
      for(let i = 0; i < NFTs.length; i++) {
          console.log("\nID: \t\t\t\t" + (i+1));
          console.log("\nName: \t\t\t\t" + NFTs[i].name);
          console.log("\nEye Color: \t\t\t" + NFTs[i].eyeColor);
          console.log("\nShirt Type: \t\t" + NFTs[i].shirtType);
          console.log("\nBling: \t\t\t\t" + NFTs[i].bling);
      }
  }

- **getTotalSupply**: This function prints the total number of minted NFTs.
  function getTotalSupply() {
      console.log("\nNFT Total Supply: \t" + NFTs.length);
  }

### Help
If you encounter any issues, here are some common problems and solutions:

- **Script execution error**: Ensure Node.js is installed and properly set up on your system. Verify the file path and name when running the script.
- **Metadata not displaying correctly**: Check that the parameters passed to the `mintNFT` function match the expected format.

## Authors
- Angel Cruz - https://github.com/PiiDeeGy

---
