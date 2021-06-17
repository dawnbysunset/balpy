# balpy
Python tools for interacting with Balancer Protocol V2 in Python. 

DISCLAIMER: While balpy is intended to be a useful tool to simplify interacting with Balancer V2 Smart Contracts, this package is an ALPHA-build and should be considered as such. Use at your own risk! This package is capable of sending Ethereum tokens controlled by whatever private key you provide. User assumes all liability for using this software. Users are STRONGLY encouraged to experiment with this package on testnets before using it on mainnet with valuable assets.

## Usage

### Install
python3 -m pip install balpy

### Build from source
git clone https://github.com/gerrrg/balpy.git

cd balpy

python3 -m build

### Environment Variables
You must set three environment variables in order to use the balpy module
- KEY_API_ETHERSCAN: 	API key for Etherscan for gas prices
- KEY_API_INFURA: 		API key for Infura for sending transactions
- KEY_PRIVATE: 			Plain text private key for signing transactions

## Samples
After installing...

cd samples

**For pool creation**

python3 poolCreationSample.py samplePool.json

**For swap samples**

python3 batchSwapSample.py sample{Single/Multihop/Flash}Swap.json