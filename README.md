# MyToken (MTK)

## Overview
MyToken is a simple ERC-20 compatible token built on Ethereum for learning and demonstration purposes.  
The contract includes all essential ERC-20 functions such as transferring tokens, approving spenders, and performing delegated transfers using `transferFrom`.

---

## Token Details
- **Name:** MyToken  
- **Symbol:** MTK  
- **Decimals:** 18  
- **Total Supply:** 1,000,000 MTK (1 million tokens, supplied during deployment)

---

## Features
- ✅ Standard ERC-20 style implementation  
- ✅ Transfer tokens between addresses  
- ✅ Approve and `transferFrom` functionality  
- ✅ Event emission for transparency (`Transfer`, `Approval`)  
- ✅ Balance tracking using mappings  
- ✅ Fully tested in Remix IDE  

---

## How to Deploy

1. Open **Remix IDE** → https://remix.ethereum.org  
2. Create a new file named **`MyToken.sol`**  
3. Paste the full contract code  
4. Go to **Solidity Compiler**  
5. Select compiler version **0.8.30**  
6. Click **Compile MyToken.sol**  
7. Go to **Deploy & Run Transactions**  
8. Select **JavaScript VM**  
9. Enter total supply (example for 1M tokens with 18 decimals):  
10. Click **Deploy**

---

## How to Use

### Check Token Information
```solidity
name()        // returns "MyToken"
symbol()      // returns "MTK"
decimals()    // returns 18
totalSupply() // returns total token supply

### **Check Balance**
```solidity
balanceOf(address) // returns uint256

### Transfer Tokens
```solidity
transfer(receiverAddress, amount)

### Approve a Spender
```solidity
approve(spenderAddress, amount)

### Delegated Transfer (Using Allowance)
```solidity
transferFrom(senderAddress, receiverAddress, amount)

