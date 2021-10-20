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

## Bug Bounty

The Solv Protocol bug bounty program is on the Immunefi platform and can be accessed at:
[https://www.immunefi.com/bounty/solvprotocol](https://www.immunefi.com/bounty/solvprotocol)

The bug bounty program is focused on the smart contracts and focused on preventing:

- Loss of user funds staked (principal) by freezing or theft
- Theft of unclaimed yield
- Freezing of unclaimed yield
- Smart contract fails to deliver promised returns

### Rewards by threat level

Rewards are distributed according to the impact of the vulnerability based on the Immunefi Vulnerability Severity Classification System.

#### Smart Contracts and Blockchain

| Threat Level | Bounty |
| :--- | :--- |
| Critical | USD $50,000 |
| High | USD $25,000 |
| Medium | USD $10,000 |
| Low | USD $3,000 |


All Critical/High severity bug reports must come with a PoC and a suggestion for a fix in order to be considered for a reward.

Payouts are handled by the Solv Protocol team directly and are denominated in USD. Payouts are done in USDT.
