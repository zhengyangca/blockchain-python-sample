## BlockChain in Python and Flask
* Flask-RESTful API + Mine + Distributed Ledger + Consensus


![BlockChain Demo](https://raw.githubusercontent.com/zhengyangca/FlaskBlockChain/master/static/title_img.png =500x300)



## Note

If you wish to get familiar with the recently famous concepts of **blockchain(and Cryptocurrencies)**, and even more details on how it works in **python** code, this repo will provide you a brief and clear sample and appropriate comments to help understand.

## Prepare
Make sure you have Python 3 installed:

`brew install python3`

or update

`brew update python`

## Usage

clone the repo to your local

`git clone https://github.com/zhengyangca/FlaskBlockChain`

then install required packages

`pip install -r requirements.txt`

Access the root directory and launch the Blockchain Web Services:

`cd ~/path-to-your-local-repo`

`python FlaskBlockChain.py`

## APIs:


### 1. Mine
`http://localhost:5000/mine`

### 2. Transactions
Use Postman or cURL make a post with json values:

`localhost:5000/transactions/new`

with raw value:

    {
     "sender": "4bb926b6dca14df48a664f2e6fbd559e", // change 
      to your client ID. 
     "recipient": "someone else's address",
     "amount": 5
    }

### 3. Check all chains of transactions
`localhost:5000/chain`