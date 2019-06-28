# JavaScript_Starter
Starter code for working with javascript and Simba

This is a simple collection of code for importing a wallet from a seed, saving & loading that wallet, 
and signing transactions using that wallet.

The code some requires additions and modifications for usage withing a smart contract. For instance generating
a wallet from scratch instead of just importing it.
* note: you can generate a random wallet by calling "ethers.Wallet.createRandom()"

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

#### The project itself didn't really have a spot for executing network code so here is some general code for executing GET/POST methods.


* Get

  axios.get('https://api.simbachain.com/v1/YOUR_API_NAME/YOUR_METHOD/',{
        headers: {
                'APIKEY' : 'YOUR API KEY'
            }})
            .then(function (response) {
            //Handle Response/Display data
            })
            
            
* Post

    //setup the form data needed for posting
        var myBody = new FormData;
        //after myBody is declared you can append the info you need to post
        myBody.append("from",USERS_PUBLIC_KEY);
       

        //the post command itself
        axios.post('https://api.simbachain.com/v1/YOUR_API_NAME/YOUR_METHOD/', myBody, {
            headers: {
                'APIKEY' : 'YOUR API KEY HERE'
            }})
  .then(function (response) {
       //handle the response by displaying data and signing the transaction    
    })
  .catch(function (error) {
    //handle error codes
  });
  



# View the project on Github pages
* https://simbachain.github.io/JavaScript_Starter/
