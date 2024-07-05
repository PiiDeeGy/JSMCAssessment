---

# NFT Minting Project

## Overview
The NFT Minting Project is a simple implementation for creating and managing NFTs (Non-Fungible Tokens) using JavaScript. This project demonstrates the basic functionality of minting NFTs, listing their metadata, and retrieving the total supply of minted NFTs.

## Description
This project allows you to create NFTs by minting them with specific metadata, store these NFTs in an array, and display their details. The key functions include minting new NFTs, listing all NFTs with their metadata, and getting the total supply of NFTs.

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

## Authors
- Angel Cruz - https://github.com/PiiDeeGy

---
