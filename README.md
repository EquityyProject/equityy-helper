# solv-v2-helper

`solv-v2-helper` contains the helper contracts and deployment scripts for the contracts of [`solv-v2-voucher`](https://github.com/solv-finance-dev/solv-v2-voucher) and [`solv-v2-market`](https://github.com/solv-finance-dev/solv-v2-market).


## Structure

- [helpers](./helpers)

  - `helpers` mainly contains the helper contracts that are used to transfer ERC20 tokens and VNFT tokens

- [plugins](./plugins)

	- `plugins` contains the scripts used for deploying contracts: 
		- [`gasNowPrice`](./plugins/gasNowPrice.js) fetches the newest gas price before deploying;
		- [`otherDeployment`](./plugins/otherDeployment.js) solves the deployment dependencies of the contract to be deployed.
		- [`ozUpgrade`](./plugins/ozUpgrade.js) is used to deploy or upgrade a contract.

- [proxy](./proxy)

	- `proxy` contains the core contracts for implementing the Proxy Pattern of a contract.
