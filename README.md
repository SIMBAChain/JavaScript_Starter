# JavaScript_Starter
Starter code for working with javascript and Simba

This is a simple collection of code for importing a wallet from a seed, saving & loading that wallet, 
and signing transactions using that wallet.

The code some requires additions and modifications for usage withing a smart contract. For instance generating
a wallet from scratch instead of just importing it.
* note: you can generate a random seed by calling "ethers.Wallet.createRandom()"

The code uses two libraries, Secure-ls and Ethers. Secure-ls saves and loads the wallet. Ethers generates the wallet
and signs transactions.

## Links
### Ethers
* https://github.com/ethers-io/ethers.js/
### Secure-ls
* https://github.com/softvar/secure-ls
### Networking
While no networking is done within this demo code your Simba app will require code for executing network requests.
For this task you may want to consider using a library to make this easier such as Axios.
* https://github.com/axios/axios

# View the project on Github pages
* https://simbachain.github.io/JavaScript_Starter/
