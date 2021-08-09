### Setup 

```sh
yarn
```

### Run tests

 First setup the Theta local privatenet with the Theta/Ethereum RPC Adaptor [following this guide](https://docs.thetatoken.org/docs/setup-local-theta-ethereum-rpc-adaptor). The ETH RPC adaptor running at `http://localhost:18888/rpc` interacts with the javascript code by translating the Theta RPC interface into the ETH RPC interface. Then, run the tests with the following commands:

```sh
npx hardhat test --network theta_privatenet

npx hardhat test test/SushiBar.test.ts --network theta_privatenet
npx hardhat test test/SushiToken.test.ts --network theta_privatenet
```
