# HiFiSwap Interface

## Accessing the HiFiSwap Interface

To access the HiFiSwap Interface, use an IPFS gateway link from the
[latest release](https://github.com/HiFiSwap/HiFiSwap-interface/releases/latest), 
or visit [app.HiFiSwap.org](https://app.HiFiSwap.org).

## Development

### Install Dependencies

```bash
yarn
```

### Run

```bash
yarn start
```

### Configuring the environment (optional)

To have the interface default to a different network when a wallet is not connected:

1. Make a copy of `.env` named `.env.local`
2. Change `REACT_APP_NETWORK_ID` to `"{YOUR_NETWORK_ID}"`
3. Change `REACT_APP_NETWORK_URL` to e.g. `"https://{YOUR_NETWORK_ID}.infura.io/v3/{YOUR_INFURA_KEY}"` 

Note that the interface only works on testnets where both 
[HiFiSwap V2](https://HiFiSwap.org/docs/v2/smart-contracts/factory/) and 
[multicall](https://github.com/makerdao/multicall) are deployed.
The interface will not work on other networks.

## Contributions

**Please open all pull requests against the `master` branch.** 
CI checks will run against all PRs.

## Accessing HiFiSwap Interface V1

The HiFiSwap Interface supports swapping against, and migrating or removing liquidity from HiFiSwap V1. However,
if you would like to use HiFiSwap V1, the HiFiSwap V1 interface for mainnet and testnets is accessible via IPFS gateways 
linked from the [v1.0.0 release](https://github.com/HiFiSwap/HiFiSwap-interface/releases/tag/v1.0.0).
