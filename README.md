# Avax-ERC20-token-creator



# Pre-requisite:
  
 
# Creating the ERC-20 Token:

  * Lets goto remix and create our mintable token. 
    * Visit this link: https://remix.ethereum.org/#optimize=false&runs=200&evmVersion=null&version=soljson-v0.8.4+commit.c7e474f2.js to open remix IDE.
  
  * You will be having an default workspace, delete that workspace by clicking on delete Icon.
  * Now create a new workspace by clicking on add icon
  * After this click on file icon to add a file
  * Since we will use an ERC-20 contract from OpenZeppelin, just paste this line to the file and save.
    * import "https://github.com/OpenZeppelin/openzeppelin-contracts/blob/master/contracts/token/ERC20/presets/ERC20PresetMinterPauser.sol";
  * Now save the file and you will see a bunch of files imported on remix IDE, this is the feature of remix that allows us to import a GitHub contract repository to remix by just giving the URL-Link. with an import statement.
  
  *  In these files there is one file named as "ERC20PresetMinterPauser.sol" file,this file is written by OpenZeppelin according to ERC20 standards with minter functionality. After deploying this file, we will be the owner of the contract and thus have the authority and ability to mint the tokens.
  
  * Now in your remix IDE open the "Compiler", which is present in second tab in your remix IDE and and select the solidity version that matches with the solidity version written in file as "pragma solidity …..".The version should be equal to or greater than the file's version.The compiler didn't showed any errors and compiled the file successfully.
  
  * Now lets move to the third tab of your remix IDE which is "DEPLOY & RUN TRANSACTION.". Before deploying your contract, click on environment and choose "Injected web3".Now metamask wallet pop-up will appear asking you to connect the account, click on connect.
  
  * The last thing before the deployment process is to set the contract that will be deployed as a token. Above the Deploy Button, there is a drop-down menu to select a contract. Select the contract named "ERC20PresetMinterPauser.sol".
