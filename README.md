# Leverdex SDK

To use this repo with its sister repositories, do the following.

```bash
cd ../leverdex-core
git clone git@github.com:leverdex/core-abi.git build/

# this overwrites your addresses file
npx hardhat node 

cd build
yarn link

cd ../../leverdex-sdk

yarn link @leverdex/core-abi
yarn build
yarn link

cd ../leverdex-interface
yarn link @leverdex/core-abi
yarn link @leverdex/sdk
```
