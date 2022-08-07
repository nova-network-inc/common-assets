# Shared Common Assets

This repository brings an array of common assets used across different Nova Network
platforms and dApps, and can be used by fellow projects to fetch up to date data
and commonly used assets - such as logos, etc.

## Fetching Raw Data

To fetch the raw data and use it with your own platform, you can call the URL below,
adding the exact path of the file you want to fetch in the end.

```shell
https://raw.githubusercontent.com/nova-network-inc/common-assets/main/
```

Eg. `https://raw.githubusercontent.com/nova-network-inc/common-assets/main/chain-lists/chains/eip155-87.json`

## Pull Requests

We welcome community contributions to this repository. Just make sure to follow
the appropriate `json` and/or other file standards while submitting your pull
request. Otherwise, it will not be approved and merged.

You can find more information on the file standards inside each asset parent
folder's `README.md`.

## Currently Listed Assets

This is a live repository, so expect frequent changes and new commits.

```shell
|- chain-lists    -   Lists known EVM networks.
|- token-info     -   Lists ERC20 token information in multiple chains.
|- token-lists    -   Compiled token lists used by our protocols.
```
