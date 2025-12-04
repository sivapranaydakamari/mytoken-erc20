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
9. Enter total supply (example for 1M tokens with 18 decimals)  
10. Click **Deploy**

---

## How to Use

### **Check Token Information**
```solidity
name()        // returns "MyToken"
symbol()      // returns "MTK"
decimals()    // returns 18
totalSupply() // returns total token supply
```

---

### **Check Balance**
```solidity
balanceOf(address) // returns uint256
```

---

### **Transfer Tokens**
```solidity
transfer(receiverAddress, amount)
```

---

### **Approve a Spender**
```solidity
approve(spenderAddress, amount)
```

---

### **Delegated Transfer (Using Allowance)**
```solidity
transferFrom(senderAddress, receiverAddress, amount)
```
---

### Testing Performed
* Contract compiled successfully
* Deployed using Remix JavaScript VM
* Verified name, symbol, decimals, totalSupply
* Tested balanceOf for deployer
* Successfully transferred tokens using transfer
* Approved another account using approve
* Executed delegated transfer using transferFrom
* Confirmed allowance decreases correctly
* Tested failure cases (invalid transfers, no approval, zero address)

---

### Conclusion
The MyToken contract implements all major ERC-20-style functionalities, works flawlessly in Remix IDE, and is suitable for educational or demo purposes.
All functions were tested and verified successfully, including transfers, approvals, and delegated transactions.