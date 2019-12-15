# CMSC 491 - Blockchain final project
This is the front end for the tendermint blockchain system. 

To run the front end on a linux machine you will need [`npm`](https://www.npmjs.com/).

Once npm is installed run the following commands from the root directory of the cloned project. 

    npm install
  
    npm run serve
  
### Running the back end tendermint blockchain
1. Enable indexing in the tendermint config. 
    
        index_all_tags = true

2. Run the standard tendermint example blockchain `kvstore` or `persistent_kvstore`. 
        
        tendermint init
        tendermint node --proxy_app=kvstore

      or

        tendermint init  
        tendermint node --proxy_app=persistent_kvstore

