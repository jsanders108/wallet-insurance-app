This is a full-stack Solidity wallet insurance app. A customer may purchase insurance for a crypto wallet and be covered for up to 50 ETH in case of a hack. There are 2 policy types: 

  1) For 0.02 ETH, a customer may purchase coverage for up to 50 ETH for 30 days.
  2) For 0.01 ETH, a customer may purchase coverage for up to 25 ETH for 30 days. 

This app's smart contracts are currently deployed on the Polygon Mumbai testnet (due to high gas fees on the Goerli ETH testnet). The app employs the "factory" method: when a customer purchases a new insurance policy, a new smart contract for that specific policy is created and deployed each time by the "Wallet Policy Factory Contract". 

The "Wallet Depository" smart contract holds all the funds deposited by customers when purchasing their insurance policies. The Wallet Depository pays out claims that are approved by the administrator. It is also possible for the administrator to deposit funds into the Compound Finance defi protocol (and get cETH tokens in return) to earn a yield (this functionality will be possible when deployed to Goerli or mainnet Ethereum). 

The app can be accessed at the following website:
