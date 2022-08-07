# Fusion Tokens List

This is the list used by Fusion to compile its whitelisted tokens in all compatible
networks. Unless arranged otherwise, all projects to be listed need to submit a
pull request with their token information.

## Pull Requests

When submitting a pull request for adding a token, please follow the `json` standard
below, with special attention to the `isAggregator` field.

We also require all tokens being listed to be added to our [`/token-info`]
(https://github.com/nova-network-inc/common-assets/tree/main/token-info) repository,
so we can fetch both the logo and the token information easily for further integration
with Fusion and other Nova Network dApps.

`isAggregator` is used by the protocol to determine where to look for liquidity
first when processing a trade. If `true`, the protocol will actively try to route
the trade via its aggregator contract, using other protocols' liquidity to do so.
When `false`, the protocol will primarily look to its own router to find liquidity
to process the trade. This option is set to `false` by default.

```shell
{
  "chainId": 87,
  "address": "0x657a66332A65B535Da6C5d67b8cD1D410c161a08",
  "symbol": "WSNT",
  "name": "Wrapped SNT",
  "decimals": 18,
  "logoURI": "https://raw.githubusercontent.com/nova-network-inc/common-assets/main/token-info/0x657a66332A65B535Da6C5d67b8cD1D410c161a08/logo.png",
  "tags": ["wrapped", "snt"],
  "isAggregator": false
},
```
