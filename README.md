# Interacting-with-Koii-Attention-State-Data

The network uses task-based infrastructure, so nodes have REST API interfaces that which can be accessed using a web URL and the data displayed in JSON format which is easily accessible. 

## What's Inside?

All the data in the Koii Attention state can be accessed [`https://mainnet.koii.live/attention/`](https://mainnet.koii.live/attention/) which returns a result similar to the screenshot below.



![Screenshot from 2022-01-21 20-27-54](https://user-images.githubusercontent.com/47121187/150548908-18847582-8feb-470e-b7c8-1a2be4386739.png)

This JSON data has all the info in the respective order:
* Attention Contract Owner Address
* Name of the Attention Contract
* List of all the NFTs with Owners
* Tasks related all the information
* Reputation of the Attention Contract
* A list of all the Valid Contract Sources


## Searching Information for a particular NFT

To search for any information related to any NFT, follow the steps below:

1. Lookup for the NFT ID on [Viewblock](https://viewblock.io/) via Finnie Wallet by clicking on Explore Block under the NFT title. 
![Screenshot from 2022-01-24 21-36-15](https://user-images.githubusercontent.com/47121187/150820034-bdb33381-cbf8-4c6c-a430-1624aef883e4.png)

2. Copy your NFT ID (*See image illustration below.*)
![Screenshot from 2022-01-21 22-22-06](https://user-images.githubusercontent.com/47121187/150568967-cbd72b91-d4f0-4026-ac8d-92b5466b01d3.png)

3. Hit the URL `https://mainnet.koii.live/attention/nft?id=[PASTE YOUR NFT ID HERE]` *Remove the square brackets when you put your NFT ID.*

4. All the information pertaining to the NFT ID will be displayed in JSON.
![Screenshot from 2022-01-21 22-37-18](https://user-images.githubusercontent.com/47121187/150569694-8bb7b883-bf56-4b01-a11d-61084132fddc.png)

The information we get after querying a particular NFT ID is in the following order:
* owner : Address of the NFT Owner
* title : NFT Title
* name : Name provided while registering the NFT
* description : Description of the NFT
* ticker : 
* balances : Wallet balance of the NFT Owner	
* contentType	: NFT Content Type 
* createdAt	: When was the NFT created
* id	: NFT ID of the NFT
* next	: NFT ID of the next NFT in series
* prev	: NFT ID of the previous NFT in series
* attention	: Attention gained by the respective NFT
* reward	: Rewards earned for the NFT
