# Pull Request Standards

## New Token Lists

To submit pull requests for adding new lists, please follow the `json` standard
below, and only submit new lists inside the `/public` directory. Submissions in
any other directories will not be accepted.

```shell
{
  "name": "Example List",
  "logoURI": "https://raw.githubusercontent.com/nova-network-inc/common-assets/main/token-info/_native/SNT/logo.png",
  "keywords": ["nova", "network"],
  "timestamp": "2022-02-20T18:18:00+00:00",
  "tokens": [
    {
      "chainId": 87,
      "address": "0x657a66332A65B535Da6C5d67b8cD1D410c161a08",
      "symbol": "WSNT",
      "name": "Wrapped SNT",
      "decimals": 18,
      "logoURI": "https://raw.githubusercontent.com/nova-network-inc/common-assets/main/token-info/0x657a66332A65B535Da6C5d67b8cD1D410c161a08/logo.png",
      "tags": ["wrapped", "snt"],
    }
  ],
  "version": {
    "major": 1,
    "minor": 0,
    "patch": 0
  }
}
```

## Add Tokens To Existing List

To add tokens to an existing list, just follow the same standard above, adding
your token information to the list you want and leaving everything else unchanged.
For every change, please add `+1` to the `patch` version of the list, so users can
keep track of the changes being made.

Example formatting:

```shell
{
  "chainId": 87,
  "address": "0x657a66332A65B535Da6C5d67b8cD1D410c161a08",
  "symbol": "WSNT",
  "name": "Wrapped SNT",
  "decimals": 18,
  "logoURI": "https://raw.githubusercontent.com/nova-network-inc/common-assets/main/token-info/0x657a66332A65B535Da6C5d67b8cD1D410c161a08/logo.png",
  "tags": ["wrapped", "snt"],
}
```

If you're making significant changes to an existing list, we recommend you to create
a new list instead.
