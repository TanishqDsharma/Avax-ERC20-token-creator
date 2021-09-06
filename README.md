# Introduction

* ERC-20 tokens are the most fundamental and essential concept in Ethereum.As the Avalanche community and the ecosystem are growing, new use cases and projects that are running on Ethereum or different chains would be implemented to Avalanche.

* Therefore, In this tutorial we will be minting ERC20 on Avalanche using Open Zeppelin.The token will be generated on Avalanche C-Chain and will be accessible on that chain.Further we will be using <b>"ERC20PresetMinterPauser.sol"</b> file,this file is written by OpenZeppelin according to ERC20 standards with minter functionality. After deploying this file, we will be the owner of the contract and thus have the authority and ability to mint the tokens.


## Requirements:

1) <b>Create a metamask wallet:</b>
   * <b>To create a wallet using metamask:</b>
     * Go visit metamask website:https://metamask.io/
     * The there click on "Download button" and add metamask extension according to your browser(Supported browsers are: Firefox, Chrome, Brave and Edge). 
     * Open the metamask extension and create an account for yourself
       * Follow my guide on creating a wallet on metamask:<a href="https://github.com/TanishqDsharma/Avax-ERC20-token-creator/blob/main/Metamask_wallet_setup_Guide.md">Wallet-Setup-Guide</a>
            
2) <b>Now, navigate to Settings-> Networks and Click on the "Add Network" button and enter the below Fuji Testnet Network settings:</b>
          
    * <b>Network Name:</b> Avalanche C-Chain
    * <b>New RPC URL:</b> https://api.avax-test.network/ext/bc/C/rpc
    * <b>Chain ID:</b> 43113
    * <b>Currency Symbol:</b> AVAX
    * <b>Block Explorer URL:</b>  https://cchain.explorer.avax-test.network
     
     
3) <b>Since we will be doing everything on testnet:</b>
          
    * <b>You can top-up your wallet with Avax from:</b> https://faucet.avax-test.network/
          
    * <b>Enter your wallet address to receive the funds.</b>
            
      ![alt text](https://github.com/TanishqDsharma/Avax-ERC20-token-creator/blob/main/avax-images/a1.png)
            
    * <b>After entering the address, click on "Request 10 Avax" and you will have your wallet funded.</b>
            
      ![alt text](https://github.com/TanishqDsharma/Avax-ERC20-token-creator/blob/main/avax-images/a2.png)

        
         
          
 
# Minting ERC-20 Token:

  1) <b>Lets goto remix and create our mintable token.</b>
      
      * <b>Visit this link:</b>
       
         ```json
         https://remix.ethereum.org/#optimize=false&runs=200&evmVersion=null&version=soljson-v0.8.4+commit.c7e474f2.js to open remix IDE.
         ```

  
  2) <b>You will be having an default workspace, delete that workspace by clicking on delete Icon.</b>
      
      ![alt text](https://github.com/TanishqDsharma/Avax-ERC20-token-creator/blob/main/avax-images/w1.png)
  
  3) <b>Now create a new workspace by clicking on add icon.</b> 
      
      ![alt text](https://github.com/TanishqDsharma/Avax-ERC20-token-creator/blob/main/avax-images/w2.png)
      
      ![alt text](https://github.com/TanishqDsharma/Avax-ERC20-token-creator/blob/main/avax-images/a3.png)
       
  4) <b>After this click on file icon to add a file and give a name to your file:</b>
      
      ![alt text](https://github.com/TanishqDsharma/Avax-ERC20-token-creator/blob/main/avax-images/a4.png)

  
  5) <b>Since we will use an ERC-20 contract from OpenZeppelin, just paste this line to the file and save.</b>
     
      ```
      import "https://github.com/OpenZeppelin/openzeppelin-contracts/blob/master/contracts/token/ERC20/presets/ERC20PresetMinterPauser.sol";
      ```
      
      ![alt text](https://github.com/TanishqDsharma/Avax-ERC20-token-creator/blob/main/avax-images/w3.png)

  6) <b>Now save the file and you will see a bunch of files imported on remix IDE, this is the feature of remix that allows us to import a GitHub contract repository to remix by just giving the URL-Link. with an import statement.</b>
     
      ![alt text](https://github.com/TanishqDsharma/Avax-ERC20-token-creator/blob/main/avax-images/a5.png)

     
  
  7) <b>In these files there is one file named as "ERC20PresetMinterPauser.sol" file,this file is written by OpenZeppelin according to ERC20 standards with minter functionality. After deploying this file, we will be the owner of the contract and thus have the authority and ability to mint the tokens.</b>
     
      ![alt text](https://github.com/TanishqDsharma/Avax-ERC20-token-creator/blob/main/avax-images/a6.png)

  
  8) <b>Now in your remix IDE open the "Compiler", which is present in second tab in your remix IDE and select the solidity version that matches with the solidity version written in file as "pragma solidity …..".The version should be equal to or greater than the file's version.The compiler didn't showed any errors and compiled the file successfully.</b>
      
      ![alt text](https://github.com/TanishqDsharma/Avax-ERC20-token-creator/blob/main/avax-images/a7.png)

  
  9) <b>Now lets move to the third tab of your remix IDE which is "DEPLOY & RUN TRANSACTION.". Before deploying your contract, click on environment and choose "Injected web3".Now metamask wallet pop-up will appear asking you to connect the account, click on connect.</b>
      
      ![alt text](https://github.com/TanishqDsharma/Avax-ERC20-token-creator/blob/main/avax-images/w6.png)  
  
  10) <b>The last thing before the deployment process is to set the contract that will be deployed as a token. Above the Deploy Button, there is a drop-down menu to select a contract. Select the contract named "ERC20PresetMinterPauser.sol".</b>
      
      ![alt text](https://github.com/TanishqDsharma/Avax-ERC20-token-creator/blob/main/avax-images/w5.png)

  11) <b>Now, enter the name and symbol of your token in the input fields. I named it as "Mangatoken" and the symbol that I gave is  "MKT".</b>
  
      ![alt text](https://github.com/TanishqDsharma/Avax-ERC20-token-creator/blob/main/avax-images/w4.png)
      
      <b>Finally, click on "transact button"</b>
      
      ![alt text](https://github.com/TanishqDsharma/Avax-ERC20-token-creator/blob/main/avax-images/a8.png)
      

  
  12) <b>After clicking the button, a pop-up will show up and just confirm it.</b>
      
      ![alt text](https://github.com/TanishqDsharma/Avax-ERC20-token-creator/blob/main/avax-images/a9.png)
  
  13) </b>And then another metamask pop-up will appear asking for confirmation.Confirm it.</b>
      
      ![alt text](https://github.com/TanishqDsharma/Avax-ERC20-token-creator/blob/main/avax-images/a10.png)
 
      
  14) <b>We can see our transaction deployed on avalache c-chain using metmask:</b>
      
      1) In your metamask wallet goto "Activity" Tab.
      2) Then select your "contract deployment" transaction.
      3) The metamask wallet will show you your transaction details, to view it on explorer follow the arrow icon:
         
         ![alt text](https://github.com/TanishqDsharma/Avax-ERC20-token-creator/blob/main/avax-images/a11.png)

  15) <b>Here we can see all details about the transaction and token contract:</b>
      
      ![alt text](https://github.com/TanishqDsharma/Avax-ERC20-token-creator/blob/main/avax-images/a12.png)
      
  16) <b>Now, visit remix IDE again and you will see your contract under deployed contracts.</b>
      
      ![alt text](https://github.com/TanishqDsharma/Avax-ERC20-token-creator/blob/main/avax-images/a13.png)
      
  17) <b>Here, we have lot of functions that we can use to interract with our contract but for this tutorial we will use the "mint" function.Enter your address and an amount in WEI and click on "transact" button.</b> 
      
      ![alt text](https://github.com/TanishqDsharma/Avax-ERC20-token-creator/blob/main/avax-images/a14.png)
      
      <b>Transaction in metamask:</b>
            
      * <b>Select the "mint" transaction:</b>
      
        
        ![alt text](https://github.com/TanishqDsharma/Avax-ERC20-token-creator/blob/main/avax-images/b4.png)

        
        ![alt text](https://github.com/TanishqDsharma/Avax-ERC20-token-creator/blob/main/avax-images/b5.png)
      
      So, I copied the address highlighted in the screenshot as i will be needing it to import my token in metamask.
      
  
  18) <b>Now, your tokens wont be visible directly in your metamask wallet so to make your tokens visible in your metamask wallet you have to add them.</b>
      
      
      <b>On metamask, click to "Add Token" button and select "Custom Token" tab:</b>
      
      ![alt text](https://github.com/TanishqDsharma/Avax-ERC20-token-creator/blob/main/avax-images/b1.png)
      
      
      
      <b>Add token contract address that you copied in step 17</b>
      
      
      ![alt text](https://github.com/TanishqDsharma/Avax-ERC20-token-creator/blob/main/avax-images/b2.png)
      
      
      <b>Click on "next" and you will have your token visible in your metamask wallet:</b>
      
      
      ![alt text](https://github.com/TanishqDsharma/Avax-ERC20-token-creator/blob/main/avax-images/b3.png)


      
 # Conclusion:
 
 1) By following all the steps in the above tutorial I was able to mint ERC20 on Avalanche using Open Zeppelin.
 2) By following the steps I was able to mint my own ERC20 token named as "Manga Token" on "Fuji Testnet" 
    
      



